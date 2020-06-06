# Infinite SVG Triangle Fusion

A Pen created on CodePen.io. Original URL: [https://codepen.io/robdimarzo/pen/VqjvqR](https://codepen.io/robdimarzo/pen/VqjvqR).

Triangles are created. Triangles are destroyed. And so on and so forth.

##What's going on here?
In this pen, I am creating 60 SVGs that each contain 4 triangles (polygons). Each polygon loops through a color and animates outward from the center point of its parent SVG every 1 second. The entire animation repeats infinitely every 4 seconds. 

##How are the triangles combining?
Each div has a clip-path to create a hexagon mask. When the hexagons are snapped together, the expanding triangles bleed evenly into the triangles of the adjacent hexagons until they disappear.

## How are the hexagons connected?
I used CSS Grid as a starting point, but I was still left with a bunch of well-mannered hexagons with empty space in between. To "connect" the hexagons, I identified the nth-children that corresponds to a row and moved them up and over via transform: translate;

Source:

The inspiration for this pen is an animation by Erica Anderson (GIF available in the link below). I was mesmerized and compelled to create something similar via SVG:  https://giphy.com/gifs/trippy-weird-psychedelic-xUOxeZR9gmFzbH8FRS
