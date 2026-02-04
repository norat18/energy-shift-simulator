# energy-shift-simulator
See how shifting your energy use helps you save money, stay comfortable, and strengthen the grid. 
# Energy Shift Simulator

An interactive demo exploring how smart energy shifting helps customers save money while supporting grid stability — built to demonstrate product thinking for [Puget Sound Energy](https://www.pse.com/).

**[View Live Demo →](https://YOUR-USERNAME.github.io/energy-shift-simulator/)**

![Energy Shift Simulator Screenshot](screenshot.png)

---

## Why I Built This

Puget Sound Energy is developing demand response programs to help commercial and industrial customers reduce peak energy consumption while saving money. The core challenge: **making complex energy concepts feel simple and actionable for customers** — businesses that want to reduce costs and support grid reliability without becoming energy experts.

This simulator explores that challenge through five interconnected features, demonstrating how demand response value propositions can be communicated effectively to drive program enrollment and engagement.

---

## Features & Product Thinking

### 📊 Energy Shift Visualization
**Problem:** Most people don't understand *when* energy is expensive or *why* shifting matters.

**Solution:** A 24-hour usage chart that shows baseline vs. optimized consumption in real-time. Toggle "Energy Shift" on/off to see the difference. The "Simulate Day" animation makes the pre-cooling → peak reduction pattern intuitive.

---

### 🎚️ Comfort vs. Savings Slider
**Problem:** Users have different tolerances — some prioritize savings, others want minimal disruption.

**Solution:** A simple slider that adjusts the aggressiveness of energy shifts. The UI responds dynamically, showing how their choice affects estimated savings. This builds trust by giving users control.

---

### 🏠 Device Ecosystem
**Problem:** VPP value scales with more connected devices, but users don't see how each device contributes.

**Solution:** Toggle devices (thermostat, water heater, EV charger, battery, pool pump) and watch savings/grid impact update. Each device shows its individual contribution, making the value of adding devices tangible.

---

### 💡 Home Opportunities
**Problem:** Users don't know what actions would help them save more.

**Solution:** Personalized recommendations based on current setup. Missing a battery? We suggest it with estimated impact. On a flat rate? We explain why TOU could unlock more savings. This mirrors the "Home Opportunities" feature area in the PM role.

---

### ⚡ Rate Plan Comparison
**Problem:** Time-of-use rates are confusing, and users don't understand why they matter for energy shifting.

**Solution:** Visual comparison of Flat, TOU, and TOU+ rate structures with a 24-hour price chart. Makes it obvious why shifting usage to green (cheap) hours saves money.

---

### 🛡️ Resilience Score
**Problem:** Energy resilience is abstract — users don't know how prepared they are for outages.

**Solution:** A simple 0-100 score with clear breakdown of what contributes (battery = +35 pts, etc.). Creates a gamified path toward better preparedness while surfacing upgrade opportunities.

---

## Technical Implementation

- **Stack:** React 18, vanilla CSS-in-JS
- **Hosting:** GitHub Pages (static HTML with CDN-loaded React)
- **No build step:** Single `index.html` file for simplicity

The simulator is intentionally lightweight — demonstrating that effective consumer experiences don't require complex infrastructure.

---

## Alignment with PSE's C&I Demand Response Goals

| PSE Goal | How This Demo Addresses It |
|----------|---------------------------|
| Develop new energy solutions for C&I customers | Demonstrates customer-facing product concepts that make demand response accessible |
| Market research & stakeholder engagement | Shows how to communicate value propositions and gather user preferences (comfort vs. savings) |
| Drive program enrollment | Visualizes ROI clearly with savings calculators and collective grid impact |
| Financial modeling & P&L | Real-time savings estimates demonstrate how to present financial benefits to customers |
| Go-to-market strategy | Personalized "Opportunities" feature shows how to upsell additional services and devices |
| Partnership & vendor management | Device ecosystem demonstrates how equipment partnerships create customer value |

---

## About Me

I'm Nora — a product-minded builder exploring the energy transition. I built this to demonstrate how I think about consumer product challenges: starting with user needs, making complex systems feel simple, and shipping something tangible.

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
