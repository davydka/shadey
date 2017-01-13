shadey
===========

Simple console tool to test OpenGL ES 2.0 fragment shaders on the Raspberry Pi.

Fragment shader and optional texture are specified on command-line.

Credits
-------

* [Pishadertoy](https://github.com/dff180/pishadertoy)

* EGL class code by [Jon Macey](http://jonmacey.blogspot.de/2012/06/opengl-es-on-raspberry-pi-pt-3-creating.html)

* Sample shaders from [ShaderToy](https://www.shadertoy.com) by Inigo 'iq' Quilez. Explore the ShaderToy website for additional shader and texture usage examples.

* Sample textures from http://elout.home.xs4all.nl/texl/tex/index.html

Installation
------------
They assume that you already have set up a working development environment where you can compile the hello\_pi examples.

1. Get sources with `git clone https://github.com/davydka/shadey.git`
2. Install dependencies with `sudo apt-get install libsoil-dev`
3. `cd shadey`
4. `make`

Running
-------
* Make sure to use latest firmware and 192/64 memory split
  * `sudo rpi-update 192`

* Start from Raspberry Pi console or via SSH client 

* Exit program with CTRL-C

### Examples

* Using default fragment shader

    `./pishadertoy`
    
* Using fragment shader which doesn't need texture

    `./pishadertoy shaders/flower.f.glsl`
    
* Using fragment shader with texture

    `./pishadertoy shaders/relieftunnel.f.glsl textures/texl2.jpg`
    
