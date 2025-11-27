
# Robot Vacuum Inventory Creation Task

## Objective
Review all markdown files in the `source_docs/` directory and create a comprehensive inventory of all robot vacuum models mentioned. The final inventory must be saved to `./analytics/inventory.md`.

## Inventory Table Specifications

### Required Columns
Create a markdown table with the following columns (in this exact order):

1. **Model Name** - Full product name/model number
2. **Manufacturer** - Brand/company name
3. **Price (CLP)** - Price in Chilean Pesos, include price range if applicable
4. **Suction Power (Pa)** - Suction power in Pascals
5. **Navigation Technology** - Type of navigation system (e.g., LiDAR, vSLAM, gyroscope)
6. **Dustbin Capacity (L)** - Dust container volume in liters
7. **Battery Life (h)** - Runtime in hours or minutes (convert to hours)
8. **Water Tank Capacity (L)** - Water reservoir volume in liters
9. **Cleaning Technology** - Mopping system type (e.g., rotating mops, vibrating pad, static cloth)
10. **App & Smartphone Control** - App name and key features
11. **Compatibility with Home Automation Systems** - Smart home integrations (Alexa, Google Home, etc.)
12. **Auto-Emptying Station** - Whether included, station features
13. **Additional Features** - Notable extras (obstacle avoidance, carpet detection, etc.)
14. **Brand Availability in Chile** - Local availability status and retailers
15. **Brand Reputation** - Brand standing and support quality
16. **Brush Roll Type** - Main brush composition (rubber, bristles, hybrid)
17. **Pros & Cons** - Key advantages and disadvantages
18. **Known Issues** - Reported problems or reliability concerns
19. **Cost Effectiveness** - Value assessment relative to features
20. **Automation Level** - Degree of hands-free operation
21. **User Reviews** - Summary of user feedback and ratings

### Data Population Rules
- **Source Citations**: Every data point MUST include inline markdown reference links using the format `[1]`, `[2]`, etc., pointing to the specific source document and section
- **Missing Data**: Leave cells empty (no placeholder text) if information is not found in source documents
- **Multiple Values**: If a field has multiple values or ranges, include all with separate citations
- **Consistency**: Use consistent units and formatting across all rows

## Implementation Strategy

### Phase 1: Task Planning & Setup
**Before any implementation work**, use the Task Management tools to:
1. Create a parent task: "Create Robot Vacuum Inventory from Source Documents"
2. Create hierarchical sub-tasks following the iteration plan below
3. Mark tasks as IN_PROGRESS/COMPLETE as you work through them

### Phase 2: Iterative Data Collection

#### Iteration 1: Foundation (Model Identification)
**Goal**: Establish the inventory structure
- **Sub-task 1.1**: Review all 7 markdown files in `source_docs/` to identify every unique robot vacuum model mentioned
- **Sub-task 1.2**: Extract Model Name and Manufacturer for each model
- **Sub-task 1.3**: Create initial inventory table structure with Model Name and Manufacturer columns populated (with source citations)
- **Sub-task 1.4**: Save initial table to `./analytics/inventory.md`

#### Iteration 2: Core Specifications
**Goal**: Add technical specifications
- **Sub-task 2.1**: Gather Price (CLP) data with citations
- **Sub-task 2.2**: Gather Suction Power (Pa) data with citations
- **Sub-task 2.3**: Gather Navigation Technology data with citations
- **Sub-task 2.4**: Gather Battery Life data with citations
- **Sub-task 2.5**: Update inventory table and save

#### Iteration 3: Physical Specifications
**Goal**: Add capacity and hardware details
- **Sub-task 3.1**: Gather Dustbin Capacity data with citations
- **Sub-task 3.2**: Gather Water Tank Capacity data with citations
- **Sub-task 3.3**: Gather Brush Roll Type data with citations
- **Sub-task 3.4**: Update inventory table and save

#### Iteration 4: Cleaning Features
**Goal**: Add cleaning-related features
- **Sub-task 4.1**: Gather Cleaning Technology data with citations
- **Sub-task 4.2**: Gather Auto-Emptying Station data with citations
- **Sub-task 4.3**: Gather Additional Features data with citations
- **Sub-task 4.4**: Update inventory table and save

#### Iteration 5: Smart Features
**Goal**: Add connectivity and automation
- **Sub-task 5.1**: Gather App & Smartphone Control data with citations
- **Sub-task 5.2**: Gather Home Automation Compatibility data with citations
- **Sub-task 5.3**: Gather Automation Level data with citations
- **Sub-task 5.4**: Update inventory table and save

#### Iteration 6: Market & Evaluation Data
**Goal**: Add market-specific and evaluative information
- **Sub-task 6.1**: Gather Brand Availability in Chile data with citations
- **Sub-task 6.2**: Gather Brand Reputation data with citations
- **Sub-task 6.3**: Gather Cost Effectiveness data with citations
- **Sub-task 6.4**: Update inventory table and save

#### Iteration 7: User Feedback & Issues
**Goal**: Add user experience data
- **Sub-task 7.1**: Gather Pros & Cons data with citations
- **Sub-task 7.2**: Gather Known Issues data with citations
- **Sub-task 7.3**: Gather User Reviews data with citations
- **Sub-task 7.4**: Update inventory table and save

#### Iteration 8: Final Review & Quality Assurance
**Goal**: Ensure completeness and accuracy
- **Sub-task 8.1**: Review entire inventory for missing citations
- **Sub-task 8.2**: Verify all data points against source documents
- **Sub-task 8.3**: Check for duplicate models or inconsistent naming
- **Sub-task 8.4**: Validate markdown table formatting
- **Sub-task 8.5**: Perform final save and mark parent task as COMPLETE

### Phase 3: Working Directory Usage

#### Directory Structure
Use `.augment/reports/inventory/` as your working directory:
- **Create `notes.md`** for ongoing observations, questions, and insights
- **Create additional files** as needed (e.g., `model-list.md`, `data-gaps.md`, `citation-index.md`)
- **Use freely** across all iterations and sub-tasks

#### Suggested Uses for Working Files
- Track which models appear in which source documents
- Note data inconsistencies or conflicts between sources
- Draft complex table cells before adding to main inventory
- Maintain a running list of TODOs and data gaps
- Document decisions about data interpretation or categorization
- Keep a citation reference guide for quick lookup
- Log any questions or ambiguities for later resolution

## Deliverable
**Final Output**: `./analytics/inventory.md` containing:
- A complete markdown table with all 21 columns
- One row per unique robot vacuum model
- All available data populated with proper source citations
- Empty cells for unavailable data (no placeholders)
- Clean, readable markdown formatting

## Success Criteria
✅ All models from source documents are included  
✅ Every data point has a source citation  
✅ Table is properly formatted and readable  
✅ All task management items are marked COMPLETE  
✅ Working directory contains documentation of the process