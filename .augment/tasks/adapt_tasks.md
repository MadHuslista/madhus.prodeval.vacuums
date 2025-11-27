# Single Task Template Adaptation Workflow

## Objective
Adapt a specific existing task template from `.augment/tasks/` to a new product evaluation scenario. This workflow guides the systematic adaptation of ONE selected template while maintaining structural integrity, accuracy, and full traceability to source materials.

---

## ⚠️ INPUT CONFIGURATION (User Must Complete Before Execution)

### 1. Template Selection
**Task Template to Adapt:**
```
TEMPLATE_PATH: .augment/tasks/[PLACEHOLDER: Enter task filename, e.g., create_inventory_from_sources.md]
```

**Available Templates:**
- `create_inventory_from_sources.md` - For creating new product inventories
- `update_inventory.md` - For updating existing inventories
- `generate_recommendations.md` - For tier-based recommendation reports
- `generate_recommendations_premium.md` - For premium segment analysis
- `update_inventory_from_web.md` - For web-supplemented inventory updates

### 2. Specification Document
**Product Evaluation Guide:**
```
SPECIFICATION_DOC: analytics/[PLACEHOLDER: Enter specification document filename]
```

**Required Content in Specification Document:**
- Product category and technical parameters
- Evaluation criteria and metrics
- User requirements (critical and secondary)
- Market context (geography, pricing, availability)

### 3. Source Documents
**Reference Materials from `source_docs/`:**
```
SOURCE_DOCS:
  - source_docs/[PLACEHOLDER: Document 1 filename]
  - source_docs/[PLACEHOLDER: Document 2 filename]
  - source_docs/[PLACEHOLDER: Document 3 filename]
  - [Add more as needed]
```

### 4. Output Configuration
**Adapted Task Output:**
```
OUTPUT_PATH: .augment/tasks/[PLACEHOLDER: New task filename for adapted version]
```

---

## Adaptation Process

### Phase 1: Template Structure Analysis

#### Iteration 1: Analyze Selected Task Template
**Goal**: Fully understand the structure and content of the selected template

**Sub-tasks:**
- **1.1**: Read and parse the template at `TEMPLATE_PATH`:
  - Identify all major sections and their purposes
  - Document the hierarchy of phases/iterations/sub-tasks
  - List all product-specific terminology used
  - Note all hardcoded paths, filenames, and references

- **1.2**: Create template structure map:
  ```markdown
  ## Template Structure Map

  **Template**: [TEMPLATE_PATH]

  ### Sections Identified
  | Section | Purpose | Adaptation Required |
  |---------|---------|---------------------|
  | Objective | [Purpose] | Yes/No |
  | Input Sources | [Purpose] | Yes/No |
  | ... | ... | ... |

  ### Product-Specific Elements
  - [Element 1]: Location in template
  - [Element 2]: Location in template
  ```

- **1.3**: Identify adaptation scope:
  - Which sections require full rewrite?
  - Which sections need terminology replacement only?
  - Which sections can remain unchanged?
  - What new sections might be needed?

- **1.4**: Save analysis to working directory

**Verification Checkpoint 1:**
- [ ] Template fully read and understood
- [ ] Structure map created
- [ ] All product-specific elements identified
- [ ] Adaptation scope defined

---

### Phase 2: Specification Extraction

#### Iteration 2: Extract Product Context from Specification Document
**Goal**: Gather all relevant information from the specification document

**Sub-tasks:**
- **2.1**: Parse `SPECIFICATION_DOC` to extract:
  - **Product Category**: Name, subcategories, variants
  - **Technical Parameters**: Key specifications and metrics
  - **Evaluation Criteria**: How products should be assessed
  - **User Requirements**: Critical vs. secondary needs
  - **Market Context**: Geography, currency, retailers, availability

- **2.2**: Create terminology extraction table:
  ```markdown
  ## Extracted Terminology

  ### Product Terms
  | Term | Definition | Usage Context |
  |------|------------|---------------|
  | [Term 1] | [Definition] | [Where to use] |

  ### Technical Specifications
  | Specification | Units | Typical Range | Evaluation Threshold |
  |---------------|-------|---------------|---------------------|
  | [Spec 1] | [Unit] | [Range] | [Threshold] |

  ### Evaluation Criteria
  | Criterion | Weight/Priority | Description |
  |-----------|-----------------|-------------|
  | [Criterion 1] | [Priority] | [Description] |
  ```

- **2.3**: Document user requirements:
  - Critical requirements (must-have)
  - Secondary requirements (nice-to-have)
  - Constraints (budget, availability, etc.)

