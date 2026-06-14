# Cookie Empire

```template
let cookies = 0
let grandmas = 0
let farms = 0
let factories = 0
let grandmaCost = 15
let farmCost = 100
let factoryCost = 500
let cookiesPerSecond = 0
let bonusMultiplier = 1
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

## The Final Challenge! @showdialog

Your complete Cookie Empire from Activities 1–4 is loaded — three upgrades, ``else if`` messages, a for loop calculating production, and the nested bonus multiplier are all there!

This is your **capstone activity**. You will add the final pieces to complete the game:
- A **prestige system** — once you reach the max level, reset with a permanent multiplier (complex branching)
- A **win condition** — reach the final goal to truly "complete" the empire
- A **splash screen** explaining the controls

Everything you built across four activities comes together here!

This activity covers **AC9TDI6P02** and **AC9TDI6P05**.

## Step 1 — Add prestige variables

In ``||loops:on start||``, add these new variables:

| Variable | Starting value | Purpose |
|----------|---------------|---------|
| ``prestigeLevel`` | 0 | How many times the player has prestiged |
| ``prestigeMultiplier`` | 1 | Permanent production bonus from prestige |
| ``cookieGoal`` | 10000 | Cookies needed to prestige |

```blockconfig.local
let prestigeLevel = 0
let prestigeMultiplier = 1
let cookieGoal = 10000
```

```blocks
let prestigeLevel = 0
let prestigeMultiplier = 1
let cookieGoal = 10000
```

## Step 2 — Apply prestige to production

In the ``||game:on game update every 1000 ms||`` block, update the production calculation to include both ``bonusMultiplier`` AND ``prestigeMultiplier``:

```blockconfig.local
cookiesPerSecond = total * bonusMultiplier * prestigeMultiplier
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
    cookiesPerSecond = total * bonusMultiplier * prestigeMultiplier
    cookies += cookiesPerSecond
    info.setScore(cookies)
})
```

## Step 3 — The Prestige system (complex branching)

Add a ``||controller:on left button pressed||`` event. This handles the prestige action.

The algorithm (design this on paper first!):
1. Check ``if prestigeLevel < 3`` (max 3 prestiges)
2. Inside that: check ``if cookies >= cookieGoal``
3. If both true: reset cookies and upgrades, increase prestigeLevel and prestigeMultiplier, double the goal
4. Else if prestigeLevel < 3 but not enough cookies: show progress message
5. Else (prestigeLevel >= 3): show "Empire Complete!" message

```blocks
controller.left.onEvent(ControllerButtonEvent.Pressed, function () {
    if (prestigeLevel < 3) {
        if (cookies >= cookieGoal) {
            prestigeLevel += 1
            prestigeMultiplier = prestigeLevel + 1
            cookies = 0
            grandmas = 0
            farms = 0
            factories = 0
            cookieGoal = cookieGoal * 2
            info.setScore(cookies)
            music.play(music.melodyPlayable(music.powerUp), music.PlaybackMode.UntilDone)
            game.showLongText("PRESTIGE " + prestigeLevel + "! Production x" + prestigeMultiplier + "!", DialogLayout.Full)
        } else {
            game.showLongText("Need " + cookieGoal + " cookies to prestige!", DialogLayout.Bottom)
        }
    } else {
        game.showLongText("You have reached the maximum prestige level!", DialogLayout.Full)
    }
})
```

## Step 4 — Win condition

Add a final win condition in the update loop. The player wins when they have **prestigeLevel = 3** and **cookies >= 50000** (the final empire goal).

```blockconfig.local
if (prestigeLevel >= 3 && cookies >= 50000) {
    game.over(true, effects.confetti)
}
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
    cookiesPerSecond = total * bonusMultiplier * prestigeMultiplier
    cookies += cookiesPerSecond
    info.setScore(cookies)
    if (prestigeLevel >= 3 && cookies >= 50000) {
        game.over(true, effects.confetti)
    }
})
```

## Step 5 — Display loop: show upgrade summary

Use the start of a game to show controls. In ``||loops:on start||``, add a ``||game:splash||`` screen explaining the controls:

```blocks
game.splash("A: Bake  B: Grandma  Up: Farm  Down: Factory  Left: Prestige!")
```

Then add a second ``||game:on game update every 5000 ms||`` (every 5 seconds) that shows a status summary. Use a for loop to build a summary string:

```blocks
game.onUpdateInterval(5000, function () {
    let summary = "G:" + grandmas + " F:" + farms + " Fac:" + factories + " CPS:" + cookiesPerSecond
    game.showLongText(summary, DialogLayout.Top)
})
```

## Step 6 — Final test: complete playthrough

Play your complete Cookie Empire and verify all systems work together:

1. Bake cookies → auto-bake starts → buy grandmas, farms, factories
2. Reach 10 grandmas + 5 farms → verify the 4× multiplier activates
3. Bake 10,000 cookies → press Left to prestige
4. Verify: cookies reset, ``prestigeMultiplier`` = 2, everything costs the same but production doubles
5. Prestige twice more → final win at 50,000 cookies on prestige 3

**Trace the prestige algorithm:** On your third prestige (``prestigeLevel = 2``), what happens when you press Left?
- Outer if: 2 < 3 ✓
- Inner if: cookies >= cookieGoal?
- If yes: prestigeLevel becomes 3, multiplier becomes 4, cookies reset ✓

## Cookie Empire Complete! @showdialog

**You have built Cookie Empire — an incredible achievement!**

Here is everything you accomplished across all five activities:

| Concept | Activity | Where used |
|---------|----------|-----------|
| **Variables** (multiple) | 1 | 6+ variables tracking game state |
| **Simple if/else** | 1 | Buying upgrades |
| **Multiple alternatives (else if)** | 2 | 3-way feedback messages |
| **AND / OR conditions** | 2 | Synergy bonus check |
| **For loops** | 3 | Production calculation across upgrade types |
| **Nested if/else** | 4 | 4-outcome bonus multiplier |
| **Complex combined branching + iteration** | 5 | Prestige system, win condition |

**Australian Curriculum:**
- **AC9TDI6P02:** You designed algorithms involving multiple alternatives (branching) and iteration
- **AC9TDI6P05:** You implemented those algorithms as visual programs involving control structures, variables and input

Collect your **Cookie Empire Certificate** and show your teacher!
