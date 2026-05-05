# 🔌 Don't Melt The Wires

> A browser-based cable and wire sizing calculator. Enter your load, run length, and installation method — get the right cable size before something catches fire.

**🔗 Live App:** [kbcianfa.github.io/DontMeltWires](https://kbcianfa.github.io/DontMeltWires)

---

## What It Does

Don't Melt The Wires takes the guesswork out of selecting electrical cable for 12V/24V DC systems — the kind found in caravans, RVs, boats, ute trays, solar setups, and shed wiring. Feed it your current draw, cable run length, and installation conditions, and it calculates the minimum safe cable size based on two key constraints:

**Ampacity** — the maximum current the cable can carry without overheating.  
**Voltage drop** — the resistance-induced loss across the run length, which kills performance at the load end.

It recommends the cable size that satisfies *both* constraints, then shows you the margins on a set of visual gauges so you can see exactly how hard you're pushing the wire.

---

## Features

**Inputs**
- Load current (amps)
- System voltage (12V / 24V toggle)
- One-way cable run length
- Installation method (free air, bundled, conduit, etc.) with derating factors applied automatically
- Conductor material (copper / aluminium)
- Ambient temperature adjustment

**Results**
- Recommended cable size (mm²) — the minimum that passes both checks
- Ampacity gauge with needle indicator showing current vs cable capacity
- Voltage drop gauge showing % loss across the run
- Bar meters for safety margin, derating load, and headroom
- Clear PASS / WARN / DANGER verdict on the result

**Design**
- Dark navy industrial aesthetic with green/blue accent gauges
- Animated SVG needle gauges with arc fill
- Responsive two-column layout → stacked on mobile
- No install, no backend — runs entirely in the browser

---

## Who It's For

- RV and caravan builders wiring 12V accessories, solar, and battery systems
- Boat and marine electrical work
- Ute tray and canopy builds
- Solar off-grid installations
- Anyone who's ever wondered "is this cable thick enough?" and guessed wrong

---

## Tech Stack

| Thing | Detail |
|---|---|
| Language | Vanilla HTML/CSS/JS — zero build tools |
| Charts | SVG gauges and bar meters, hand-coded |
| Hosting | GitHub Pages |
| Architecture | Single-file app (`index.html`) |
| Backend | None |

Classic vibe-coded tool. One file, open it, it works.

---

## Getting Started

### Use the Hosted Version

Head to [kbcianfa.github.io/DontMeltWires](https://kbcianfa.github.io/DontMeltWires) — no sign-up, no install.

### Run Locally

```bash
git clone https://github.com/KBCIanFa/DontMeltWires.git
cd DontMeltWires
# Open index.html in your browser.
```

---

## ⚠️ Disclaimer

This tool is a sizing guide, not a certified engineering tool. Always verify critical electrical installations against the relevant Australian Standards (AS/NZS 3000, AS/NZS 3008) and have work on mains or high-current systems checked by a licensed electrician. Cable ratings vary by manufacturer — confirm against your specific cable's datasheet.

---

## Files

```
DontMeltWires/
├── index.html    # The whole app
└── README.md
```

---

## Part of the Vibe Coding Portfolio

Built at [kbcianfa.github.io](https://kbcianfa.github.io) — a suite of Australian-focused single-file web tools. Other tools in the family:

- [RV Power Designer](https://kbcianfa.github.io/RVPowerSystems) — full solar/battery system sizing for caravans
- [RV Route Planner AU](https://kbcianfa.github.io/RVRoutePlanner) — AI-powered caravan route planning
- [TowCheck AU](https://kbcianfa.github.io/Towing/) — towing compliance calculator
- [LogMyJourney AU](https://kbcianfa.github.io/LogMyJourney/) — trip logging app

---

*Built in Queensland, Australia. Don't melt the wires.*
