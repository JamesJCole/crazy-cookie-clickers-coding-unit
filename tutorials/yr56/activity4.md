# Cookie Multipliers

```template
let cookies = 0
let grandmas = 0
let farms = 0
let factories = 0
let grandmaCost = 15
let farmCost = 100
let factoryCost = 500
let cookiesPerSecond = 0
scene.setBackgroundColor(3)
let cookie = sprites.create(img`
...............................
............dddddd.............
.........44444444444d..........
.......e44444ed44dd444d........
......e444444eee4444444d.......
....e44444444eee44444d44dd.....
....4444edd444e4444444444d.....
...e444eeed444444444444444d....
..e4444eeee444444dd444e4d4dd...
..444444eee44444eed44eee444d...
.e444444ee444444ee444eee4444d..
.e44444444444444444444ee44444..
e44ee444444444444444444444444..
e44ee44444444ed44444444444444d.
e444444444444eee4444444dd4444d.
e444444444444ee4444444eedd444d.
e444444e4444444444d444eeee444d.
e44444eee44444444edd44eee4444d.
ee4444eeee44eed44eee44444444dd.
.e44444ee444eee44ee44444e444d..
.ee44444e444eee44444444eeee44..
.ee4444444444ee44444444eee44d..
..e444444444444444444444e444...
..ee444444e44444444444444444...
...e44444eee444eee444444444....
....ee444eee444eee444eed44.....
.....ee444e4444eee44eeee4e.....
......eee4444444e4444eee.......
........eee4444444444ee........
.........eeeee44444ee..........
............eeeeee.............
...............................
`, SpriteKind.Player)
cookie.setPosition(70, 60)
info.setScore(0)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += 1
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= grandmaCost) {
        cookies -= grandmaCost
        grandmas += 1
        grandmaCost = Math.round(grandmaCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= grandmaCost / 2) {
        game.showLongText("Almost there! Need " + (grandmaCost - cookies) + " more cookies.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Grandma costs " + grandmaCost + " cookies.", DialogLayout.Bottom)
    }
})
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= farmCost) {
        cookies -= farmCost
        farms += 1
        farmCost = Math.round(farmCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= farmCost / 2) {
        game.showLongText("Almost there! Need " + (farmCost - cookies) + " more for a Farm.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Farm costs " + farmCost + " cookies.", DialogLayout.Bottom)
    }
})
controller.down.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= factoryCost) {
        cookies -= factoryCost
        factories += 1
        factoryCost = Math.round(factoryCost * 1.15)
        info.setScore(cookies)
    } else if (cookies >= factoryCost / 2) {
        game.showLongText("Almost there! Need " + (factoryCost - cookies) + " more for a Factory.", DialogLayout.Top)
    } else {
        game.showLongText("Keep baking! Factory costs " + factoryCost + " cookies.", DialogLayout.Bottom)
    }
})
game.onUpdateInterval(1000, function () {
    let total = 0
    for (let i = 0; i <= 2; i++) {
        if (i == 0) {
            total += grandmas * 1
        } else if (i == 1) {
            total += farms * 8
        } else if (i == 2) {
            total += factories * 47
        }
    }
    cookiesPerSecond = total
    cookies += cookiesPerSecond
    info.setScore(cookies)
    if (grandmas >= 5 && farms >= 3) {
        cookies += 10
    }
})
```

## Nested Conditions @showdialog

Your factory from Activities 1–3 is already loaded — three upgrades, ``else if`` messages, and a for loop calculating production each second!

So far your conditions are fairly straightforward. But what about a situation where you need to check **one thing, and then another thing depending on the first result**?

That is **nested conditions** — an ``if`` block inside another ``if`` block:

```
if grandmas >= 10 then
    if farms >= 5 then
        bonus = HUGE   (both grandmas AND farms maxed)
    else
        bonus = medium  (only grandmas)
else
    if farms >= 5 then
        bonus = medium  (only farms)
    else
        bonus = none    (neither)
```

In this activity you will:
- **Design** a bonus multiplier system on paper first
- **Implement** it using nested if/else
- Combine it with the for loop to apply the multiplier to total production

This is the most complex concept in this skillmap — take your time and think carefully!

This is **AC9TDI6P02** at its full depth.

## Step 1 — Design on paper first

**Algorithm design challenge — do this before touching code!**

Draw a flowchart (or write pseudocode) for this rule:

> Calculate a ``bonusMultiplier`` based on how many grandmas and farms you have:
> - grandmas ≥ 10 **AND** farms ≥ 5 → multiplier = **4** (master baker!)
> - grandmas ≥ 10 (but not enough farms) → multiplier = **2**
> - farms ≥ 5 (but not enough grandmas) → multiplier = **2**
> - neither condition met → multiplier = **1** (no bonus)

