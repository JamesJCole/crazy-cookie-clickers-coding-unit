# Educator Guide — Cookie Clicker Skillmap

## Overview

This MakeCode Arcade Skillmap is designed for Australian primary school classrooms to teach **Digital Technologies** concepts using a **Cookie Clicker** game theme.

| Path | Year Level | Activities | Duration | Curriculum |
|------|-----------|------------|----------|------------|
| Cookie Clicker | Year 3/4 | 5 × ~12 min | ~60 min total | AC9TDI4P02 |
| Cookie Empire | Year 5/6 | 5 × ~17 min | ~85 min total | AC9TDI6P02, AC9TDI6P05 |

**No installation required** — students open the skillmap URL in a browser.

---

## How to Load the Skillmap

Once the repository is published to GitHub, share this URL with students:

```
https://arcade.makecode.com/skillmap#github:JamesJCole/crazy-cookie-clickers-coding-unit/skillmap
```

Students click their year level path and begin Activity 1. Each activity opens the MakeCode Arcade editor in their browser with step-by-step guided instructions.

**Controls in the browser:**
- **A button** = Space bar or Z key
- **B button** = X key
- **Up/Down/Left/Right** = Arrow keys

---

## Australian Curriculum v9 Alignment

### Year 3/4 — AC9TDI4P02
*Follow and describe algorithms involving sequencing, comparison operators (branching) and iteration; implement them as visual programs*

| Activity | Concept | How it is taught |
|----------|---------|-----------------|
| 1 — The Cookie Sprite | Sequence, variables | Setting up sprites and variables in order |
| 2 — Click to Bake | Events, sequence | Button event triggers a sequence of actions |
| 3 — Upgrade Time! | **Branching** | ``if/else`` decides whether you can afford an upgrade |
| 4 — Auto Baker | **Iteration** | ``on game update every 1000ms`` loop bakes cookies automatically |
| 5 — Cookie Champion | Synthesis | Win condition uses branching inside iteration |

### Year 5/6 — AC9TDI6P02 + AC9TDI6P05
*Design algorithms involving multiple alternatives (branching) and iteration; implement as visual programs with control structures, variables and input*

| Activity | Concept | How it is taught |
|----------|---------|-----------------|
| 1 — Build the Shop | Variables, simple branching | Multiple variables, three upgrades |
| 2 — Multiple Upgrades | **Multiple alternatives** | ``else if`` chains, AND conditions |
| 3 — Cookie Factory | **Iteration (for loops)** | For loop calculates production across upgrade types |
| 4 — Cookie Multipliers | **Nested conditions** | Nested if/else gives 4 distinct outcomes |
| 5 — Cookie Empire | Capstone synthesis | Prestige system combines complex branching + iteration |

---

## Suggested Lesson Structure

### Year 3/4 (3 × 20-minute sessions or 2 × 30-minute sessions)

**Session 1 (Activities 1–2):** Set up the game. Introduce variables and events.
**Session 2 (Activity 3):** Focus on **branching**. Discuss "if/else" using real-world examples (traffic lights, vending machines) before coding.
**Session 3 (Activities 4–5):** Focus on **iteration**. Discuss loops in real life (heartbeat, traffic light cycles) then implement the auto baker.

### Year 5/6 (4–5 × 20-minute sessions)

**Session 1 (Activity 1):** Build the shop foundations. Discuss why we need multiple variables.
**Session 2 (Activity 2):** Multiple alternatives. Do a quick class flowchart activity before coding.
**Session 3 (Activity 3):** For loops. Trace the loop manually on paper before implementing.
**Session 4 (Activity 4):** Nested conditions. **Algorithm design on paper is required** before students open the editor.
**Session 5 (Activity 5):** Capstone. Students work mostly independently.

---

## Classroom Tips

### Pair Programming
Pair students (one "driver", one "navigator") for Activities 3 and 4. The navigator reads the instructions and describes what to do; the driver operates the keyboard. Swap roles each step.

### Paper Design First (Year 5/6)
For Activities 3 and 4, require students to sketch their algorithm (flowchart or pseudocode) before touching the keyboard. This directly aligns with AC9TDI6P02 which requires students to **design** algorithms, not just implement them.

### Class Discussion Prompts

**For branching (Activity 3 / Yr3-4, Activity 2 / Yr5-6):**
- "What real-life decisions work like if/else?" (e.g., "if it's raining, take an umbrella")
- "What happens if we remove the else branch? What could go wrong?"

**For iteration (Activity 4 / Yr3-4, Activity 3 / Yr5-6):**
- "Where do you see loops in real life?" (factory lines, music repeating, traffic lights)
- "How would you write the cookie factory WITHOUT a loop? Would that be harder or easier?"

**For nested conditions (Activity 4 / Yr5-6):**
- "Before coding: draw the decision tree on the board together"
- "How many outcomes are there? How did you figure that out?"

### Early Finisher Extensions

| Activity | Extension idea |
|----------|---------------|
| Yr3/4 Act 3 | Add a second upgrade tier (costs 50, gives +5 per click) |
| Yr3/4 Act 4 | Make the auto baker cost increase after each purchase |
| Yr5/6 Act 3 | Add a 4th upgrade type (Mine: 200/sec, costs 5000) |
| Yr5/6 Act 4 | Refactor nested if to use AND/OR — which is more readable? |
| Yr5/6 Act 5 | Add an achievements system (first grandma, first farm, etc.) |

---

## Technical Notes

### MakeCode Arcade
- Students use the **Blocks** editor (visual drag-and-drop)
- The JavaScript view is available under the code window — great for curious students or for comparing block and text representations
- Games auto-save to the browser. Students can share their project using the "Share" button.

### Keyboard Shortcuts in MakeCode Arcade
- **Play:** F5 or the green Play button
- **Switch to JavaScript:** Click "JavaScript" tab above the code area
- **Undo:** Ctrl+Z

### Sprite Images
The tutorials include pre-drawn cookie sprites. Students can customise these by clicking the grey image square in any sprite block to open the sprite editor.

---

## Contact and Sharing

If you adapt this skillmap or create additional activities, consider sharing back with the community via the MakeCode forums at [forum.makecode.com](https://forum.makecode.com).
