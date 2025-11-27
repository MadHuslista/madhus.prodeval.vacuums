# Guía de Evaluación de Productos con LLMs

---

## Resumen del Proceso

| Etapa | Descripción |
|-------|-------------|
| **1. Especificación** | Definir qué características buscar en el producto |
| **2. Candidatos** | Identificar productos disponibles en el mercado |
| **3. Inventario** | Organizar y consolidar la información recopilada |
| **4. Recomendaciones** | Generar conclusiones finales basadas en el análisis |

---

## 1. Generar la Especificación de Requerimientos

**Objetivo:** Descubrir todas las características importantes del producto y definir qué requisitos debe cumplir para satisfacer las necesidades específicas.

> **Nota:** Usae la LLM en "modo investigación", donde le pedimos que busque información en internet sobre el tema.

### Fase 1: Descubrimiento de Criterios

**Propósito:** Identificar todas las dimensiones relevantes para evaluar el producto.

**Prompt sugerido:**
```
"Revisa cuáles son todas las características importantes que debo tomar en
atención para escoger una <producto> para <escenario importante>"
```

**Ejemplo práctico:**
```
"Investiga qué características debo tomar en atención para escoger una
aspiradora automática para un piso vinílico"
```

> 💡 **Consejo:** Itera un par de veces si es necesario. Puedes hacer preguntas de seguimiento para profundizar en aspectos específicos.

### Fase 2: Creación de Especificaciones

**Propósito:** Obtener un documento estructurado (marco de trabajo) que servirá como base para identificar y evaluar candidatos.

**Prompt sugerido:**
```
"Crea una especificación de requerimientos en formato markdown con todos
los criterios comentados aquí, en consideración con el <escenario importante>"
```

> **¿Por qué Markdown?**
> Markdown es un formato de texto simple que permite crear documentos estructurados con títulos, listas y tablas. Las LLMs lo entienden muy bien y es fácil de leer tanto para humanos como para máquinas.

### Ejemplo Completo de Esta Fase

Puedes ver un ejemplo real de cómo completar esta fase usando Claude:
- 🔗 [Conversación de ejemplo en Claude](https://claude.ai/share/6a68ad16-d9bf-44f8-9c1c-ee56f92e9e1f)

---

## 2. Capturar Posibles Candidatos

**Objetivo:** Automatizar la recopilación de información sobre productos disponibles en el mercado, ahorrando tiempo en la búsqueda manual.

**Prompt sugerido:**
```
"Based on the <documento de especificaciones> archive, run a deep comprehensive
evaluation of the <product> available in the chilean market. Report a tier table
following the considerations indicated on the document."
```

> 💡 **Consejo:** A partir de la respuesta inicial, itera varias veces. Revisa la información, haz preguntas de seguimiento y permite que la LLM acumule datos sobre los aspectos que más te interesen.

### Ejemplo Completo de Esta Fase

Puedes ver un ejemplo real usando ChatGPT:
- 🔗 [Conversación de ejemplo en ChatGPT v4](https://chatgpt.com/share/69288c69-bd1c-8011-aa3a-ffd5c0c5ee1b)
  *(Nota: Con versiones más recientes como GPT-5, los resultados pueden ser aún mejores)*

---

## 3. Inventariar

**Objetivo:** Resumir y organizar toda la información acumulada en un formato estructurado y fácilmente consultable.

### Pasos a Seguir

1. **Descargar documentos:** Exporta los documentos generados por ChatGPT en formato `.docx`

2. **Crear estructura de carpetas:** Organiza tu proyecto siguiendo esta estructura:
   ```
   product_evaluation/
   ├── .llm/
   │   └── tasks/
   │       ├── create_inventory_from_sources.md
   │       ├── update_inventory.md
   │       └── update_inventory_from_web.md
   ├── source_docs/
   │   ├── doc1.md
   │   ├── doc2.md
   │   └── ...
   └── analytics/
       └── specifications.md
   ```

3. **Convertir a Markdown:** Transforma los archivos `.docx` a formato Markdown usando [word2md.com](https://word2md.com/)

4. **Crear inventario inicial:** Adapta y utiliza la tarea descrita en [create_inventory_from_sources](.augment/tasks/create_inventory_from_sources.md)

5. **Actualizar inventario (si es necesario):** Adapta y utiliza la tarea descrita en [update_inventory](.augment/tasks/update_inventory.md)

6. **Completar información faltante:** Utiliza búsquedas web para rellenar datos. Adapta y utiliza la tarea descrita en [update_inventory_from_web](.augment/tasks/update_inventory_from_web.md)

7. **Iterar:** Repite los pasos anteriores tantas veces como sea necesario hasta obtener un inventario completo

### Prompt de Ejemplo para Actualizar Inventario

```markdown
Based on the structure of the task `./augment/requests/update_inventory.md`,
the specifications of the product to evaluate at
`/home/levi/Documents/Outside_Life/Manuales/Evaluacion_Prod_Tecnicos/Aspiradoras/analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md`
and the contents of the source documents in the `source_docs/` directory

redact a new task to update the inventory table at `./analytics/inventory.md`
with information obtained from the web to verify and supplement existing data.
The task should include multiple iterations focusing on different aspects of
the inventory data, ensuring thorough verification and updates with proper citations.
```

### Cómo Adaptar las Tareas

Para adaptar las tareas predefinidas a tu producto específico, puedes utilizar la guía descrita en [adapt_tasks.md](.augment/tasks/adapt_tasks.md)

---

## 4. Generar Recomendaciones Finales

**Objetivo:** Producir conclusiones y recomendaciones basadas en todo el análisis realizado.

### Tipos de Recomendaciones Disponibles

| Tipo | Descripción | Tarea |
|------|-------------|-------|
| **Generales** | Recomendaciones para usuarios con presupuesto estándar | [generate_recommendations](.augment/tasks/generate_recommendations.md) |
| **Premium** | Recomendaciones para usuarios que buscan las mejores opciones sin restricción de precio | [generate_recommendations_premium](.augment/tasks/generate_recommendations_premium.md) |

> 💡 **Consejo:** Adapta cada tarea a tu producto y contexto específico antes de ejecutarla.

---

## Glosario de Términos

| Término | Definición |
|---------|------------|
| **LLM** | Large Language Model (Modelo de Lenguaje Grande). Sistema de IA que procesa y genera texto. |
| **Prompt** | Instrucción o pregunta que se le da a una LLM para obtener una respuesta. |
| **Markdown** | Formato de texto ligero para crear documentos estructurados, usando símbolos simples para dar formato. |
| **Iterar** | Repetir un proceso varias veces, refinando los resultados en cada repetición. |
| **Task** | Archivo que contiene instrucciones predefinidas para que la LLM ejecute una tarea específica. |
