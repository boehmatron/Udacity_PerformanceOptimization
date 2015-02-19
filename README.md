# Changes I made...

## ... to images

* I compressed the images with a higher compression rate, so that 
they still look aweseome but use much less filessize and are 
faster to load.


## ... to changePizzaSizes()

* I put all queries that only needed to be done once out of the
for-loop and stored their values into variables.

* The for-loop now only iterates over the allPizzaContainers-
Array and sets the new width to all of them.


## ... to UpdatePositions()

* I again moved queries that needed only to be done once out
of the for-loop.

* The phase of the position of the pizzas is put in a separate
for-loop and loops from 0 to 4 and not through the whole item-
array

* The second for-loop iterates through all the items and modifies
their x-position by using "translateX" WebKitTransform wich is 
a much efficient way to move objects in the browser. Also the 
phase gets a reset every 4 loops.