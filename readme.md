# Guía de Evaluación de Productos con LLMs

---

## Resumen del Proceso

| Etapa                  | Descripción                                       |
| ---------------------- | ------------------------------------------------- |
| **1. Especificación**  | Definir características y requisitos del producto |
| **2. Candidatos**      | Identificar productos disponibles en el mercado   |
| **3. Inventario**      | Organizar y consolidar la información recopilada  |
| **4. Recomendaciones** | Generar conclusiones finales                      |

---

## 1. Generar la Especificación de Requerimientos

**Objetivo:** Identificar características importantes del producto y requisitos para el caso de uso específico.

Usar la LLM en modo investigación para buscar información de manera profunda.

### Fase 1: Descubrimiento de Criterios

Identificar dimensiones relevantes para evaluar el producto.

**Prompt:**
```
"Revisa cuáles son todas las características importantes que debo tomar en
atención para escoger una <producto> para <escenario importante>"
```

**Ejemplo:**
```
"Investiga qué características debo tomar en atención para escoger una
aspiradora automática para un piso vinílico"
```

Iterar según sea necesario con preguntas de seguimiento.

### Fase 2: Creación de Especificaciones

Generar un documento estructurado como base para evaluar candidatos.

**Prompt:**
```
"Crea una especificación de requerimientos en formato markdown con todos
los criterios comentados aquí, en consideración con el <escenario importante>"
```

> Nota: (markdown es el formato de este mismo doc, y es el que mejor entienen las llm después de lenguajes de programación propiamente tal)

### Ejemplo

- Esta fase completa la hice con Claude [https://claude.ai/share/6a68ad16-d9bf-44f8-9c1c-ee56f92e9e1f](https://claude.ai/share/6a68ad16-d9bf-44f8-9c1c-ee56f92e9e1f)

---

## 2. Capturar Posibles Candidatos

**Objetivo:** Recopilar información sobre productos disponibles en el mercado.

**Prompt:**
```
"Based on the <documento de especificaciones> archive, run a deep comprehensive
evaluation of the <product> available in the chilean market. Report a tier table
following the considerations indicated on the document."
```

Basado en la respuesta, iterar hartas veces, revisar info, chatear con la LLM para que acumule info respecto a lo que interese

### Ejemplo

- Esta fase completa la hice con ChatGPT v4 (ahora con el 5 debe resultar mejor) [https://chatgpt.com/share/69288c69-bd1c-8011-aa3a-ffd5c0c5ee1b](https://chatgpt.com/share/69288c69-bd1c-8011-aa3a-ffd5c0c5ee1b)

---

## 3. Inventariar

**Objetivo:** Resumir y organizar la información en un formato estructurado.

### Pasos

1. **Descargar documentos:** Exportar documentos de ChatGPT en formato `.docx`

2. **Crear estructura de carpetas:**
   ```
   product_evaluation/
   ├── .llm/
   │   └── tasks/ # From this repo
   │       ├── adapt_tasks.md
   │       ├── generate_recommendations.md
   │       ├── generate_recommendations_premium.md
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

3. **Convertir a Markdown:** Usar [word2md.com](https://word2md.com/)

4. **Crear inventario inicial:** Adaptar y ejecutar [create_inventory_from_sources](.augment/tasks/create_inventory_from_sources.md)

5. **Actualizar inventario:** Ejecutar [update_inventory](.augment/tasks/update_inventory.md)

6. **Completar información faltante con búsquedas web:** Ejecutar [update_inventory_from_web](.augment/tasks/update_inventory_from_web.md)

7. **Iterar** como sea necesario (yo ejecuté 1 vez el `update_inventory` y 1 vez el `update_inventory_from_web`)

> Nota: Preferi dejar campos vacíos en el inventario si no encontraba info confiable, en vez de inventar datos. Este requisito está también embebido en las tasks


### Adaptar Tareas

Para adaptar las tareas a un nuevo contexto o producto, usar la tarea [adapt_tasks](.augment/tasks/adapt_tasks.md).

Ver [adapt_tasks.md](.augment/tasks/adapt_tasks.md)

### LLMs: 

En este caso utilicé el agente `AugmentCode` desde el plugin de Augment para Visual Studio Code (un editor de texto), pero también se puede ejecutar con cualquier otra LLM mediante subir/descargar los archivos correspondientes. 

Para las adaptaciones, recomiendo Claude. 
Para las inverstigaciones y recomendaciones, recomiendo ChatGPT  
(no sé eso sí qué tal DeepSeek/Grok - sólo no he probado esas LLMs jiji)


---

## 4. Generar Recomendaciones Finales

**Objetivo:** Producir conclusiones basadas en el análisis.

> La idea del presupuesto estándar es la el clásico "mejor en relación precio/calidad", con el límite de precio indicado. 

> La gracia del premium, es poder ver "que tanto mejores" son las que quedan fuera del presupuesto estándar, si es que valen la pena, y poder también considerarlas porque los precios encontrados por las LLMs son más que nada approximativos.

| Tipo          | Descripción               | Tarea                                                                                  |
| ------------- | ------------------------- | -------------------------------------------------------------------------------------- |
| **Generales** | Presupuesto estándar      | [generate_recommendations](.augment/tasks/generate_recommendations.md)                 |
| **Premium**   | Sin restricción de precio | [generate_recommendations_premium](.augment/tasks/generate_recommendations_premium.md) |

Adaptar cada tarea al producto y contexto específico usando [adapt_tasks](.augment/tasks/adapt_tasks.md).

