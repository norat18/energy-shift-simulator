# energy-shift-simulator
See how shifting your energy use helps you save money, stay comfortable, and strengthen the grid. 
# Energy Shift Simulator

An interactive demo exploring how smart energy shifting helps homeowners save money while supporting grid stability — built to demonstrate product thinking for [Renew Home](https://www.renewhome.com/).

**[View Live Demo →](https://YOUR-USERNAME.github.io/energy-shift-simulator/)**

![Energy Shift Simulator Screenshot](screenshot.png)

---

## Why I Built This

Renew Home is building North America's largest residential virtual power plant (VPP) by helping millions of homes shift energy use to cheaper, cleaner times. The core challenge: **making complex energy concepts feel simple and actionable for everyday consumers** — people who want to save money without becoming energy experts.

This simulator explores that challenge through five interconnected features.

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

## Alignment with Renew Home's Mission

| Renew Home Goal | How This Demo Addresses It |
|-----------------|---------------------------|
| "Make it easy for customers to save energy and money" | Every feature focuses on clarity and actionability |
| "Without needing to be energy experts" | Complex concepts (TOU rates, demand response, VPP) explained visually |
| "Improve comfort and increase resilience" | Comfort slider + Resilience Score make these tangible |
| "Surface new ways for users to save" | Home Opportunities provides personalized recommendations |
| "Partner-integrated product requirements" | Device ecosystem shows how OEM partnerships create user value |

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
