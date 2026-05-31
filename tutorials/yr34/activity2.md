# Click to Bake

## Welcome back! @showdialog

Your code from Activity 1 is already loaded — you can see your cookie sprite on screen!

In this activity you will **add new blocks** to make the cookie respond to button presses.

You will:
- Add a **cookiesPerClick** variable
- Make the **A button** bake cookies when pressed
- Update the score display each time you bake
- Add a fun effect to celebrate each click

Pressing the **A key** on your keyboard (or the A button on a controller) will be your "click"!

## Step 1 — Add a cookiesPerClick variable

We want to track how many cookies each press earns. Later we can upgrade this to earn more per click!

Open **Variables**, make a new variable called ``cookiesPerClick``, and set it to **1** inside ``||loops:on start||``.

```blockconfig.local
let cookiesPerClick = 1
```

```blocks
scene.setBackgroundColor(3)
let cookies = 0
let cookiesPerClick = 1
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

## Step 2 — Add a button event

An **event** is something that runs when something happens. We want code to run when the player presses the A button.

Find ``||controller:on A button pressed||`` in the **Controller** drawer. Drag it out — it will sit *beside* your ``||loops:on start||`` block, not inside it.

```blockconfig.local
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
})
```

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
})
```

## Step 3 — Add cookies when the button is pressed

Inside the ``||controller:on A button pressed||`` event, we need to:
1. Add ``cookiesPerClick`` to our ``cookies`` variable
2. Update the score on screen

From **Variables**, drag ``||variables:change cookies by 1||`` inside the event. Change the **1** to the ``cookiesPerClick`` variable block.

Then add ``||info:set score to||`` below it and set the value to the ``cookies`` variable.

```blockconfig.local
cookies += cookiesPerClick
info.setScore(cookies)
```

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += cookiesPerClick
    info.setScore(cookies)
})
```

## Step 4 — Add a fun effect!

Let's make the cookie look like it's being pressed! Find ``||sprites:cookie start effect spray||`` in the **Sprites** drawer and add it inside the event.

You can also try other effects — look for ``confetti``, ``hearts``, or ``spray``!

```blockconfig.local
cookie.startEffect(effects.spray, 200)
```

```blocks
controller.A.onEvent(ControllerButtonEvent.Pressed, function () {
    cookies += cookiesPerClick
    info.setScore(cookies)
    cookie.startEffect(effects.spray, 200)
})
```

## Step 5 — Test your game!

Press the **Play** button and try pressing **A** (or **Space** on your keyboard).

Watch the score go up each time! Try pressing A many times really fast.

Can you get to 20 cookies?

## Great baking! @showdialog

Your cookie clicker is working!

**What you built:**
- A ``cookiesPerClick`` variable
- An ``on A button pressed`` event — this runs code when something happens
- The score updates every time you press A
- A satisfying effect on each bake

**Coming up:** In Activity 3, we will add an *upgrade* you can buy — but only if you have enough cookies. That means your code will need to **make a decision**. That is called **branching**!
