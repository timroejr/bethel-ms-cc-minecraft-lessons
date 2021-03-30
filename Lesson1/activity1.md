### @explicitHints 1

# Activity: Random Number Spawning

## Step 1
Let's create a new event to do our work. Drag the ``||Player: on chat command||`` block into the workspace.

### ~ tutorialhint
```blocks
		player.onChat("spawn", function () {
})
```

## Step 2
Let's create a new ```variable:new variable``` called **times**. Then, set it to be equal to **0**.

### ~ tutorialhint
```blocks
	player.onChat("spawn", function () {
		times = 0
	})
```

## Step 3
Let's set up our code so we get a random number between **5** and **10**

### ~ tutorialhint
```blocks
	player.onChat("spawn", function () {
		times = randint(5, 10)
	})
```

## Step 3
Now we want to loop through the amount of times we specified. Let's use the variable to loop.

### ~ tutorialhint
```blocks
	player.onChat("spawn", function () {
		times = randint(5, 10)
		for (let index = 0; index < times; index++) {
			
		}
	})
```

## Step 4
Finally let's add a Mob Spawner by adding some chickens.

### ~ tutorialhint
```blocks
	player.onChat("spawn", function () {
		times = randint(5, 10)
		for (let index = 0; index < times; index++) {
			mobs.spawn(CHICKEN, pos(0, 0, 0))
		}
	})
```