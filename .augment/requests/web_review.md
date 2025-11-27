Based on the task `./augment/requests/update_inventory.md`, redact a new task to update the inventory table at `./analytics/inventory.md` with information obtained from the web to verify and supplement existing data. The task should include multiple iterations focusing on different aspects of the inventory data, ensuring thorough verification and updates with proper citations.

As starting point use the links in the source documents located in the `source_docs/` directory. The final output should be a complete and accurate markdown table with the inventory updated as much as possible using the web sources. Ensure that all data points have proper citations and that any new information discovered is included in the inventory. If a piece of information is not available, the cell should be left empty for now.

## Deliverable

Task detailed description for updating the robot vacuum inventory table, using web sources for verification and supplementation, at `./augment/tasks/update_inventory_from_web.md`.

## Reference

For reference, the existing task to update the inventory table based on the source documents is located at `./augment/requests/update_inventory.md`.


-------------------------------------


Create a new task file at `./augment/tasks/update_inventory_from_web.md` that provides detailed instructions for updating the robot vacuum inventory table located at `./analytics/inventory.md` using web-based research.

## Context
- Reference the existing task at `./augment/requests/update_inventory.md` to understand the current inventory update process
- Use links found in source documents within the `source_docs/` directory as starting points for web research
- The goal of the new task is to verify existing inventory data and supplement it with additional information from authoritative web sources

## Task Requirements

The new task file should specify:

1. **Iterative Research Approach**: Define multiple research iterations, each focusing on specific aspects of the inventory data (e.g., technical specifications, pricing, availability, features, user reviews, etc.)

2. **Data Verification**: Instructions for cross-referencing existing inventory data against web sources to confirm accuracy

3. **Data Supplementation**: Guidelines for identifying and adding missing information to complete the inventory table

4. **Citation Standards**: Clear requirements that every data point must include proper citations to web sources (URLs, access dates, source names)

5. **Data Handling Rules**:
   - Leave cells empty if information cannot be verified from reliable web sources
   - Do not fabricate or assume data
   - Prioritize manufacturer websites and reputable retailers for technical specifications
   - Use review sites and forums for user feedback and known issues (reddit, product review sites, etc, with proper citations)

6. **Quality Criteria**: Define what constitutes a "complete and accurate" inventory entry

7. **Output Format**: Ensure the final result maintains the markdown table structure at `./analytics/inventory.md`

## Deliverable
A comprehensive task description file at `./augment/tasks/update_inventory_from_web.md` that can be executed to systematically update the robot vacuum inventory using web research with proper documentation and citations.