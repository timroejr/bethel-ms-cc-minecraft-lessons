### @explicitHints 1

# Activity: Place a random block under our feet

## Step 1

Let's get started by placing a ``||Loops: forever||`` block

# ~ tutorialHint
```blocks
	loops.forever(function () {
	})
```

## Step 2

Next let's add a  ``||Blocks: place||``

# ~ tutorialHint
```blocks
loops.forever(function () {
    blocks.place()
})
```

## Step 3

Next, we'll want to create a variable called ``||Variable: block||`` and set it to be a ``||Math: pick random||`` between 12 and 25.

# ~ tutorialHint
```blocks
loops.forever(function () {
    block = randint(12, 25)
    blocks.place()
})
```

## Step 4

Then let's update our block placement. Let's place a block by an **id** and at the ground. It should look like...
```blocks
loops.forever(function () {
    block = randint(12, 25)
    blocks.place(blocks.blockById(block), positions.groundPosition(player.position()))
})
```

## Step 5
Run the code and walk around on the glass. What happens?