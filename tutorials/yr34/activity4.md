# Auto Baker

```template
let cookies = 0
let cookiesPerClick = 1
let upgradeCost = 10
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
cookie.setPosition(80, 60)
let upgradeButton = sprites.create(img`
    . . . . . . . . . . . . . . . .
    . . . . . 5 5 5 5 5 5 . . . . .
    . . . . 5 5 5 5 5 5 5 5 . . . .
    . . . 5 5 5 1 1 1 1 5 5 5 . . .
    . . 5 5 5 1 5 5 5 5 1 5 5 5 . .
    . . 5 5 5 1 5 5 5 5 1 5 5 5 . .
    . . 5 5 5 5 1 1 1 1 5 5 5 5 . .
    . . 5 5 5 5 5 5 5 5 5 5 5 5 . .
    . . 5 5 5 5 5 5 5 5 5 5 5 5 . .
    . . . 5 5 5 5 5 5 5 5 5 5 . . .
    . . . . 5 5 5 5 5 5 5 5 . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
    . . . . . . . . . . . . . . . .
`, SpriteKind.Food)
upgradeButton.setPosition(140, 40)
info.setScore(0)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += cookiesPerClick
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= upgradeCost) {
        cookies -= upgradeCost
        cookiesPerClick += 1
        info.setScore(cookies)
        music.play(music.melodyPlayable(music.powerUp), music.PlaybackMode.UntilDone)
    } else {
        game.showLongText("Not enough cookies! Keep baking!", DialogLayout.Bottom)
    }
})
```

## What is Iteration? @showdialog

Your code from Activities 1–3 is already loaded — you have a clickable cookie and a working upgrade system!

Now let's take it to the next level: what if the game baked cookies **automatically**, without the player pressing anything?

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
