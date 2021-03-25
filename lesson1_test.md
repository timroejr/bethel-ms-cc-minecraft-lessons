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
Let's create a new ```variable:new variable``` called **times**. Then, set it to be equal to **5**.

### ~ tutorialhint
```blocks
	let times = 0
	player.onChat("spawn", function () {
		times = 5
	})
```

## Step 3
Now we want to loop through the amount of times we specified. Let's use the variable to loop.

### ~ tutorialhint
```blocks
	let times = 5
	player.onChat("spawn", function () {
		times = 5
		for (let index = 0; index < times; index++) {
			
		}
	})
```

## Step 4
Finally let's add a Mob Spawner by adding some chickens.

### ~ tutorialhint
```blocks
	let times = 5
	player.onChat("spawn", function () {
		times = 5
		for (let index = 0; index < times; index++) {
			mobs.spawn(CHICKEN, pos(0, 0, 0))
		}
	})
```