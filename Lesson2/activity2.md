### @explicitHints 1

# Activity: Moving the agent to a coordinate.

## Step 3
To get started, we want to add our ``||Agent: teleport to player||`` in our ``||Loops: on start||``.

### ~ tutorialhint
```blocks
	agent.teleportToPlayer()
```

## Step 4
Next, let's add our agent to our ``||Player: on chat command||``. Let's create a ``||Agent: teleport||``

### ~ tutorialhint
```blocks
player.onChat("run", function () {
    agent.teleport(pos(0, 0, 0), WEST)
})
```

## Step 5
Next, let's create a three ``||variable||`` and call them, **X**, **Y**, **Z**

### ~ tutorialhint
```blocks
player.onChat("run", function () {
	x = 0
	y = 0
	z = 0
    agent.teleport(pos(0, 0, 0), WEST)
})
```

## Step 6
Now, let's set them to be equal to a random number like we did yesterday between **2** and **6**.

### ~ tutorialhint
Use ``||Math: pick random||`` for each variable.

*Example:*
```blocks
	variable = randint(2, 6)
```

## Step 7
Then, set the coorindate to the variables we selected

### ~ tutorialhint
```blocks
player.onChat("run", function () {
	x = randint(2, 6)
	y = randint(2, 6)
	z = randint(2, 6)
    agent.teleport(pos(x, y, z), WEST)
})
```

## Step 4
Hit run. What do you notice happens when you run the code?