- **2.4**: Save extraction results to working directory

**Verification Checkpoint 2:**
- [ ] All product terminology extracted
- [ ] Technical specifications documented
- [ ] Evaluation criteria identified
- [ ] User requirements cataloged

---


### Phase 4: Source Document Integration

#### Iteration 4: Integrate Source References and Citations
**Goal**: Establish proper citation structure using the specified source documents

**Sub-tasks:**
- **4.1**: Create citation index from `SOURCE_DOCS`:
  ```markdown
  ## Citation Reference Index

  ### Document Citations
  [1] source_docs/[Document_1.md] - [Brief description of content]
  [2] source_docs/[Document_2.md] - [Brief description of content]
  [3] source_docs/[Document_3.md] - [Brief description of content]
  ...

  ### Web Citations (if applicable)
  [W1] [URL] - [Source description]
  [W2] [URL] - [Source description]
  ...
  ```

- **4.2**: Map source content to template sections:
  | Template Section | Relevant Source(s) | Citation(s) |
  |------------------|-------------------|-------------|
  | Technical Specs | [Document name] | [1], [2] |
  | Pricing Data | [Document name] | [3] |
  | User Reviews | [Document name] | [4] |

- **4.3**: Update citation requirements in adapted template:
  - Replace original citation references with new identifiers
  - Specify citation format to use
  - Define when to use inline vs. reference citations

- **4.4**: Document citation guidelines for task execution:
  - Format for inline citations
  - Handling multiple citations
  - Resolving conflicting sources
  - Citation verification requirements

**Verification Checkpoint 4:**
- [ ] All source documents have citation identifiers
- [ ] Source-to-section mapping complete
- [ ] Citation format specified in adapted template
- [ ] No references to non-existent sources

---

### Phase 5: Terminology Consistency

#### Iteration 5: Apply Terminology Changes Throughout Template
**Goal**: Systematically replace all product-specific terminology

**Sub-tasks:**
- **5.1**: Update Objective section:
  - Replace product category references
  - Adjust market/geographic context
  - Modify evaluation purpose statement
  - Update target audience description

- **5.2**: Update Input Sources section:
  - Replace specification document reference
  - Update source document paths
  - Modify citation format references
  - Adjust web source references

- **5.3**: Update User Requirements section:
  - Adapt critical requirements to new product
  - Modify secondary requirements
  - Update budget/price constraints
  - Adjust availability requirements

- **5.4**: Update Evaluation/Analysis sections:
  - Replace all technical specifications
  - Update tier classification criteria
  - Modify filtering/prioritization logic
  - Adjust ranking methodology

- **5.5**: Update Deliverable sections:
  - Modify output file paths
  - Update required section names
  - Adjust table column definitions
  - Revise format requirements

**Verification Checkpoint 5:**
- [ ] Objective section fully updated
- [ ] All input sources correctly referenced
- [ ] User requirements adapted
- [ ] Evaluation criteria use new terminology
- [ ] Deliverables reference correct paths

---

### Phase 6: Validation Against Specifications

#### Iteration 6: Validate Adapted Task Against Product Specifications
**Goal**: Ensure the adapted task accurately reflects the new product context

**Sub-tasks:**
- **6.1**: Cross-reference with specification document:
  - All evaluation criteria from spec are included
  - Technical parameters match spec definitions
  - User requirements are correctly represented
  - Market context is accurately reflected

- **6.2**: Verify structural integrity:
  - All sections reference each other correctly
  - No broken internal links
  - Consistent numbering/hierarchy
  - Proper markdown formatting

- **6.3**: Terminology audit:
  - Search for remaining original product terms
  - Verify consistent use of new terminology
  - Check for mixed terminology within sections
  - Validate technical accuracy

- **6.4**: Citation validation:
  - All citations reference real documents from SOURCE_DOCS
  - Citation numbers are sequential
  - No duplicate citation identifiers
  - Citation format is consistent throughout

- **6.5**: Completeness verification:
  - All original template sections accounted for
  - New required sections added
  - Irrelevant sections removed with justification
  - No placeholder or TODO content remains

**Verification Checkpoint 6:**
- [ ] Adapted task matches specification document
- [ ] Structural integrity maintained
- [ ] All terminology consistently updated
- [ ] All citations valid
- [ ] Task is complete with no placeholders

---

### Phase 7: Final Review and Quality Check

#### Iteration 7: Final Quality Assurance and Documentation
**Goal**: Ensure the adapted task is ready for execution and fully documented

