# Upgrade Time!

```template
let cookies = 0
let cookiesPerClick = 1
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
info.setScore(0)
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += cookiesPerClick
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
```

## What is Branching? @showdialog

Your code from Activities 1 and 2 is already loaded — you can click the cookie and watch the score go up!

Now it's time to add an **upgrade shop**. But before a player can buy an upgrade, your program needs to **make a decision**: does the player have enough cookies?

Imagine a fork in the road with a sign: **"If you have a key, go left. Otherwise, go right."**

That is **branching** — your program takes a different path depending on whether something is true or false.

> **if** *you have enough cookies* **then** buy the upgrade
> **else** show a message saying "not enough cookies!"

In this activity you will:
- Add an **upgrade** that costs 10 cookies
- Use an ``||logic:if/else||`` block to decide what happens
- Learn to read comparison operators like **>=** (greater than or equal to)

This is **AC9TDI4P02** — branching!

## Step 1 — Add upgrade variables

We need two new variables: the cost of the upgrade and how many cookies we earn per click.

In ``||loops:on start||``, make sure ``cookiesPerClick`` is already set to ``1``.

Add a new variable ``upgradeCost`` and set it to **10**.

```blockconfig.local
let upgradeCost = 10
```

```blocks
scene.setBackgroundColor(3)
let cookies = 0
let cookiesPerClick = 1
let upgradeCost = 10
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

## Step 2 — Add an upgrade sprite

Let's show a small "upgrade" button on the right side of the screen so players know they can buy something.

Create a new sprite. Draw a simple star or coin shape (or use yellow circles). Call it ``upgradeButton``.

Position it at **x: 140, y: 40**.

```blocks
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
```

## Step 3 — Add a B button event

Add a new ``||controller:on B button pressed||`` event. This will handle buying the upgrade. It lives beside your other blocks.

```blockconfig.local
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
})
```

```blocks
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
})
```

## Step 4 — The if/else decision (BRANCHING!)

This is the key step! We need our code to ask:
**"Does the player have enough cookies?"**

Inside the ``||controller:on B button pressed||`` event, add an ``||logic:if true then else||`` block from the **Logic** drawer.

In the **condition** slot (where it says ``true``), drag in a comparison block: ``||logic:0 >= 0||``. Change the first **0** to the ``cookies`` variable and the second **0** to ``upgradeCost``.

This reads as: **"if cookies are greater than or equal to upgradeCost"**

```blockconfig.local
if (cookies >= upgradeCost) {
} else {
}
```

```blocks
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= upgradeCost) {
    } else {
    }
})
```

## Step 5 — The TRUE branch (can afford)

Inside the **if** (top) section, add the code for when the player CAN afford the upgrade:

1. Subtract ``upgradeCost`` from ``cookies``
2. Add 1 to ``cookiesPerClick``
3. Update the score display
4. Play a sound — find ``||music:play melody power up||`` in the **Music** drawer

```blockconfig.local
cookies -= upgradeCost
cookiesPerClick += 1
info.setScore(cookies)
music.play(music.melodyPlayable(music.powerUp), music.PlaybackMode.UntilDone)
```

```blocks
controller.B.onEvent(ControllerButtonEvent.Pressed, function () {
    if (cookies >= upgradeCost) {
        cookies -= upgradeCost
        cookiesPerClick += 1
        info.setScore(cookies)
        music.play(music.melodyPlayable(music.powerUp), music.PlaybackMode.UntilDone)
    } else {
    }
})
```

## Step 6 — The FALSE branch (cannot afford)

Inside the **else** (bottom) section, add the code for when the player **cannot** afford it:

Find ``||game:show long text "" bottom||`` in the **Game** drawer. Type a message like: ``"Not enough cookies! Keep baking!"``

```blockconfig.local
game.showLongText("Not enough cookies! Keep baking!", DialogLayout.Bottom)
```

```blocks
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

## Step 7 — Test your branching!

Press **Play** and test both paths:

1. Press **B** before you have 10 cookies — what happens? (the ELSE branch)
2. Bake 10 cookies by pressing **A** ten times
3. Press **B** again — what happens now? (the IF branch)

Your ``cookiesPerClick`` goes up, so you earn more cookies per press!

**Think about it:** Can you trace the path your program takes in each case?

## You used branching! @showdialog

Amazing work! You just wrote code that **makes decisions**!

**What you built:**
- An ``if/else`` block that chooses between two paths
- A comparison (``>=``) that checks if you can afford the upgrade
- Two different outcomes depending on the result

**What this means in the Australian Curriculum (AC9TDI4P02):** You followed and implemented an algorithm with *branching* — your program takes different actions depending on a condition.

**Next up:** Activity 4 — you will make cookies bake *automatically* using a **loop** (iteration)!
