# Task: Update Robot Vacuum Inventory from Web Sources

## Objective
Update and verify the robot vacuum inventory table at `./analytics/inventory.md` using web-based research, ensuring all data points are properly cited and verified from authoritative sources.

## Starting Points
Use links from source documents in `source_docs/` as initial research sources:
- Manufacturer websites (Dreame, Xiaomi, Roborock, Ecovacs, Narwal, Eufy, iRobot, Cecotec)
- Review sites: VacuumWars, RTINGS, Xataka, HogarSys
- Retailers: Amazon, MercadoLibre Chile, Nuvac

---

## Research Iterations

### Iteration 1: Technical Specifications
**Focus**: Verify and complete core technical data
- Suction Power (Pa)
- Navigation Technology
- Dustbin Capacity (L)
- Battery Life (h/min)
- Water Tank Capacity (L)

**Priority Sources**:
1. Manufacturer official websites
2. Major retailers (Amazon, official distributors)
3. Technical review sites (RTINGS, VacuumWars)

### Iteration 2: Cleaning Technology & Features
**Focus**: Cleaning capabilities and unique features
- Cleaning Technology (mop type, vibration, rotation)
- Brush Roll Type
- Auto-Emptying Station capabilities
- Additional Features

**Priority Sources**:
1. Manufacturer specs
2. In-depth reviews (VacuumWars, Xataka, HogarSys)
3. YouTube review channels with technical analysis

### Iteration 3: Smart Features & Compatibility
**Focus**: App control and smart home integration
- App & Smartphone Control
- Compatibility with Home Automation (Alexa, Google, HomeKit)

**Priority Sources**:
1. Manufacturer app documentation
2. Smart home compatibility databases
3. User reviews mentioning integration

### Iteration 4: Pricing & Availability (Chile Market)
**Focus**: Current market data for Chile
- Price (CLP)
- Brand Availability in Chile
- Import vs local availability

**Priority Sources**:
1. Chilean retailers (MercadoLibre Chile, Paris, Falabella, Ripley)
2. Official distributors in Chile
3. Import cost calculators

### Iteration 5: User Feedback & Known Issues
**Focus**: Real-world performance data
- Pros & Cons
- Known Issues
- User Reviews summary

**Priority Sources**:
1. Reddit (r/RobotVacuums, r/Roborock, r/Xiaomi, r/chile)
2. Amazon reviews (aggregate sentiment)
3. Forum discussions
4. YouTube long-term reviews

### Iteration 6: Value Assessment
**Focus**: Comparative analysis
- Brand Reputation
- Cost Effectiveness
- Automation Level

**Priority Sources**:
1. Comparative review articles
2. Expert rankings
3. Price-to-feature analysis

---

## Data Verification Process

1. **Cross-reference**: Each data point must be verified against at least 2 independent sources
2. **Conflict resolution**: When sources disagree, prefer:
   - Manufacturer specs for technical data
   - Multiple user reports for real-world issues
   - Most recent data for pricing
3. **Date tracking**: Note access date for all sources (especially pricing)

---

## Citation Standards

### Format
Use bracketed reference numbers: `[W1]`, `[W2]`, etc. for web sources

### Required Information
Each citation must include:
- Source name
- URL
- Access date

### Citation Section
Add a new section at the end of inventory.md:

```markdown
## Web Source References

[W1]: Source Name - URL (Accessed: YYYY-MM-DD)
[W2]: Source Name - URL (Accessed: YYYY-MM-DD)
```

---

## Data Handling Rules

### DO:
- Leave cells empty if information cannot be verified
- Use ranges when sources provide varying data (e.g., "5,000-6,000")
- Note discrepancies in parentheses when significant
- Prioritize manufacturer data for specs
- Cite every data point with web source references

### DO NOT:
- Fabricate or assume data
- Use outdated pricing (>3 months old) without notation
- Copy text verbatim without citation
- Mix currencies without conversion notation

### Source Priority (highest to lowest):
1. Manufacturer official websites
2. Authorized retailers/distributors
3. Technical review sites (RTINGS, VacuumWars)
4. Reputable tech media (Xataka, The Verge, TechRadar)
5. User forums and Reddit (for issues/reviews only)

---

## Quality Criteria

### Complete Entry Requirements:
- [ ] All core specs verified (suction, navigation, capacity, battery)
- [ ] Cleaning technology documented
- [ ] Price with currency and source date
- [ ] At least 2 citations per model
- [ ] Pros/Cons from user feedback
- [ ] Known issues section (or explicit "None reported")

### Accuracy Standards:
- Technical specs match manufacturer data
- Prices current within 3 months
- User feedback represents multiple sources
- All claims have citations

---

## Output Format

Maintain the existing markdown table structure at `./analytics/inventory.md`:
- Keep all current columns
- Add web citations using [W#] format alongside existing [#] references
- Update Source References section with new web sources
- Preserve existing source document references

---

## Execution Checklist

- [ ] Review current inventory state
- [ ] Complete Iteration 1 (Technical Specs)
- [ ] Complete Iteration 2 (Cleaning Technology)
- [ ] Complete Iteration 3 (Smart Features)
- [ ] Complete Iteration 4 (Pricing Chile)
- [ ] Complete Iteration 5 (User Feedback)
- [ ] Complete Iteration 6 (Value Assessment)
- [ ] Verify all citations are complete
- [ ] Update Source References section
- [ ] Final review for consistency

