### @explicitHints 1

# Activity: Random Number Spawning

## Step 1
Let's create a circle in the air of diamond blocks, and each time we run our command it is a different size.

## Step 2
Let's create a new event to do our work. Drag the ``||Player: on chat command||`` block into the workspace.

### ~ tutorialhint

```blocks
	player.onChat("circle", function () {

	})
```

## Step 3
Next let's create a new ``||variable||`` and call it **size**

### ~ tutorialhint

```blocks
player.onChat("circle", function () {
    size = 0

})
```

## Step 4
Let's set our variable to be a random number. Go and find a ``||Math: pick random||`` and pick a number between **5** and **10**

## Step 4
Go to our ``||Shapes||`` and let's grab ``||Shapes: circle of||`` and add it below the new variable we created. **IMPORTANT: Make sure you set your "around" to be "y (Up/Down)"**

### ~ tutorialhint

```blocks
player.onChat("circle", function () {
    size = randint(5, 10)
    shapes.circle(
    GRASS,
    pos(0, 0, 0),
    5,
    Axis.Y,
    ShapeOperation.Replace
    )
})
```

## Step 5
Next, let's set our block to be diamond and our radius to be the variable we created.

### ~ tutorialhint
Go to ``||Variables||`` and select the variable **size** and put it in our radius. You can change the block using the dropdown menu.

## Step 6
Finally, click run, what happens when you walk around and type **circle** circle in the chat?

