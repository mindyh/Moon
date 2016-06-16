---
id: 82
title: 'My Hapkit Journey &#8211; Virtual Environments'
date: 2013-12-16T02:33:16+00:00
author: Mindy Huang
layout: post
guid: http://mindyhuang.me/blog/?p=82
permalink: /my-hapkit-journey-virtual-environments/
categories:
  - Projects
tags:
  - haptics
  - hardware
comments: true
project: true
---
The last two weeks of the course were all about virtual environments. This is also where I really geeked out. Basically my friends were subjected to me going &#8220;Lookit! Touchit! It feels like a button OMG.&#8221;

The labs started out coding fairly basic environments &#8211; just springs and dampers. But what I found cool about this was that we modeled them with equations from high school physics. The way that everything is interconnected in the end&#8230;proof that school is useful! 

Once we had springs and dampers figured out, we went on to building more complex environments &#8211; walls (one-sided springs, essentially) and textures (damping fields interspersed with low-resistance bands). Below is the graph of force vs position of my damping field texture, courtesy of Matlab.

<img class="alignnone size-medium wp-image-88" alt="damping_texture" src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/damping_texture.png" />

The last lab consisted of putting all these techniques together and creating environments based off of real life objects. I tried to recreate a button and a stapler.

The button environment consisted of a step function of a spring and a wall.  It actually worked really well. The data is graphed below.

<img class="alignnone size-medium wp-image-89" alt="button" src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/button.png" />

This is where I sat and pressed my virtual button over and over for a few minutes, just because I could.

The last object I tried to recreate was a stapler. This endeavor was a failure, unfortunately. The motor on the Hapkit was not strong enough to recreate the sensation (I was modelling a normal, 5 dollar stapler. Not one of the fancy one-finger push staplers).

I wanted to program more environments, but the time crunch of finals week meant I had to limit myself to accomplishing the bare minimum.

And so ended my Hapkit journey. My thoughts on the course: it was very easy, which is good because otherwise I could not have taken it on top of my existing workload. But despite (or maybe because of) it being easy, I actually learned a lot. It was definitely my favorite class of the quarter. An altogether very rewarding experience that peaked my interest in haptics, I will be on the lookout for more opportunities like it in the future.
