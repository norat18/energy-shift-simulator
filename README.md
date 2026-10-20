# C&I Demand Response Simulator

An interactive demo exploring how demand response helps commercial and industrial customers reduce costs, earn incentives, and support grid reliability. Built to demonstrate product thinking for [Puget Sound Energy](https://www.pse.com/), and grounded in PSE's published Flex program terms and system peak data.

**[View Live Demo →](https://norat18.github.io/energy-shift-simulator/)**

---

## Why I Built This

PSE needs a lot more demand response, fast. It has about 129 MW of demand response today. Under Washington's 2024 Decarbonization Act for Large Combination Utilities, it must plan for load flexibility equal to 10% of its winter and summer peaks, which PSE estimates at roughly 500 MW by 2030. Commercial and industrial customers make up about 55% of PSE's peak demand, so they are central to closing that gap.

The core challenge: **making C&I demand response concrete and trustworthy for every stakeholder.** Facility managers need to know what happens to their building. CFOs need a business case that survives scrutiny. Operations teams need to plan around events. This simulator walks each of them from "what is this?" to "should we enroll?"

---

## Features & Product Thinking

### 🏢 Customer Segments + "Model Your Facility"
**Problem:** C&I customers vary dramatically, and generic numbers don't persuade anyone.

**Solution:** Five segments (Small-Medium Business, Commercial, Industrial, Large Load, and Fleet Depot for EV charging) with winter and summer load shapes. Every load's kW and "can shed %" is editable, so a prospect can model *their* building. Peak demand determines the PSE rate schedule (24, 25 or 26), which determines which programs they can join.

---

### ❄️ Event Settings Grounded in PSE's Grid
**Problem:** Most DR demos assume a summer-afternoon peak. PSE peaks in winter, every year.

**Solution:** Event windows match PSE's own peak data: winter mornings (7–10 AM) and evenings (5–10 PM), plus summer afternoons (3–9 PM). Event duration is capped at 4 hours, per PSE's Flex terms. A single "delivered performance" setting drives the chart, payments, and settlement, so every number in the tool agrees.

---

### 📊 Load Profile: The Actual Shift
**Problem:** Curtailed energy doesn't disappear. HVAC pre-conditions, production gets rescheduled, and EV fleets charge later. That snapback can set a *new* monthly peak and wipe out the savings.

**Solution:** The 24-hour chart shows pre-conditioning, the event, and the rebound, with three recovery strategies: uncontrolled restart, pre-condition + ramp, and staggered (valley-fill) restart. Callouts flag when your peak falls outside the event window (no demand-charge savings) or when the rebound sets a new peak. PSE's 2026 DR RFP explicitly asks vendors to forecast this "pre-conditioning and snapback."

---

### 💰 PSE Flex Program Comparison
**Problem:** Customers can't tell which program fits them or what they'd actually earn.

**Solution:** PSE's three business programs, using their published terms:
- **Flex C&I:** up to $65/kW per season (up to $130/kW a year), with no-cost enrollment support from PSE and Enel
- **Flex Business:** $1/kWh saved, for Schedules 24 and 25
- **Flex Smart (business thermostats):** $35/kW per season, for Schedules 24 and 25

Each program shows eligibility for the modeled facility and an estimated annual incentive. PSE's published terms include no financial penalties, so a shortfall shows up as unearned incentive, not a charge.

---

### 🧾 Baseline & Settlement
**Problem:** "How do I get paid?" is the most common C&I question, and baselines are confusing.

**Solution:** A step-by-step settlement of one event using a common method: a 10-in-10 baseline with a day-of adjustment. It shows why the adjustment matters on extreme-weather days, and why the adjustment window has to end before pre-conditioning starts.

---

### 📈 Risk-Adjusted Business Case
**Problem:** Decision-makers need numbers that hold up, not best-case marketing.

**Solution:**
- Flex C&I rate and committed-kW sliders
- Demand charge savings counted only in months where an event lands on the billing peak, at Schedule 26 winter and summer rates
- Manual plan (no cost) vs. automated controls (upfront cost, editable)
- 10-year NPV, payback, and downside / expected / upside scenarios

---

### ⚙️ Operations, 🌎 Grid & Carbon, ✅ Next Steps
- **Operations:** segment- and season-specific impacts and mitigations, the restart plan, and a stakeholder communication guide
- **Grid & Carbon:** PSE's 2019–2025 winter vs. summer peaks, progress toward the 2030 DR need, a portfolio slider ("if 100 sites like this enrolled…"), and CETA context
- **Next Steps:** a readiness checklist, manual vs. automated response paths, and PSE's actual Flex C&I enrollment process

---

### 🔍 What's Sourced vs. Assumed
**Problem:** A demo that blends real program terms with modeled values can mislead if it doesn't say which is which.

**Solution:** A panel on every tab sorts everything into three groups: **confirmed** from PSE and state sources, **modeled** (with the reason for each assumption), and **unknown until enrollment**. Amber "assumed" tags mark the affected numbers in the tool. For example, PSE says Flex C&I pay "combines" committed kW and performance but doesn't publish the formula, so the simulator labels its formula as an assumption.

---

## Key C&I vs. Residential Differences

| Residential Focus | C&I Focus (This Demo) |
|------------------|----------------------|
| Individual appliances | Facility-level loads (HVAC, process equipment, EV fleets) |
| Simple kWh savings | Demand charges ($/kW) set by a single monthly peak, which a rebound can raise |
| Single user decision | Multiple stakeholders (facility manager, CFO, operations) |
| Comfort trade-offs | Production and operations impact, commitment levels, settlement |

---

## Sources

Program terms and data were checked in October 2026. PSE may change incentives at any time.

- [PSE Flex C&I](https://www.pse.com/en/business-incentives/energy-management-programs/flex-c-i) and [Flex for Business](https://www.pse.com/en/business-incentives/energy-management-programs/flex-for-business)
- [PSE Demand Response terms and conditions](https://www.pse.com/en/rebates/PSE-flex/PSE-Demand-Response-terms-and-conditions)
- [PSE 2026 Demand Response RFP](https://www.pse.com/en/pages/energy-supply/acquiring-energy/2026-Demand-Response-Request-for-Proposals) (peak data, DR portfolio, 2030 need)
- [Schedule 26 rates via OpenEI](https://apps.openei.org/USURDB/rate/view/69ef9df37b85aa692d050dba)
- CETA: [RCW 19.405.030](https://app.leg.wa.gov/rcw/default.aspx?cite=19.405.030) and [RCW 19.405.040](https://app.leg.wa.gov/rcw/default.aspx?cite=19.405.040)

Load shapes, segment bills, controls costs, and emissions factors are illustrative.

---

## Technical Implementation

- **Stack:** React 18 (pinned CDN versions), inline CSS-in-JS
- **Hosting:** GitHub Pages (static HTML)
- **No build step:** a single `index.html` file

The simulator is intentionally lightweight, to show that an effective B2B experience doesn't need complex infrastructure.

---

## About Me

I'm Nora, a product-minded builder exploring the energy transition. I built this to show how I approach B2B product challenges: understanding diverse customer segments, addressing multiple stakeholders, grounding the experience in real program rules, and being upfront about what's known and what's assumed.

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

MIT. Feel free to fork and adapt.
