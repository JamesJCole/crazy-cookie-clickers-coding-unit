# Auto Baker

## What is Iteration? @showdialog

Imagine a factory machine that stamps out cookies once every second, forever, without stopping.

That is **iteration** (also called a **loop**) — code that runs **again and again**, repeating its actions.

In this activity you will:
- Add an ``autoBakers`` variable to track your automatic bakers
- Add a button to buy an auto baker
- Use a ``||game:on game update every||`` block — a loop that runs every second
- Inside the loop, check **if** any auto bakers are working, then add cookies

This combines **branching** AND **iteration** — both from AC9TDI4P02!

## Step 1 — Add the autoBakers variable

In ``||loops:on start||``, create a new variable called ``autoBakers`` and set it to **0**.

Also add a variable ``autoBakerCost`` and set it to **50**.

```blockconfig.local
let autoBakers = 0
let autoBakerCost = 50
```

```blocks
scene.setBackgroundColor(3)
let cookies = 0
let cookiesPerClick = 1
let upgradeCost = 10
let autoBakers = 0
let autoBakerCost = 50
let cookie = sprites.create(img`
    . . . . 4 4 4 4 4 4 4 4 . . . .
    . . 4 4 4 4 4 4 4 4 4 4 4 4 . .
    . 4 4 4 4 4 e 4 4 4 4 4 4 4 4 .
    . 4 4 4 4 4 4 4 4 4 e 4 4 4 4 .
    4 4 4 e 4 4 4 4 4 4 4 4 4 4 4 4
    4 4 4 4 4 4 4 4 4 4 4 4 4 4 4 4
    4 4 4 4 4 4 4 e 4 4 4 4 4 e 4 4
    4 4 4 4 4 4 4 4 4 4 4 4 4 4 4 4
    4 4 e 4 4 4 4 4 4 4 4 4 4 4 4 4
    4 4 4 4 4 4 4 4 4 4 4 4 e 4 4 4
    4 4 4 4 4 4 4 4 e 4 4 4 4 4 4 4
    4 4 4 e 4 4 4 4 4 4 4 4 4 4 4 4
    . 4 4 4 4 4 4 4 4 4 4 4 4 4 4 .
    . 4 4 4 4 4 4 4 4 4 4 e 4 4 4 .
    . . 4 4 4 4 4 4 4 4 4 4 4 4 . .
    . . . . 4 4 4 4 4 4 4 4 . . . .
`, SpriteKind.Player)
cookie.setPosition(80, 60)
info.setScore(0)
```

## Step 2 — Add a buy auto baker button

We need a way to buy an auto baker. Let's use the **Up** button on the controller (the Up arrow key on a keyboard).

Add a new ``||controller:on up button pressed||`` event.

Inside it, add an ``||logic:if/else||`` block that checks: **if cookies >= autoBakerCost**.

```blockconfig.local
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= autoBakerCost) {
    } else {
    }
})
```

```blocks
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= autoBakerCost) {
    } else {
    }
})
```

## Step 3 — Buy the auto baker

Inside the **if** branch (when the player can afford it):
1. Subtract ``autoBakerCost`` from ``cookies``
2. Add **1** to ``autoBakers``
3. Update the score
4. Make the cost go up a little (multiply by 1.5 and round — find ``||math:round||`` in the Math drawer)

```blocks
controller.up.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= autoBakerCost) {
        cookies -= autoBakerCost
        autoBakers += 1
        info.setScore(cookies)
        autoBakerCost = Math.round(autoBakerCost * 1.5)
    } else {
        game.showLongText("Need " + autoBakerCost + " cookies for an auto baker!", DialogLayout.Bottom)
    }
})
```

## Step 4 — The loop! (ITERATION)

Here comes the important part — the **loop**!

Find ``||game:on game update every 500 ms||`` in the **Game** drawer. Drag it out as a new block. Change the time to **1000** milliseconds (1 second).

This block runs its code **every 1 second**, automatically, forever. That is **iteration** — your code repeats!

```blockconfig.local
game.onUpdateInterval(1000, function () {
})
```

```blocks
game.onUpdateInterval(1000, function () {
})
```

## Step 5 — Bake inside the loop

Inside the ``||game:on game update every 1000 ms||`` block, add an ``||logic:if||`` block:

**if autoBakers > 0** — then add ``autoBakers`` to ``cookies`` and update the score.

We use **if** here (branching inside iteration!) because we only want to add cookies if there are actually some auto bakers working.

```blockconfig.local
if (autoBakers > 0) {
    cookies += autoBakers
    info.setScore(cookies)
}
```

```blocks
game.onUpdateInterval(1000, function () {
    if (autoBakers > 0) {
        cookies += autoBakers
        info.setScore(cookies)
    }
})
```

## Step 6 — Test your auto baker!

Press **Play** and:

1. Bake **50 cookies** by pressing A many times
2. Press the **Up arrow** to buy an auto baker
3. Watch the score — it should go up by 1 every second automatically, without pressing anything!
4. Try buying 2 or 3 auto bakers — they all run at once in the loop!

**Think about it:** What happens inside the loop if ``autoBakers`` is 0? (Nothing — the if condition is false!)

## You used iteration! @showdialog

Incredible! Your bakery runs itself!

**What you built:**
- An ``on game update every 1000 ms`` block — a loop that repeats every second
- Branching inside the loop to only bake when auto bakers exist
- An upgrade purchase with another if/else check

**What this means in the Australian Curriculum (AC9TDI4P02):** You implemented an algorithm with *iteration* — your code repeats automatically. You also combined it with *branching* — the loop only does something when the condition is true.

**Next up:** Activity 5 — you will add a **win condition** and put everything together to complete your Cookie Clicker game!