**Sub-tasks:**
- **7.1**: Full read-through:
  - Read entire adapted task from start to finish
  - Verify logical flow and coherence
  - Check that all instructions are clear and actionable
  - Confirm success criteria are measurable

- **7.2**: Create adaptation changelog:
  ```markdown
  ## Adaptation Changelog

  **Source Template**: [TEMPLATE_PATH]
  **Specification Document**: [SPECIFICATION_DOC]
  **Adapted Task**: [OUTPUT_PATH]
  **Date Adapted**: [Date]

  ### Major Changes
  | Section | Change Type | Description |
  |---------|-------------|-------------|
  | [Section] | [Modified/Added/Removed] | [Description] |

  ### Terminology Replacements
  | Count | Original Term | New Term |
  |-------|---------------|----------|
  | [N] | [Original] | [New] |

  ### Citation Structure
  - Total citations: [N]
  - Document citations: [N]
  - Web citations: [N]

  ### Sections Added
  - [Section name]: [Purpose]

  ### Sections Removed
  - [Section name]: [Justification]
  ```

- **7.3**: Update working directory specifications:
  - Set appropriate working directory path for new product
  - List relevant working files to create
  - Adjust documentation requirements
  - Specify changelog/tracking format

- **7.4**: Finalize success criteria:
  - Ensure all criteria are achievable
  - Add product-specific success metrics
  - Remove inapplicable criteria
  - Define quality thresholds

- **7.5**: Save adapted task to `OUTPUT_PATH`:
  - Final formatting check
  - Verify file saves correctly
  - Confirm no syntax errors in markdown

**Verification Checkpoint 7:**
- [ ] Full read-through completed
- [ ] Changelog is complete and accurate
- [ ] Working directory structure defined
- [ ] Success criteria are appropriate
- [ ] Adapted task saved to OUTPUT_PATH

---

## Working Directory Structure

Use `.augment/reports/adaptation/` as the working directory for this adaptation:

```
.augment/reports/adaptation/
├── notes.md                      # Ongoing observations and decisions
├── template-analysis.md          # Phase 1 structure map
├── specification-extraction.md   # Phase 2 extracted content
├── terminology-mapping.md        # Phase 3 complete mapping table
├── citation-index.md             # Phase 4 citation reference list
├── consistency-check.md          # Phase 5 terminology audit results
├── validation-log.md             # Phase 6 validation results
├── adaptation-changelog.md       # Phase 7 final changelog
└── drafts/                       # Work-in-progress versions
    └── [task-name]-draft-v1.md
```

---

## Deliverable

**Final Output**: Adapted task file at `OUTPUT_PATH` containing:
- Fully adapted task template for the new product evaluation scenario
- All terminology updated using the mapping from Phase 3
- Complete citation structure referencing SOURCE_DOCS
- Proper iteration phases with product-specific sub-tasks
- Working directory specifications for task execution
- Success criteria appropriate to the new product context
- Full traceability documented in adaptation changelog

---

## Success Criteria

✅ Template structure preserved from `TEMPLATE_PATH`
✅ All content adapted to match `SPECIFICATION_DOC`
✅ All citations reference documents from `SOURCE_DOCS`
✅ No original product terminology remains
✅ All 7 verification checkpoints passed
✅ Terminology mapping table complete
✅ Adaptation changelog documents all changes
✅ Adapted task is executable as written
✅ Working directory contains complete documentation

---

## Quick Reference: Adaptation Checklist

### Before Starting
- [ ] `TEMPLATE_PATH` placeholder filled in
- [ ] `SPECIFICATION_DOC` placeholder filled in
- [ ] `SOURCE_DOCS` list completed
- [ ] `OUTPUT_PATH` defined
- [ ] Working directory created

### During Adaptation (Per Phase)
- [ ] Phase 1: Template structure analyzed
- [ ] Phase 2: Specification content extracted
- [ ] Phase 3: Parameter mappings created
- [ ] Phase 4: Citations integrated
- [ ] Phase 5: Terminology applied consistently
- [ ] Phase 6: Validation against specs complete
- [ ] Phase 7: Final review and changelog done

### After Completion
- [ ] Adapted task saved to OUTPUT_PATH
- [ ] No original product references remain
- [ ] All citations point to real sources
- [ ] Changelog documents all changes
- [ ] Task is ready for execution

---

**Version**: 1.0
**Created**: November 2025
**Purpose**: Focused workflow for adapting a single task template to a new product evaluation context
**Related**: See `adapt_task_full.md` for general multi-template adaptation workflow
