# Extrusion3DEC
Extrusion of a surface from .stl file into a blocky volume
The code is written in FISH (Itasca's proprietary language). 
Being the surface defined by a number of triangles, each triangle is extruded to the specified altitude* to form a single block. The iteration through all the triangles gives the total amount of blocks forming the overall volume. The so defined blocks may be merged into one single block by using the command 'join on' into 3DEC's console.

*The altitude must be defined by the user consistently with the stl data: if the lowest point of the imported data has an altitude of 380m, the user must specify an extrusion altitude of 380m at maximum. Otherwise, the program will return an error (usually something like 'cannot create a block with negative volume').
