+++
title = 'Nvdia RTX Graphic Cards'
slug = 'post'
image = 'images/rtx.jpg'
date = "2018-09-21T16:15:00"
description = ''
disableComments = true
+++

## RASTERIZATION

To understand what ray tracing means first we need to understand how an image is rendered in a GPU. Currently, Graphics cards use a technology called rasterization.

Rasterization basically converts a 3d shape into a 2d image. This process is fast but not realistic it can be described simply as how a painter would draw a scenery. A GPU which works by Rasterization creates a 3d model by combining polygons accordingly and mapping the polygon into individual pixels which then further undergoes the process of shader which gives it texture colour and lighting effect to give a fully rendered frame. The catch here is that at the end of the day rasterization is only trying to approximate a 3d scene to a 2d surface.

## RAY-TRACING

This is where Ray Tracing comes in we can consider this to how our eye actually perceives an image. When a source emits light(photons) it travels to all direction hits many objects and undergoes physical conditions life absorption refraction reflection and bounces off to the next surface. When this light (photons) enter our eye we perceive an image.

![RASTERISATION VS RAY-TRACING](/images/rayvsras.jpg)

This is the same process undergone in Ray Tracing but it is very difficult to do this in real time. It takes up even a month to render a scene. For people who have watched the Disney movie  Big Hero 6 this might come as a surprise but the movie uses Ray-Tracing (Path-Tracing) to create every frame but Disney rendered this film with a  55,000 core supercomputer. And this supercomputer took about a day to render a frame. Compare this to the latest and greatest thing that we as an individual can get out hands on (after breaking the bank ) is an Intel i9-8950HK that has 6 cores. Well bye-bye, ray-traced games then, Not Really Nvidia has some tricks up its sleeves that could bring Ray-Traced games to lives.


## REAL-TIME RAY-TRACING

The solutions that Nvidia brought up are the new turing  architecture (more on that later) and the real-time ray-tracing. what happens here is that instead of a drawing a light from the source the light is simulated from the camera (the perspective from the scene is viewed) towards the object thereby decreasing the number of rays required. This rays will undergo all the physical properties that light undergo and finally, it is directed toward the source. The result is an image with realistic shadows, lighting, and textures. This done a definite number of times a second gives a ray-traced game.

{{< youtube Q8V2F3NtCGk>}}



## NVIDIA-TURING

Turing is the new architecture developed by Nvidia which combines rasterization raytracing AI and simulation to obtain an image that is almost lifelike. Unlike the traditional architecture of Nvidia, this hybrid has physical engines that are doing separate tasks that end up with a lifelike image.  To put this into perspective Nvidia's Tesla V100 Data server (costs $68000) is 10 milliseconds slower than a single Turing based GPU.

![NVEDIA RTX TURING](/images/nvidia-rtx-turing-gpu.png)

## NVIDIA-RTX

Nvidia Shows off Ray-Tracing with its new RTX Graphics cards that comes in three new flavours The RTX 2070($499) that has 6 Giga Rays/s 45T RTX-OPS and 8GB of video memory. The RTX 2080($699)  has 8Giga Rays/s 80RTX-OPS and 8GB of video memory. Then comes the Grand finale with the RTX 2080 Ti($999) that has 10Giga Rays/s 78T RTX-OPS and 11GB of video memory.

{{< youtube KJRZTkttgLw>}}

## MY OPINION

When all that seems interesting should you go out and buy these cards well for a gamer, not yet wait for some time see the reviews since these cards do not use the traditional ways of measuring the performance of a GPU we do not still have a confirmation on how much of an upgrade this could be to the current generation. Furthermore, we are yet to see how many game developers are adding Ray-Tracing features to their games. Hopefully, this could be a turning point in the world of graphics cards

For an ML developer hold on this is probably not the GPU for you Nvidia is developing a new ML focused GPU (Quadro RTX) based on Ray-Tracing that could take the whole ML technology to a new level and would be more focused on the scientific side of things rather than gaming.
