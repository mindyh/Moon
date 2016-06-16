---
id: 317
title: 'Experimental Haptics: Rage Quit'
date: 2014-06-05T23:55:17+00:00
author: Mindy Huang
layout: post
guid: http://mindyhuang.me/?p=317
permalink: /experimental-haptics-rage-quit/
tags:
  - haptics
  - projects
  - coding
comments: true
---
A while ago, I built and programmed a [Haptic Paddle](/my-hapkit-journey-assembly/ "My Hapkit Journey – Assembly"). I enjoyed it, and so this quarter I decided to take Experimental Haptics. It was led by a grad student who invented the [Novint Falcon](http://www.novint.com/index.php/novintfalcon "novint falcon"), low-end, 3-DOF haptic device. This was also the device we used for all our homework assignments and projects.

<figure class="">

<img src="http://www.novint.com/images/stories/Novint_rendering_full3.jpg" alt="Novint Falcon"/><figcaption class="">Novint Falcon</figcaption>
</figure> 


The class took us through the theory as well as the practice of programming haptic devices &#8211; from workspaces to fast collision detection to modelling haptic feedback. My partner and I decided to base our final project on the theme Rage Quit, after a particularly frustrating debugging session on one of the homework assignments.

More specifically, our project was to virtually simulate smashing things out of frustration. We delved into fracturing models (both graphic and haptic) and event-based haptic feedback. There was a lot of tweaking and creativity involved &#8211; having a ton of fractured objects to detect against made it difficult to keep the update rate at a decent 1000Hz. But we managed it in the end! The abstract is linked at the bottom of this post if you&#8217;re interested.

Through this project, I learned that I enjoy learning and creating mathematical models (in this case for the haptic feedback, but it holds generally as well). I also learned that programming math is extremely prone to difficult debug sessions, so make sure your model is spotless before you try to translate it to code.

All in all, this was a really fun (albeit frustrating and time consuming) class. I learned a lot, and enjoyed playing with the Falcon immensely.

[My abstract for this project.](https://github.com/mindyh/mindyh.github.io/raw/master/assets/docs/ragequit.pdf)