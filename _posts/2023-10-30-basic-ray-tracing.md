---
date: 2023-10-30 04:07:07
layout: post
title: "Ray Tracing Basics"
subtitle:
description:
image: /Resources/Images/Posts/IntroRayTracing/CornellBox.png
optimized_image:
category: graphics
tags:
    - graphics
author:
paginate: false
---
*Cover: Ray Tracing w/ unlimited-bounce, 512-spp global illumination*
## Why Ray Tracing
Rasterization is efficient in handling direct lighting and lights that are reflected only once, using shading models like Blinn-Phong. However, 
when it comes to global illumination problems like multiple reflections, rasterization requires more complex approximations and methods.

![Rasterization](/Resources/Images/Posts/IntroRayTracing/Raster-1.png)
*Rasterization result (simulated by Ray Tracing)*

You can see from the image above that general rasterization approaches can only generate hard shadow, i.e., black shadow with clear edges. However, in photo-realistic scenes, the shadow is usually soft and fades off towards the edges. Another obvious issue is, the scene generated by rasterization is quite dark. From the perspective of physics, every light carrys energy. Rasterization "cuts off" the lights with multiple times of bounces, causing loss of energy within the scene. 

![Compare](/Resources/Images/Posts/IntroRayTracing/RT-Compare.png)
*The brighter, the better!*
Condition: 12-core CPU, 128 ssp, 1,2,3,unlimited- bounces  
Time: 162, 234, 279, 407 seconds

## What is Ray Tracing
To do...

## How to implement Ray Tracing
To do...