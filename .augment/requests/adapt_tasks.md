based on the tasks at `.augment/tasks/`, redact a new task called `adapt_tasks.md` that allow to take any of the existing tasks as template and adapt it to a new context or product evaluation scenario, based on the specifications provided in a given document (equivalent to `analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md`), and the contents of the source documents in the `source_docs/` . 

The task should include multiple iterations focusing on different aspects of the inventory data, ensuring thorough verification and updates with proper citations.

--------------------------------------------


Create a new task file at `.augment/tasks/adapt_tasks.md` that defines a reusable workflow for adapting existing task templates to new product evaluation scenarios.

**Objective:**
The task should provide a systematic process for taking any existing task from `.augment/tasks/` as a template and customizing it for a different product or evaluation context.

**Key Requirements:**

1. **Input Specifications:**
   - Accept a specification document (similar in structure to `analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md`) that defines the new product evaluation scenario
   - Reference source documents from the `source_docs/` directory for contextual information

2. **Adaptation Process:**
   - Define clear steps for selecting an appropriate task template from `.augment/tasks/`
   - Specify how to identify and replace product-specific terminology, criteria, and evaluation parameters
   - Outline how to maintain the structural integrity of the original task while adapting content

3. **Iterative Verification:**
   - Include multiple iteration phases, each focusing on different aspects:
     - Product specifications and technical parameters
     - Evaluation criteria and metrics
     - Source document references and citations
     - Terminology consistency
   - For each iteration, specify verification checkpoints to ensure accuracy and completeness

4. **Citation and Documentation:**
   - Establish guidelines for properly citing source documents
   - Ensure all adapted content maintains traceability to original sources
   - Define format for documenting changes made during adaptation

**Deliverable:**
A comprehensive task template that can be followed to systematically adapt any existing evaluation task to a new product context while maintaining quality, accuracy, and proper documentation.

=================================================

based on the tasks at `.augment/tasks/`, redact a new task called `adapt_tasks.md` that allow to SELECT a single task from any of the existing tasks as template and adapt it to a new context or product evaluation scenario, based on the specifications provided in a given document (equivalent to `analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md`), and the contents of the source documents in the `source_docs/` . 

The task should include multiple iterations focusing on different aspects of the inventory data, ensuring thorough verification and updates with proper citations.

This task should be able to take the task template indicated by the user as input, and adapt it to the new context, based on the specifications provided in the given document, and the contents of the source documents in the `source_docs/` directory.


---------------------------------------------

Create a new task file at `.augment/tasks/adapt_tasks.md` that provides a streamlined workflow for adapting a single existing task template to a new product evaluation context.

**Objective:**
The task should enable the user to selecting ONE specific task template from `.augment/tasks/` (e.g., `create_inventory_from_sources.md`, `generate_recommendations.md`, `update_inventory.md`) by updating the corresponding placeholders and from there systematically adapting it to a different product or evaluation scenario.

**Key Requirements:**

1. **Input Specifications:**
   - **Template Selection**: User explicitly specifies which task template from `.augment/tasks/` to use as the base. For that purpose the `adapt_tasks.md` should have a placeholder at the beginning of the task for the user to indicate the task template to be adapted.
   - **Specification Document**: Accept a guide document (structured like `analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md`) that defines the new product evaluation context, including:
     - Product category and technical parameters
     - Evaluation criteria and metrics
     - User requirements (critical and secondary)
     - Market context (geography, pricing, availability)
     - For that purpose the `adapt_tasks.md` should have a placeholder at the beginning of the task for the user to indicate the specification document to be used as input.
   - **Source Documents**: Reference materials from `source_docs/` directory containing product data, comparisons, and reviews. For that purpose the `adapt_tasks.md` should have a placeholder at the beginning of the task for the user to indicate the source documents to be used as input.

2. **Adaptation Workflow:**
   - Define the same 7 iteration phases as the full version, but focused on adapting the selected task template:
     - **Phase 1**: Analyze the selected task template structure and content
     - **Phase 2**: Extract relevant product-specific terminology and criteria from the specification document
     - **Phase 3**: Map existing evaluation parameters to the new product context
     - **Phase 4**: Integrate source document references into the adapted task
     - **Phase 5**: Ensure consistency in terminology and evaluation metrics
     - **Phase 6**: Validate the adapted task against the new product specifications
     - **Phase 7**: Final review and quality check of the adapted task

3. **Citation and Documentation:**
   - Establish guidelines for mapping new source documents to citation identifiers
   - Ensure all adapted content maintains proper citations to source materials
   - Create a terminology mapping table (old term → new term)
   - Document all changes in an adaptation changelog

4. **Deliverable:**
   - A fully adapted task file ready to execute in the new product context
   - All product-specific terminology updated
   - Complete citation structure referencing actual source documents
   - Working directory specifications for the adapted task
   - Success criteria appropriate to the new scenario

**Differences from `adapt_task_full.md`:**
This should be a equally comprehensive and detailed task as `adapt_task_full.md`, but it should be focused on adapting a single task template, instead of providing a general workflow for adapting all the tasks at once.