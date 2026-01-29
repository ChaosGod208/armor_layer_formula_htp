# HTP — Armor Layer Formula

**A universal flat-armor system designed to pair with Relative Defense Formula — enabling clean, scalable, post-mitigation damage reduction for RPG/ARPG/MMO/MOBA combat systems.**

---

## 🧠 Overview

The **Armor Layer Formula** introduces a second layer of defense: **flat damage reduction applied after all other mitigation**. It complements percentage-based systems like **Relative Defense**, solving the late-game tankiness problem while preserving early-game balance.

This system is ideal for games needing **predictable, scalable, and class-neutral survivability curves**.

---

## 🧩 Core Mechanics

1. **Two-Layer Defense Model**  
   - **Relative Defense (DEF):** Percentage-based mitigation  
   - **Armor:** Flat reduction applied *after* all other formulas

2. **Armor Formula**  
   \[
   Armor = \frac{Defense}{15}
   \]  
   - Max boostable to:  
     \[
     Armor = \frac{Defense}{10}
     \]  
     via passives, traits, or class bonuses

3. **Final Damage Calculation**  
   \[
   FinalDamage = \max(0, DamageAfterAllMitigation - Armor)
   \]

---

## 🔢 Examples

| Scenario | Monster Hit | Player DEF | Armor | Damage After Mitigation | Final Damage |
|----------|-------------|------------|--------|--------------------------|---------------|
| Base Case | 10,000 | 1,500 | 100 | 7,000 | **6,900** |
| High DEF | 2,000 | 3,000 | 200 | 1,200 | **1,000** |
| Max Boost | 2,000 | 2,000 (×1.5) | 200 | 1,200 | **1,000** |

---

## ✅ Design Benefits

- **Post-mitigation layer** — cleanly separates % reduction from flat reduction  
- **Scales with defense** — but never overpowers early game  
- **Prevents late-game defense inflation** — avoids “immortal tanks”  
- **Keeps low-damage enemies relevant** — even at high levels  
- **Works across genres** — RPGs, shooters, MOBAs, strategy games

---

## 🧪 Applications

- **RPG / ARPG / MMO tanking systems**  
- **Shooter ballistic armor**  
- **MOBA final damage clamps**  
- **Strategy unit survivability**  
- **PvP balance tuning**

---

## 🔁 Recommended Pairing

Combine with **HTP Relative Defense Formula** for optimal results:

| Layer | Role |
|-------|------|
| **Relative DEF** | Dynamic % scaling — handles early/mid-game |
| **Armor Layer** | Stable flat reduction — ensures late-game survivability |

→ Together, they form a **two-layer defense system** with satisfying progression and no power creep.

---

## 🆓 License

**Public Domain.** Use, fork, modify, or integrate freely. No attribution required — but linking back is appreciated.

---

## 🔗 Original Gist

HTP Armor Layer Formula — [Gist Version](https://gist.github.com/ChaosGod208/88ef5ca1a2edeb1796c79c905772e2cf)

Relative defense formula - [Gist version](https://gist.github.com/ChaosGod208/f16731a46cc8c39b3392a47e7915aca3)

Full gist archive (100+ frameworks): [ChaosGod208 gist](https://gist.github.com/ChaosGod208)

---

**Made with raw insight & zero corporate fluff.**  
— ChaosGod208
