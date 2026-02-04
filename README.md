# C&I Demand Response Simulator

An interactive demo exploring how demand response helps commercial and industrial customers reduce costs, earn incentives, and support grid reliability — built to demonstrate product thinking for [Puget Sound Energy](https://www.pse.com/).

**[View Live Demo →](https://YOUR-USERNAME.github.io/energy-shift-simulator/)**

![C&I Demand Response Simulator Screenshot](screenshot.png)

---

## Why I Built This

Puget Sound Energy is developing demand response programs to help commercial and industrial customers reduce peak energy consumption while earning revenue. The core challenge: **making complex C&I demand response concepts accessible to multiple stakeholders** — facility managers who need to understand operational impacts, CFOs who need to see the business case, and operations teams who need to plan around events.

This simulator explores that challenge through four interconnected features, demonstrating how demand response value propositions can be communicated effectively to drive program enrollment and engagement.

---

## Features & Product Thinking

### 🏢 Customer Segment Selector
**Problem:** C&I customers vary dramatically — a restaurant has different loads, constraints, and economics than a data center.

**Solution:** Four distinct customer segments (SMB, Commercial, Industrial, Large Load) with realistic load profiles, demand charges, and facility-specific equipment. Selecting a segment instantly updates all calculations and recommendations to match that customer's reality.

---

### 📊 Load Profile Visualization
**Problem:** Customers don't know which loads they can curtail vs. which are critical to operations.

**Solution:** Visual breakdown of facility loads showing curtailable vs. critical classification. The 24-hour demand chart shows baseline consumption and what happens during a DR event — making the curtailment opportunity concrete and measurable.

---

### 💰 DR Program Comparison
**Problem:** Multiple program types exist (capacity, energy, emergency) with different payment structures, notice periods, and penalties. Customers struggle to compare options.

**Solution:** Side-by-side comparison of three program types showing:
- Payment structure ($/kW/month vs $/kWh)
- Firm commitment vs. economic dispatch
- Auto-DR vs. manual response requirements
- Penalty structures and event frequency

---

### 📈 Business Case Builder
**Problem:** Decision-makers need to justify DR participation with hard numbers — implementation costs, payback period, annual ROI.

**Solution:** Dynamic calculator that combines:
- Incentive revenue based on selected program
- Demand charge savings ($/kW matters more than $/kWh for C&I)
- Implementation costs (~$15/kW for controls)
- Payback period in months
- Ongoing annual benefit

---

### ⚙️ Operational Impact Scenarios
**Problem:** Operations teams worry: "What happens to my facility during a 4-hour event?"

**Solution:** Segment-specific impact scenarios showing:
- What each curtailable load experiences during an event
- Severity ratings (low/moderate)
- Mitigation strategies (pre-cooling, production shifting, etc.)
- Stakeholder communication guide (Facility Manager, CFO, Operations)

---

## Key C&I vs. Residential Differences

| Residential Focus | C&I Focus (This Demo) |
|------------------|----------------------|
| Individual appliances | Facility-level loads (HVAC systems, industrial processes) |
| Simple kWh savings | Demand charges ($/kW) often matter more than energy ($/kWh) |
| Single user decision | Multiple stakeholders (facility manager, CFO, operations) |
| Comfort trade-offs | Production/operations impact concerns |

---

## Technical Implementation

- **Stack:** React 18, vanilla CSS-in-JS
- **Hosting:** GitHub Pages (static HTML with CDN-loaded React)
- **No build step:** Single `index.html` file for simplicity

The simulator is intentionally lightweight — demonstrating that effective B2B experiences don't require complex infrastructure.

---

## Alignment with PSE's C&I Demand Response Goals

| PSE Goal | How This Demo Addresses It |
|----------|---------------------------|
| Develop new energy solutions for C&I customers | Four distinct customer segments with segment-specific load profiles and economics |
| Market research & stakeholder engagement | Multi-stakeholder communication guide addresses FM, CFO, and Operations concerns |
| Drive program enrollment | Business case builder makes ROI tangible with payback periods and annual savings |
| Financial modeling & P&L | Dynamic calculations for incentive revenue, demand charge savings, and implementation costs |
| Go-to-market strategy | Program comparison helps customers self-select the right program for their operations |
| Partnership & vendor management | Auto-DR recommendations show how technology partnerships enable faster response |

---

## About Me

I'm Nora — a product-minded builder exploring the energy transition. I built this to demonstrate how I think about B2B product challenges: understanding diverse customer segments, addressing multiple stakeholder concerns, and making complex economics feel simple.

**Let's chat:** [LinkedIn](https://linkedin.com/in/YOUR-PROFILE) | [Email](mailto:your@email.com)

---

## Running Locally

Just open `index.html` in a browser. No dependencies, no build step.

```bash
# Or use a local server if you prefer
npx serve .
```

---

## License

MIT — feel free to fork and adapt.
