

# Generar la Especificación de Requerimientos sobre <Producto>
1. LLM => modo investigación:

Objetivo:
- Que la LLM descubra todas las dimensiones que son importante para <producto>
- Luego que describa cuáles serían los requisitos a cumplir en esas dimensiones para que <producto> cumpla con <escenario importante>

## Fase 1: Descubrimiento de criterios

Prompt 1 :
"Revisa cuáles son todas las características importantes que debo tomar ateción para escoger una <producto> para <x escenario importante>"
ej:
"Investiga qué características debo tomar ateción para escoger una aspiradora automática para un piso vinílico"

Iterar un par de veces de ser necesario

## Fase 2: Creación de Especificaciones
Prompt 2:

Objetivo:
- Obtener un marco de trabajo sobre la cual la LLM pueda partir, revisar internet y empezar a identificar posibles candidatos.

"Crea una especificación de requerimientos en formato markdown con todos los criterios comentados aquí, en consideración con el <escenario importante>"
(markdown es el formato de este mismo doc, y es el que mejor entienen las llm después de lenguajes de programación propiamente tal)

## Ejemplo:
Esta fase completa la hice con Claude
- https://claude.ai/share/6a68ad16-d9bf-44f8-9c1c-ee56f92e9e1f

# Capturar posibles candidatos

Objetivo:
- Que te ahorre la paja de acumular información desde internet:

Prompt:
"Based on the <documento de especificaciones> archive,  run a deep comprehensive evaluation of the <product> available in the chilean market. Report a tier table following the considerations indicated on the document."

Basado en la respuesta, iterar hartas veces, revisar info, chatear con la LLM para que acumule info respecto a lo que interese


## Ejemplo:
Esta fase completa la hice con ChatGPT v4 (ahora con el 5 debe resultar mejor)
- https://chatgpt.com/share/69288c69-bd1c-8011-aa3a-ffd5c0c5ee1b


# Inventariar

Objetivo: el siguiente prompt: 
```markdown
Based on the structure of the task `./augment/requests/update_inventory.md`, the specifications of the product to evaluate at `/home/levi/Documents/Outside_Life/Manuales/Evaluacion_Prod_Tecnicos/Aspiradoras/analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md` and the contents of the source documents in the `source_docs/` directory

redact a new task to update the inventory table at `./analytics/inventory.md` with information obtained from the web to verify and supplement existing data. The task should include multiple iterations focusing on different aspects of the inventory data, ensuring thorough verification and updates with proper citations.
- Resumir y organizar la info acumulada

Pasos:
1. Descargar documentos creados por chatgpt en formato docx
2. Crear una carpeta con una estructura similar a esta: 
   ```
   product_evaluation/
   ├── .llm/
   │   └── tasks/
   │       └── create_inventory_from_sources.md
   │       └── update_inventory.md
   │       └── update_inventory_from_web.md
   ├── source_docs/
   │   ├── doc1.md
   │   ├── doc2.md
   │   └── ...
   └── analytics/
       └── specifications.md
    ```
3. Convertirlos a markdown con https://word2md.com/
4. Inventariar: (adaptar y utilizar tarea descrita en [create_inventory_from_sources](.augment/tasks/create_inventory_from_sources.md))
5. Si es necesario, Actualizar inventario: (adaptar y utilizar tarea descrita en [update_inventory](.augment/tasks/update_inventory.md))
6. Rellenar información faltante con búsquedas web: (adaptar y utilizar tarea descrita en [update_inventory_from_web](.augment/tasks/update_inventory_from_web.md))
7. Iterar tantas veces como sea necesario

## Adaptar Tasks: 
Para adaptar las tasks, puedes utilizar la tarea descrita en [.augment/tasks/adapt_tasks.md](.augment/tasks/adapt_tasks.md)


# Generar Recomendaciones Finales

1. Recomendaciones Generales (adaptar y utilizar tarea descrita en [generate_recommendations](.augment/tasks/generate_recommendations.md))
2. Recomendaciones Premium (adaptar y utilizar tarea descrita en [generate_recommendations_premium](.augment/tasks/generate_recommendations_premium.md))
