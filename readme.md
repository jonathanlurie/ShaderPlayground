This repo is just to keep track of my learning of shaders language (as custom shaders in ThreeJS).

## shader_cube_moving_texture.html
Displays jpeg strip as a "cinematic" since the strip is composed of 64 images of the brain at different depth.

## shader_world_coordinates.html
Use the vertex shader to find the 3D world coordinates and make them accessible from the fragment shader. Then change the color of a moving cube depending on it 3D position on world space.

## draggablecubes_shader_world_coord.html
Just like `shader_world_coordinates.html` to adapt the color on the world coordinate positioning. This example is based on the [draggable cubes](https://threejs.org/examples/webgl_interactive_draggablecubes.html) of ThreeJS, so that playing with colors is easier.


## shader_nano_oblique.html
Map a 3D texture on a plane that we can move around. It uses world coordinates and nearest neighbor interpolation.

## shader_nano_oblique2.html
The same as `shader_nano_oblique.html` but using an algorithm from stack overflow to work with 2D texture as 3D texture. Uses linear interpolation.


## shader_nano_oblique_jpegLoader.html
Uses the same concept and interpolation as `shader_nano_oblique.html` but we are loading and decoding a jpeg image in native JS to put in a `THREE.DataTexture`.


## shader_nano_oblique_multiload.html
Uses the same concept and interpolation as `shader_nano_oblique.html` but sends an array of texture to see how responsive it remain. Only one texture is displayed though.

## shader_micro_oblique_multiload.html
Uses an Object3D filled with small planes, all having the same shader. Only one texture is loaded but it intersect with several planes.
