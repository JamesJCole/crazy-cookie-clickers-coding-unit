# Build the Shop

## Welcome to Cookie Empire! @showdialog

This is the **Year 5/6** track — a more complex challenge designed to push your thinking!

In Cookie Empire you will design and build a full upgrade shop. Instead of one upgrade, you will have **three** (Grandma, Farm, and Factory), each with their own variables and costs.

In this first activity you will:
- Set up all your game variables
- Create the cookie sprite and score display
- Add basic clicking
- Build your first two upgrade purchases using simple ``if`` conditions

By the end of all five activities you will have a complete Cookie Empire game!

**Before you code:** On paper (or in your head), think about this:
- What variables will you need to track three different upgrades?
- What information does the player need to see on screen?

## Step 1 — Set up all variables

A more complex game needs more variables. In ``||loops:on start||``, set up these variables:

| Variable | Starting value |
|----------|---------------|
| ``cookies`` | 0 |
| ``grandmas`` | 0 |
| ``farms`` | 0 |
| ``grandmaCost`` | 15 |
| ``farmCost`` | 100 |
| ``cookiesPerSecond`` | 0 |

```blockconfig.local
let cookies = 0
let grandmas = 0
let farms = 0
let grandmaCost = 15
let farmCost = 100
let cookiesPerSecond = 0
```

```blocks
let cookies = 0
let grandmas = 0
let farms = 0
let grandmaCost = 15
let farmCost = 100
let cookiesPerSecond = 0
```

## Step 2 — Set up the scene and cookie sprite

Set a background colour and create your cookie sprite. Centre it on screen at **x: 70, y: 60**.

Also add ``||info:set score to 0||`` to show the cookie count.

```blocks
scene.setBackgroundColor(3)
let cookies = 0
let grandmas = 0
let farms = 0
let grandmaCost = 15
let farmCost = 100
let cookiesPerSecond = 0
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
```

## Step 3 — Basic clicking

Add an ``||controller:on A button pressed||`` event. Each press adds **1** to ``cookies`` and updates the score.

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += 1
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
```

## Step 4 — Buy a Grandma (B button)

Grandmas are the cheapest upgrade — they each produce 1 cookie per second.

Add a ``||controller:on B button pressed||`` event. Inside it, add an ``||logic:if||`` to check ``cookies >= grandmaCost``.

If true:
- Subtract ``grandmaCost`` from ``cookies``
- Add 1 to ``grandmas``
- Increase ``cookiesPerSecond`` by 1
- Make the next grandma cost more (multiply by **1.15** and round)
- Update the score

If false: show a message with the cost.

```blocks
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= grandmaCost) {
        cookies -= grandmaCost
        grandmas += 1
        cookiesPerSecond += 1
        grandmaCost = Math.round(grandmaCost * 1.15)
        info.setScore(cookies)
    } else {
        game.showLongText("Grandma costs " + grandmaCost + " cookies!", DialogLayout.Bottom)
    }
})
```

## Step 5 — Buy a Farm (Up button)

Farms produce 8 cookies per second each — but cost much more.

Add a ``||controller:on up button pressed||`` event with a similar if/else structure.

If true:
- Subtract ``farmCost`` from ``cookies``
- Add 1 to ``farms``
- Increase ``cookiesPerSecond`` by **8**
- Multiply ``farmCost`` by **1.15** and round
- Update score

```blocks
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= farmCost) {
        cookies -= farmCost
        farms += 1
        cookiesPerSecond += 8
        farmCost = Math.round(farmCost * 1.15)
        info.setScore(cookies)
    } else {
        game.showLongText("Farm costs " + farmCost + " cookies!", DialogLayout.Bottom)
    }
})
```

## Step 6 — The automatic baking loop

Add a ``||game:on game update every 1000 ms||`` loop.

Inside it, check ``if cookiesPerSecond > 0``, then add ``cookiesPerSecond`` to ``cookies`` and update the score.

```blocks
game.onUpdateInterval(1000, function () {
    if (cookiesPerSecond > 0) {
        cookies += cookiesPerSecond
        info.setScore(cookies)
    }
})
```

## Step 7 — Test your shop!

Press **Play** and try both upgrades:
- Bake 15 cookies and buy a grandma (B)
- Bake 100 cookies and buy a farm (Up)
- Watch the auto-baking get faster as you buy more!

**Notice:** The grandma cost goes up after each purchase. Why is that a good game design decision?

## Your shop is open! @showdialog

**Excellent start!** You have built the foundation of Cookie Empire.

**What you built:**
- Six variables tracking multiple game states
- Two upgrades with different costs and production rates
- An automatic baking loop

**Coming up:** In Activity 2, you will replace the simple ``if/else`` with ``else if`` chains — that is how you handle **multiple alternatives** in code!
