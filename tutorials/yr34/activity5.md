# Cookie Champion

## Almost there! @showdialog

Your complete game from Activities 1–4 is loaded and ready — clicking, upgrades, and auto bakers all working!

You have learned two big programming ideas:

- **Branching** (if/else) — your code makes decisions
- **Iteration** (loops) — your code repeats actions

In this final activity, you will **complete the game** by adding:
- A **goal** — 500 cookies to win!
- A win condition check inside the loop (**branching inside iteration**)
- A splash screen and polish to make it feel finished!

## Step 1 — Set a goal variable

In ``||loops:on start||``, create a new variable called ``goal`` and set it to **500**.

This is how many cookies the player needs to win.

```blockconfig.local
let goal = 500
```

```blocks
scene.setBackgroundColor(3)
let cookies = 0
let cookiesPerClick = 1
let upgradeCost = 10
let autoBakers = 0
let autoBakerCost = 50
let goal = 500
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

## Step 2 — Check for win inside the loop

Open your ``||game:on game update every 1000 ms||`` block.

After the auto baker code, add **another** ``||logic:if||`` block:

**if cookies >= goal** — then call ``||game:game over WIN||``

Also add a confetti effect to make it feel amazing: ``||game:game over WIN effect confetti||`` (look for the + button on the game over block to add an effect).

```blockconfig.local
if (cookies >= goal) {
    game.over(true, effects.confetti)
}
```

```blocks
game.onUpdateInterval(1000, function () {
    if (autoBakers > 0) {
        cookies += autoBakers
        info.setScore(cookies)
    }
    if (cookies >= goal) {
        game.over(true, effects.confetti)
    }
})
```

## Step 3 — Show progress to the player

It helps players know how close they are to winning. Let's add a **countdown** label.

Add a ``||game:on game update every 1000 ms||`` (or add inside your existing one):

Use ``||game:show long text||`` to display: ``"Goal: " + goal + " cookies"`` — but only show this at the start. You can display a ``splash`` screen at the start using ``||game:splash||``.

Add a ``||game:splash||`` block inside ``||loops:on start||`` after all your setup:

```blocks
game.splash("Bake " + goal + " cookies to win! Press A to bake.")
```

## Step 4 — Upgrade the click sound

Update your ``||controller:on A button pressed||`` event to play a sound when clicking:

Add ``||music:play tone Middle C for 1 beat||`` or ``||music:play melody ba ding||`` inside the A button event for extra feedback.

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += cookiesPerClick
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
    music.play(music.melodyPlayable(music.baDing), music.PlaybackMode.InBackground)
})
```

## Step 5 — Play your complete game!

Press **Play** and try to reach 500 cookies!

**Strategy tips:**
- Upgrade your click first (press B after 10 cookies)
- Then save up for auto bakers (press Up after 50 cookies)
- Combine both — more auto bakers AND more cookies per click!

**Think about it:** Can you trace the full algorithm?
1. On start: set up sprites and variables (sequence)
2. On A pressed: bake cookies (event + branching for upgrade)
3. On B pressed: try to buy upgrade (branching)
4. On Up pressed: try to buy auto baker (branching)
5. Every second: auto bake + check for win (iteration + branching)

## You are a Cookie Champion! @showdialog

**Congratulations! You built a complete Cookie Clicker game!**

Here is what you accomplished:

| Concept | Where you used it |
|---------|------------------|
| **Sequence** | The steps in ``on start`` run in order |
| **Variables** | ``cookies``, ``cookiesPerClick``, ``autoBakers``, ``goal`` |
| **Events** | ``on A pressed``, ``on B pressed``, ``on Up pressed`` |
| **Branching** | ``if/else`` blocks for upgrades and win checking |
| **Iteration** | ``on game update every 1000ms`` loops automatically |

**Australian Curriculum (AC9TDI4P02):** You followed, described, and *implemented* an algorithm involving sequencing, branching, and iteration as a visual program. Well done!

Collect your **Certificate** and show your teacher!