How many different outcomes are there? (Answer: 4)
How many conditions do you need to check? (Answer: 2, nested)

Show your design to your teacher before moving on.

## Step 2 — Create a bonusMultiplier variable

In ``||loops:on start||``, add a new variable ``bonusMultiplier`` and set it to **1**.

```blockconfig.local
let bonusMultiplier = 1
```

```blocks
let bonusMultiplier = 1
```

## Step 3 — The outer if (check grandmas)

After the for loop in your ``||game:on game update every 1000 ms||`` block, add the outer condition:

``if grandmas >= 10`` — this is the **outer** decision.

Inside the ``if``:
- Add another ``if/else`` to check ``farms >= 5``
- If farms also >= 5: set ``bonusMultiplier`` to **4**
- Else (grandmas >= 10 but not enough farms): set ``bonusMultiplier`` to **2**

```blockconfig.local
if (grandmas >= 10) {
    if (farms >= 5) {
        bonusMultiplier = 4
    } else {
        bonusMultiplier = 2
    }
}
```

```blocks
if (grandmas >= 10) {
    if (farms >= 5) {
        bonusMultiplier = 4
    } else {
        bonusMultiplier = 2
    }
}
```

## Step 4 — The outer else (grandmas < 10)

Add an ``else`` to the outer condition. Inside it:
- Add another ``if/else`` to check ``farms >= 5``
- If farms >= 5 (but grandmas < 10): set ``bonusMultiplier`` to **2**
- Else (neither): set ``bonusMultiplier`` to **1**

```blocks
if (grandmas >= 10) {
    if (farms >= 5) {
        bonusMultiplier = 4
    } else {
        bonusMultiplier = 2
    }
} else {
    if (farms >= 5) {
        bonusMultiplier = 2
    } else {
        bonusMultiplier = 1
    }
}
```

## Step 5 — Apply the multiplier

Now use ``bonusMultiplier`` in your production calculation. Modify the for loop result:

After calculating ``total`` in the for loop, multiply by ``bonusMultiplier``:

```blockconfig.local
cookiesPerSecond = total * bonusMultiplier
```

```blocks
game.onUpdateInterval(1000, function () {
    let total = 0
    for (let i = 0; i <= 2; i++) {
        if (i == 0) {
            total += grandmas * 1
        } else if (i == 1) {
            total += farms * 8
        } else if (i == 2) {
            total += factories * 47
        }
    }
    if (grandmas >= 10) {
        if (farms >= 5) {
            bonusMultiplier = 4
        } else {
            bonusMultiplier = 2
        }
    } else {
        if (farms >= 5) {
            bonusMultiplier = 2
        } else {
            bonusMultiplier = 1
        }
    }
    cookiesPerSecond = total * bonusMultiplier
    cookies += cookiesPerSecond
    info.setScore(cookies)
})
```

## Step 6 — Test nested conditions

Verify each of the 4 outcomes:

1. **0 grandmas, 0 farms:** multiplier = 1 (no bonus) — check
2. **0 grandmas, 5+ farms:** multiplier = 2 — buy 5 farms and verify
3. **10+ grandmas, 0 farms:** multiplier = 2 — buy 10 grandmas and verify
4. **10+ grandmas, 5+ farms:** multiplier = 4 — build both and verify the CPS quadruples!

**Trace the nested logic:** For 10 grandmas and 3 farms, which path does the code take?
- Outer if: grandmas >= 10 ✓ → enter outer if
- Inner if: farms >= 5? No (3 < 5) → take inner else
- Result: multiplier = 2 ✓

## Step 7 — Refactor challenge

**Extension:** Can you refactor the nested condition into a *single* condition using ``AND`` and ``OR``?

Hint: ``if grandmas >= 10 AND farms >= 5`` for the 4× case, then two separate ``else if`` for the 2× cases.

Which approach is easier to read? Which is easier to extend? Discuss with a partner.

## Complex branching achieved! @showdialog

**Phenomenal work!** You have implemented one of the most complex patterns in programming.

**What you built:**
- A nested if/else system with 4 distinct outcomes
- A bonus multiplier applied through the production loop
- An algorithm you designed *before* implementing

**What this means (AC9TDI6P02):** You *designed* and implemented an algorithm with **complex branching** — nested conditions where the inner check depends on the outer result.

**Final activity:** Activity 5 — Cookie Empire. You will add a prestige system, a win condition, and put your complete game together!
