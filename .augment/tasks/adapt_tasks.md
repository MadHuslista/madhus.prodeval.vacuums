# Task Template Adaptation Workflow

## Objective
Systematically adapt any existing task template from `.augment/tasks/` to a new product evaluation scenario. This workflow ensures that adapted tasks maintain structural integrity, accuracy, proper documentation, and full traceability to source materials.

---

## Input Requirements

### 1. Specification Document
A specification document (similar in structure to `analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md`) that defines:
- **Product Category**: The type of product being evaluated
- **Target Market**: Geographic and demographic considerations
- **User Requirements**: Critical and secondary requirements for evaluation
- **Evaluation Criteria**: Specific metrics and parameters for assessment
- **Budget/Price Range**: Applicable price constraints
- **Use Case Context**: Intended usage scenarios

### 2. Source Documents
Reference materials from the `source_docs/` directory containing:
- Technical specifications and comparisons
- Market analysis and availability data
- User reviews and feedback compilations
- Decision frameworks and evaluation methodologies

### 3. Template Selection
Identify the most appropriate existing task template from `.augment/tasks/`:
- `create_inventory_from_sources.md` - For creating new product inventories
- `update_inventory.md` - For updating existing inventories
- `generate_recommendations.md` - For tier-based recommendation reports
- `generate_recommendations_premium.md` - For premium segment analysis
- `update_inventory_from_web.md` - For web-supplemented inventory updates

---

## Adaptation Process

### Phase 1: Analysis & Planning

#### Iteration 1: Context Analysis
**Goal**: Understand the new evaluation scenario completely

**Sub-tasks:**
- **1.1**: Review the specification document to identify:
  - Product category and subcategories
  - Primary evaluation focus areas
  - Critical requirements vs. nice-to-have features
  - Market-specific constraints (geography, currency, availability)

- **1.2**: Catalog all source documents relevant to the new scenario:
  - Document name and location
  - Key content areas covered
  - Unique data points available
  - Citation identifiers to use

- **1.3**: Select the most appropriate template from `.augment/tasks/`:
  - Match template purpose to task objective
  - Identify template sections that apply directly
  - Note sections requiring significant modification
  - Document sections to add or remove

- **1.4**: Create adaptation plan in working directory:
  - List all terminology changes needed
  - Map old parameters to new equivalents
  - Identify new criteria not in original template
  - Document structural changes required

**Verification Checkpoint 1:**
- [ ] Specification document fully analyzed
- [ ] All source documents cataloged with citation keys
- [ ] Template selected with clear justification
- [ ] Adaptation plan documented

---

### Phase 2: Terminology & Parameter Adaptation

#### Iteration 2: Product-Specific Terminology
**Goal**: Replace all product-specific terms and nomenclature

**Sub-tasks:**
- **2.1**: Create terminology mapping table:
  | Original Term | New Term | Context/Notes |
  |---------------|----------|---------------|
  | [Original product] | [New product] | Product category name |
  | [Original specs] | [New specs] | Technical parameters |
  | [Original metrics] | [New metrics] | Evaluation criteria |

- **2.2**: Update Objective section:
  - Replace product category references
  - Adjust market/geographic context
  - Modify evaluation purpose statement

- **2.3**: Update Input Sources section:
  - List new source documents with paths
  - Update citation format references
  - Adjust web source references if applicable

- **2.4**: Update User Requirements section:
  - Adapt critical requirements to new product
  - Modify secondary requirements accordingly
  - Ensure all requirement categories are relevant

**Verification Checkpoint 2:**
- [ ] All product names replaced consistently
- [ ] Technical terminology updated throughout
- [ ] Market references corrected
- [ ] No orphaned references to original product

---

#### Iteration 3: Evaluation Criteria Adaptation
**Goal**: Customize evaluation parameters and metrics

**Sub-tasks:**
- **3.1**: Review and adapt tier classification criteria:
  - Identify which original criteria apply
  - Define new product-specific criteria
  - Establish scoring weights for new scenario
  - Document tier boundary definitions

- **3.2**: Update evaluation methodology:
  - Adjust filtering criteria (price, availability, etc.)
  - Modify prioritization factors
  - Update ranking methodology
  - Adapt per-model analysis requirements

- **3.3**: Revise inventory columns (if applicable):
  - Keep universally applicable columns
  - Add product-specific specification columns
  - Remove irrelevant columns
  - Adjust column order for logical flow

- **3.4**: Update technical specifications:
  - Adapt power/performance metrics
  - Modify capacity/dimension requirements
  - Adjust technology/feature categories
  - Update compatibility requirements

**Verification Checkpoint 3:**
- [ ] All evaluation criteria relevant to new product
- [ ] Metrics and thresholds are product-appropriate
- [ ] No inherited criteria that don't apply
- [ ] Scoring methodology documented and consistent

---

### Phase 3: Source Integration & Citation

#### Iteration 4: Source Document References
**Goal**: Establish proper citation structure for new sources

**Sub-tasks:**
- **4.1**: Create citation index:
  ```markdown
  ## Citation Reference Index

  ### Document Citations
  [1] source_docs/Document_Name_1.md - Brief description
  [2] source_docs/Document_Name_2.md - Brief description
  ...

  ### Web Citations (if applicable)
  [W1] URL - Source description
  [W2] URL - Source description
  ...
  ```

- **4.2**: Update citation requirements section:
  - Specify citation format to use
  - List required citation types
  - Define inline vs. reference citation rules

- **4.3**: Map source content to evaluation areas:
  - Which sources cover specifications?
  - Which sources have pricing data?
  - Which sources contain user reviews?
  - Which sources address market availability?

