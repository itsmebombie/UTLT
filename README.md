# uTLFN
some kinda useful functions that arent in spwn v.0.7 and under

# functions
`random` - pseudo random number generator

`math` - some math functions such as `clamp`, `lerp`, `round` (which can also round with decimals) and others

`sine_terrain` - generates a 1d terrain using sine and lerp functions (also outputs the raw points without any interpolation for later modifications)

`bulk_add_objects` - adds blocks in bulk which will probably recieve more updates later

# docs
## random
`random.next(max: @number = 2^32)` - returns the next random integer

`random.next_float(accuracy: @number = 2^32)` - returns the next random float

`random.set_seed(seed: @number)` - sets the seed to the recieved arg

`random.get_seed()` - returns the current seed

## math
`math.clamp(number: @number, min: @number = 0, max: @number = 1)` - clamps the given number between 2 values

`math.wrap(number: @number, min: @number = 0, max: @number = 1)` - wraps the given number between 2 values

`math.lerp(a: @number, b: @number, f: @number = 0.5)` - gets the value(f) between 2 numbers (a,b) (linear interpolation)

`math.cerp(y0: @number, y1: @number, y2: @number, y3: @number, mul: @number = 1)` - idk how it works you can search it on google (cubic interpolation)

`math.round(number: @number, decimal_places: @number = 0)` - like the normal round function but it can also round to decimal places

## others
`sine_terrain(seed: @number, res: @number, intensity: @number = 2, lerpamt: @number = 8)` - generates a 1d terrain using sine and lerp functions (also outputs the raw points without any interpolation for later modifications)

`bulk_objects(array: @array, start_x: @number = 0, start_y: @number = 0, obj_id: @number = 1)` - adds blocks in bulk which will probably recieve more updates later (array structure is literally just the y position of the block, example: `[0,0,0,1,2,2,2,3,3,3,3,2,2,1,1,1,1,1,1,0]` cringe ikr)


