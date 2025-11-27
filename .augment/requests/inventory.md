please review all the markdown files in the `source_docs` directory. 
Based on that review, create an inventory of robot vacuum models mentioned in those files.
The inventory should be saved at ./analytics/inventory.md

The inventory should be formatted as a markdown table with the following columns:
- Model Name
- Manufacturer
- Price (CLP)
- Suction Power (Pa)
- Navigation Technology
- Dustbin Capacity (l) 
- Battery Life (h)
- Water Tank Capacity (l)
- Cleaning Technology
- App & Smartphone Control
- Compatibility with Home Automation Systems
- Auto-Emptying Station
- Additional Features
- Brand Availability in Chile
- Brand Reputation
- Brush Roll Type
- Pros & Cons
- Known Issues
- Cost Effectiveness
- Automation Level
- User Reviews


Every field in the table should be populated with the information available in the source documents, and with a link to the source document and the specific section within the document where the information was found (use markdown links, with the format [1], [2], etc). 
If a piece of information is not available, the cell should be left empty for now. 


This task is expected that it requires multiple iterations to complete.
So: 

## Implementation Plan

1. Break down the task in multiple smaller sub-tasks, each focused on gathering specific pieces of information for the inventory table.
   1. Plan the first iteration to gather all the Model Names and Manufacturers from the source documents, including links to the source documents, in order to create the initial structure of the inventory table.
   2. Plan subsequent iterations to gather additional pieces of information (e.g., Price, Suction Power, Navigation Technology, etc.) and fill in the corresponding cells in the inventory table.
   3. Use as many iterations as needed to complete the inventory table with all the required information.
2. For each iteration, create as many hierarchical sub-tasks as needed to gather the targeted pieces of information.
   1. Review the source documents to gather the specific pieces of information targeted for that iteration.
   2. Update the inventory table with the newly gathered information, ensuring to include links to the source documents.
   3. Save the updated inventory table to ./analytics/inventory.md.

3. After completing all iterations, review the entire inventory table for completeness and accuracy.
4. Make any necessary adjustments or corrections to ensure the inventory table meets the specified requirements.

## Task Management
Before starting the implementation, use the Task Manager to create the main task and all the sub-tasks as per the implementation plan above.


## Utility
Use the directory at `.augment/reports/inventory/` and the initial empty file `notes.md` as you please, to aid in your analysis and documentation process
   1. The whole directory `.augment/reports/inventory/` is at your disposal to help you with your analysis and documentation process.
   2. Use it as you see fit, transversally across all subtasks.
   3. So you can create any additional files you need.
   4. In particular, the file `notes.md` (or any other file you create) can be used as a personal notepad to jot down any insights, questions, or ideas that arise during your analysis.
   5. You can use `notes.md` (or any other file you create) to keep track of important points that you want to remember or revisit later.
   6. You can also use `notes.md` (or any other file you create) to draft sections of the documentation files before finalizing them.
   7. You can also use `notes.md` (or any other file you create) to keep track of any TODOs or action items that need to be addressed before the documentation is considered complete.
   8. You can also use `notes.md` (or any other file you create) to brainstorm any additional documentation files that may be needed beyond those listed in the Documentation Deliverables section.
   9. You can also use `notes.md` (or any other file you create) to track any questions or uncertainties that arise during your analysis, which can be addressed in later subtasks.
   10. You can also use `notes.md` (or any other file you create) to jot down important insights, and references as you review the source files.


## Documentation Deliverables
1. The final inventory table saved at ./analytics/inventory.md, formatted as a markdown table with all the specified columns and populated with the information gathered from the source documents, including links to the source documents.

--------------

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