- **4.4**: Document citation guidelines:
  - Format for inline citations
  - When to use multiple citations
  - How to handle conflicting sources
  - Citation verification requirements

**Verification Checkpoint 4:**
- [ ] All source documents have citation identifiers
- [ ] Citation format is clearly specified
- [ ] Source-to-content mapping is complete
- [ ] No references to non-existent sources

---

#### Iteration 5: Content Adaptation
**Goal**: Ensure all content sections are properly adapted

**Sub-tasks:**
- **5.1**: Update deliverable specifications:
  - Modify output file path/name
  - Adjust required sections list
  - Update table column definitions
  - Revise format requirements

- **5.2**: Adapt iteration phases:
  - Ensure sub-tasks reference correct content
  - Update data collection categories
  - Modify verification steps
  - Adjust timing/sequencing if needed

- **5.3**: Update working directory specifications:
  - Set appropriate working directory path
  - List relevant working files to create
  - Adjust documentation requirements
  - Specify changelog/tracking format

- **5.4**: Review and update success criteria:
  - Ensure all criteria are achievable
  - Add product-specific success metrics
  - Remove inapplicable criteria
  - Define quality thresholds

**Verification Checkpoint 5:**
- [ ] All deliverable specs are product-appropriate
- [ ] Iteration phases are logically sequenced
- [ ] Working directory structure is defined
- [ ] Success criteria are measurable and relevant

---

### Phase 4: Verification & Finalization

#### Iteration 6: Structural Integrity Verification
**Goal**: Ensure adapted task maintains logical coherence

**Sub-tasks:**
- **6.1**: Cross-reference check:
  - All sections reference each other correctly
  - No broken internal links
  - Consistent numbering/hierarchy
  - Proper markdown formatting

- **6.2**: Terminology consistency audit:
  - Search for any remaining original product terms
  - Verify consistent use of new terminology
  - Check for mixed terminology within sections
  - Validate technical accuracy of terms

- **6.3**: Citation validation:
  - All citations reference real documents
  - Citation numbers are sequential
  - No duplicate citation identifiers
  - Citation format is consistent

- **6.4**: Completeness check:
  - All original template sections accounted for
  - New required sections added
  - Irrelevant sections removed with justification
  - No placeholder or TODO content remains

**Verification Checkpoint 6:**
- [ ] No structural inconsistencies found
- [ ] All terminology is consistent
- [ ] All citations are valid
- [ ] Task is complete and ready for use

---

#### Iteration 7: Documentation & Traceability
**Goal**: Document all changes for future reference

**Sub-tasks:**
- **7.1**: Create adaptation changelog:
  ```markdown
  ## Adaptation Changelog

  **Source Template**: [Original template name]
  **Target Scenario**: [New product/evaluation context]
  **Date Adapted**: [Date]

  ### Major Changes
  - [Change 1]: [Justification]
  - [Change 2]: [Justification]

  ### Terminology Mappings
  - [Original] → [New]

  ### Added Sections
  - [Section name]: [Purpose]

  ### Removed Sections
  - [Section name]: [Justification]
  ```

- **7.2**: Document source traceability:
  - Which sources informed which sections
  - Confidence level for each data area
  - Gaps in source coverage
  - Recommendations for additional sources

- **7.3**: Create usage notes:
  - Prerequisites for using this task
  - Expected timeline for completion
  - Common pitfalls to avoid
  - Tips for successful execution

- **7.4**: Final review and approval:
  - Read through entire adapted task
  - Verify it can be executed as written
  - Confirm all verification checkpoints are achievable
  - Approve for use or note needed revisions

**Verification Checkpoint 7:**
- [ ] Changelog is complete and accurate
- [ ] Source traceability is documented
- [ ] Usage notes provide sufficient guidance
- [ ] Adapted task is approved for use

---

## Working Directory Structure

Use `.augment/reports/adaptation/` as the working directory for this workflow:

```
.augment/reports/adaptation/
├── notes.md                    # Ongoing observations and decisions
├── terminology-mapping.md      # Complete terminology translation table
├── citation-index.md           # Full citation reference list
├── source-analysis.md          # Source document analysis notes
├── adaptation-changelog.md     # Record of all changes made
├── verification-log.md         # Checkpoint completion records
└── [scenario-name]/            # Scenario-specific subdirectory
    └── adapted-task.md         # Draft versions during adaptation
```

---

## Deliverable

**Final Output**: A new task file in `.augment/tasks/` containing:
- Fully adapted task template for new product/evaluation scenario
- All terminology updated to match new context
- Complete citation structure referencing actual source documents
- Proper iteration phases with relevant sub-tasks
- Working directory specifications
- Success criteria appropriate to the new scenario
- Complete traceability to original template and adaptation decisions

---

## Success Criteria

✅ All product-specific terminology correctly adapted
✅ All source documents properly referenced with citations
✅ Evaluation criteria relevant to new product category
✅ Structural integrity maintained from original template
✅ All verification checkpoints passed
✅ Adaptation changelog complete and accurate
✅ Adapted task is executable as written
✅ Working directory contains complete adaptation documentation

---

## Quick Reference: Adaptation Checklist

### Before Starting
- [ ] Specification document available and reviewed
- [ ] Source documents identified and accessible
- [ ] Template selected with clear rationale
- [ ] Working directory created

### During Adaptation
- [ ] Terminology mapping table maintained
- [ ] Each section reviewed and adapted
- [ ] Citations verified after each update
- [ ] Verification checkpoints completed

### After Completion
- [ ] Full read-through completed
- [ ] No original product references remain
- [ ] All citations point to real sources
- [ ] Changelog documents all changes
- [ ] Task is ready for execution

---

**Version**: 1.0
**Created**: November 2025
**Purpose**: Reusable workflow for systematic task template adaptation
