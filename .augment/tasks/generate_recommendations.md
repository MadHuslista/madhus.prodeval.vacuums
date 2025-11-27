

# Task: Create Comprehensive Robot Vacuum Recommendation Report for Chilean Market

## Objective
Analyze the robot vacuum inventory and source documents to create a tier-based recommendation report for the Chilean market, specifically tailored to vinyl floor cleaning with the user's requirements.

## Input Sources
1. **Evaluation Guide**: `analytics/Guía Completa_Robot_Aspirador_para_Pisos_Vinílicos.md` - Use the tier classification criteria and evaluation methodology from this guide
2. **Robot Vacuum Inventory**: `analytics/inventory.md` - Contains 38 models with complete specifications, pricing, and citations
3. **Source Documents**: `source_docs/` directory - Contains detailed evaluations and comparisons
4. **Web Sources**: `./analytics/inventory.md` - Contains web sources for verification and supplementation

## User Requirements

### Critical Requirements (Must Have)
- **Price Range**: Maximum budget of $700,000 CLP (if above, it's discouraged)
- **Floor Type**: Must be safe and effective for vinyl floors (primary requirement)
- **Coverage Area**: 80m² apartment
- **Battery Life**: Minimum 90 minutes continuous operation to cover entire area
- **Mopping System**: Reliable mopping with adjustable water flow and washable mop pads that won't damage vinyl
- **Automation Level**: High automation with minimal supervision - automatic dirt disposal and smart mapping preferred
- **Smart Home Integration**: Must be compatible with Alexa, Google Home, or Home Assistant

### Secondary Requirements
- **Availability**: Both online and in-store options in Chile (retailers like Falabella, Paris, Ripley, MercadoLibre)
- **Cost Effectiveness**: Prioritize best value for money backed by positive user feedback from Reddit, forums, and reviews
- **Use Case**: Daily cleaning & mopping with minimal intervention + occasional deep cleaning
- **Pet Hair**: Not a priority (no pets in household)

## Analysis Requirements

### Tier Classification
Create a tier table (S, A, B, C, D tiers) based on:
1. **Vinyl Floor Safety**: No risk of water damage or scratching
2. **Mopping Performance**: Quality of mopping system (rotating mops > vibrating > static)
3. **Automation Level**: Auto-emptying, self-cleaning mops, smart navigation
4. **Cost Effectiveness**: Price vs features ratio within budget
5. **Availability in Chile**: Local support, warranty, ease of purchase
6. **User Reviews**: Real-world feedback from Reddit, forums, and review sites
7. **Battery Life**: Ability to complete 80m² in one session
8. **Smart Home Compatibility**: Verified Alexa/Google/Home Assistant integration, or at least non-official support (like IFTTT, or Home Assistant community plugins)

### Evaluation Methodology
1. **Filter** inventory to models ≤$700,000 CLP available in Chile
2. **Prioritize** models with:
   - Confirmed vinyl floor compatibility
   - ≥90 minutes battery life
   - Auto-emptying station (preferred)
   - Rotating or advanced mopping systems
   - Smart home integration
   - Positive user reviews
3. **Rank** by tier based on overall score across all criteria
4. **Include** for each model:
   - Tier placement with justification
   - Key strengths and weaknesses
   - Price and where to buy in Chile
   - User feedback summary with citations
   - Specific vinyl floor performance notes

## Deliverable Specifications

**Output File**: `./analytics/recommendation.md`

**Required Sections**:
1. **Executive Summary**: Top 3 recommendations with brief rationale
2. **Tier Table**: Complete tier classification (S/A/B/C/D) with all qualifying models
3. **Detailed Model Analysis**: For each tier, provide:
   - Model specifications relevant to user requirements
   - Vinyl floor compatibility assessment
   - Mopping system evaluation
   - Automation features
   - Chilean availability and pricing
   - User feedback summary with source citations
   - Pros/cons specific to user's use case
4. **Purchase Recommendations**: Where to buy in Chile (online/in-store) with current pricing
5. **Final Recommendation**: Single best choice based on all criteria with detailed justification

**Citation Requirements**:
- Reference inventory.md citations [1]-[9] and [W1]-[W20]
- Include user review sources (Reddit threads, forums)
- Cite Chilean retailer pricing where available

**Format**: Professional markdown report with clear tables, headings, and actionable recommendations
