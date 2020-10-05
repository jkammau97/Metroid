# Metroid
Goal: Make a Metroid in Onshape

## Table of contents
- [Planning](#Planning)
- [Picture_Sketching](#Picture_Sketching)
- [Base](#Base)
- [Talons](#Talons)
- [Orbs](#Orbs)
- [Jelly_Shell](#Jelly_Shell)

### Planning
### Picture_Sketching
### Base

note: I had written a lot on here, but it appears that I'd forgotten to save my work so it's all mostly gone :(

I started by tracing out what 2D dimmensions the reference pics were giving me. At first, I figured I could use exactly that to form elipses that fit into them to be used as loft planes. But i then realized i just needed to figure out the general shape of the solid, then use that as a loft plane. For the base, I thought it looked almost like a saddle, so i used a spline with a flatter top to sorta form it.

Had some mishaps with extend entities. just had to undo them and manually extend them.

Came back to the base after creating the shell bc it doesn't line up with the shell. Using composite curves on the outlines in order to have them all meet at the end vertexes.
### Talons
### Orbs
### Jelly_Shell

Final frontier lets do this

The game plan is to:
1. Use same planes fron the base and do basically the same thing (but with a more bulbous shape)
2. Use the shell command to make it hollow
3. use boolean to solve any intersections

Looking back, I feel like I should do it another way, but I'm running out of time and I know how to do this

Ok. how should I construct the shape?

I decided on two separate arcs that are tangent at the top and bottom(and then mirror about the vertical center line.

All of the midplanes use this shape, so that the number of verticies is the same at 4.

At one end, the side continues beyond the top, so I just made the lengths proportional to the next one over

How did i do it? Using the line intersection theorem to create similar triangles, and set the lengths equal to the lines constructing the main sketch.

ins proportional triangles

My 3D fit spline didn't work because I had tried to make it a closed spline. making half of it and then mirroring it as before fixed it

ins ShellComplete

Finally made a shell so it actually looks like a meteriod!

Just one problem...

ins Bad 3D print

It doesn't line up with the base very well...
