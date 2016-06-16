---
id: 538
title: 'Graphics Pt. 2 &#8211; Raytracer'
date: 2015-12-18T06:36:27+00:00
author: Mindy Huang
layout: post
permalink: raytracer/
excerpt: "My final raytracer project for CS148, was ranked #11 out of ~150 projects. (Pretty good for the amount of work I [didn't] put in)."
tags:
  - art
  - coding
  - projects
comments: true
---
[See my first post featuring my scanline image!](/scanline-2/)

I never was terribly interested in graphics but needed this course for my degree. I came out of it with one of highest grades I&#8217;ve ever gotten in a CS class (they graded partially on aesthetics and I probably have an unfair advantage in that area) and the conclusion that I am far more interested in the math underlying graphics simulations than I am in actually creating art with it. (read: I don&#8217;t ever want to touch Autodesk Maya and 3DS Max again, there are far easier ways to create art @_@)

#### An LA Christmas<figure id="attachment_539"  class="">

<figure>
<img src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/final-1-1024x582.png" alt="My raytracer project for CS148 - Intro to Graphics." /><figcaption class="">My raytracer project for CS148 &#8211; Intro to Graphics.</figcaption>
</figure> 


**Inspiration**

<span style="font-weight: 400;">I was having some trouble with my first idea that involved a light bulb (this was a few days before the refraction bug was found), but I noticed that reflections showed up really nicely. So I decided to do something that emphasized reflections instead, and since I was in LA at the time I decided to do something sunshine themed. Thus I ended up with sunglasses at the beach.</span>

**Modelling**

<span style="font-weight: 400;">Since raytracing takes a lot of time, I wanted to minimize the amount of geometry I had. For this image, I only have the sunglasses, a picnic table, and two sky planes. I pulled all the models and images from online. Originally I also wanted to put bottles or some still life to be reflected in the glasses as well, but I felt they detracted from the scene so I took it out.</span>

<span style="font-weight: 400;">I have 2 lights in the scene &#8211; one area light and one point light. The point light is placed right in front of the image of the sun on the sky plane so the glasses would reflect it as an extra glare. The area light is placed above and in front of the glasses and tilted down to imitate the ambient sunset light. I originally wanted soft shadows and was puzzled why this setup didn’t produce any, but then realized that at such an angle shadows are generally long and hard-edged, just as shadows at sunset are.</span>

**Advanced techniques**

<span style="font-weight: 400;">I was really looking forward to doing something photorealistic with the raytracer assignment and I really like photographs with soft focus, so naturally I chose to implement depth of field. My aperture is quite large. My final render is with 256 samples per pixel and 8 reflection bounces. Since I have no refraction I set the max refraction bounces to 0. I used BVH acceleration structures and multithreading to help speed up the rendering process.</span>
  
<span style="font-weight: 400;">The most aggravating issue I encountered was determining what value of LARGE_EPSILON to perturb by. I found that if it was too small a grid pattern would show up on the glasses lens. But if it was too large then the shadows on the table would render incorrectly. Unfortunately there was no intermediary value that solved both issues satisfactorily, so I chose to have the lens render well at the expense of the shadows. </span>