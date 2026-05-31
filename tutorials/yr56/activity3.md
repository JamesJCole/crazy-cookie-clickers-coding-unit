# Cookie Factory

## Iteration with For Loops @showdialog

So far, your ``cookiesPerSecond`` variable gets updated every time you buy an upgrade. But what if you wanted to *recalculate* the total production from scratch each second?

That is where a **for loop** becomes powerful. A for loop repeats code a set number of times, working through a list of items one by one.

```
for i = 0, 1, 2:
    total = total + production[i] × count[i]
```

In this activity you will:
- Replace the manual ``cookiesPerSecond`` updates with a **for loop** that recalculates production each second
- Understand how a **loop variable** (``i``) counts through a list
- See how loops make it easy to add more upgrades without rewriting lots of code

This is **AC9TDI6P02** — iteration — and **AC9TDI6P05** — implementing algorithms with variables!

## Step 1 — Algorithm design on paper first

**Before coding**, sketch this algorithm:

> We have 3 upgrade types. Each has a *count* (how many you own) and a *rate* (cookies per second each produces).
> Every second, loop through all 3 types and add (count × rate) to total production.

Upgrade rates:
- Grandma: **1** cookie/second each
- Farm: **8** cookies/second each
- Factory: **47** cookies/second each

Why does this design make it easy to add a 4th upgrade later?

## Step 2 — Remove the cookiesPerSecond updates from upgrade buttons

Now that we will calculate production in the loop, we no longer need to manually update ``cookiesPerSecond`` when buying upgrades.

Remove the ``cookiesPerSecond += 1`` line from the grandma (B button) handler.
Remove the ``cookiesPerSecond += 8`` line from the farm (Up button) handler.
Remove the ``cookiesPerSecond += 47`` line from the factory (Down button) handler.

Keep everything else in those handlers.

## Step 3 — The for loop

In your ``||game:on game update every 1000 ms||`` block, **replace** the ``cookiesPerSecond`` calculation with a for loop.

Find ``||loops:for index from 0 to 4||`` in the **Loops** drawer. Change the maximum to **2** (we have 3 items: index 0, 1, and 2).

```blockconfig.local
for (let i = 0; i <= 2; i++) {
}
```

```blocks
game.onUpdateInterval(1000, function () {
    let total = 0
    for (let i = 0; i <= 2; i++) {
    }
    cookies += total
    info.setScore(cookies)
})
```

## Step 4 — Calculate production inside the loop

Inside the for loop, we need to look up the count and rate for each upgrade based on ``i``:
- When ``i = 0``: Grandma (count = ``grandmas``, rate = 1)
- When ``i = 1``: Farm (count = ``farms``, rate = 8)
- When ``i = 2``: Factory (count = ``factories``, rate = 47)

Use ``||logic:if/else if||`` inside the loop to pick the right values:

```blockconfig.local
if (i == 0) {
    total += grandmas * 1
} else if (i == 1) {
    total += farms * 8
} else if (i == 2) {
    total += factories * 47
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
    cookies += total
    info.setScore(cookies)
})
```

## Step 5 — Add the synergy bonus back

After the for loop (but still inside the update block), add back the synergy bonus from Activity 2:

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
    cookies += total
    info.setScore(cookies)
    if (grandmas >= 5 && farms >= 3) {
        cookies += 10
    }
})
```

## Step 6 — Show CPS to the player

Use a ``||game:splash||`` at the start to explain controls, and add a display of cookies per second.

In the update loop, calculate and update an info display. You can use ``||info:set life to||`` creatively to display CPS, or use ``||game:show long text||`` occasionally. For now, calculate and store CPS in a variable:

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
    cookiesPerSecond = total
    cookies += cookiesPerSecond
    info.setScore(cookies)
    if (grandmas >= 5 && farms >= 3) {
        cookies += 10
    }
})
```

## Step 7 — Test the for loop

Press **Play** and verify:
1. Buying grandmas, farms, and factories still works
2. Cookies increase automatically each second
3. Try mixing multiple upgrade types — does your CPS total correctly?

**Trace the loop manually:** If you have 3 grandmas, 1 farm, and 0 factories, what does the loop calculate?
- i=0: 3 × 1 = 3
- i=1: 1 × 8 = 8
- i=2: 0 × 47 = 0
- Total = 11 cookies/second ✓

## Challenge: Add a 4th upgrade

Can you add a **Mine** (200 cookies/second each, starting cost 5000) using the Down button or another button? Notice that you only need to:
1. Add new variables
2. Add a buy handler
3. Change ``2`` to ``3`` in the for loop and add one more ``else if``

How does the for loop design make adding new upgrades easier?

## For loops mastered! @showdialog

**Outstanding work!**

**What you built:**
- A for loop that iterates through all upgrade types
- Branching inside the loop to pick the right upgrade
- A clean, extensible production calculation

**What this means (AC9TDI6P02 + AC9TDI6P05):** You designed and implemented an algorithm using *iteration* — your loop processes multiple items in sequence — and *variables* to track state across loop iterations.

**Next up:** Activity 4 — you will combine **nested if/else** with loops to create Cookie Multipliers!
