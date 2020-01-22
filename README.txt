Scott Aiton

List of Files:

box.png				        - box texture
moon.jpg				    - moon texture
moonHeight.jpg			    - moon heightmap

FlatShading.png             - screenshot of flat shader
GouraudShading.png          - screenshot of gouraud shader
PhongShading.png            - screenshot of phong shader
MathTexture.png             - screenshot of math texture
NoiseTexture.png            - screenshot of noise texture
SecondShader.png            - screenshot of scene with second shader

glMatrix_util.js            
webgl-utils.js

Moon.html 	   		        - main page with all the shaders
README.txt			        - this file

For the mouse controls, the scroll wheel zooms in and out.
Moving the mouse up and down tilts the map back and forth.
Moving the mouse left and right rotates the map about it's center.

For the model, I made a sphere and mapped a texture of the moon to it.
The texture and the heightmap were both from NASA https://svs.gsfc.nasa.gov/4720

In order to do the flat shading, I made the position a varying variable, and then
used the dFdx and dFdy functions to get the normal.

For the bump mapping, I mapped the texture coordinate to a spherical coordinate (theta,phi)
and then calculated the radius from the heightmap. I then used the derivative
functions to get the normal.

For the second shader, I used the shader code from the box example and then made it orbit
the moon.