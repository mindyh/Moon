---
id: 55
title: 'My Hapkit Journey &#8211; Calibration'
date: 2013-11-22T08:08:49+00:00
author: Mindy Huang
layout: post
guid: http://mindyhuang.me/blog/?p=55
permalink: /my-hapkit-journey-calibrating/
tags:
  - haptics
  - projects
  - coding
comments: true
---
This week, the lab consisted of calibrating the sensors and outputting a specified force. It as the first time we got to program the board. And as a software person, it was very exciting. Getting to learn Arduino was one of the main reasons I decided to take this course.

The Hapkit board is a version of Arduino, with its components rearranged and some sensors added. Also, producing their own board instead of buying off-the-shelf saved a lot of money for the course. 

The first program I ran on my board was Blink.ino, which simply made the LED blink on and off. Simple though it was, it was a good example on manipulating pins and also very cool to see hardware respond!

<img class="alignnone size-large wp-image-58" alt="2013-11-20 00.02.27" src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/2013-11-20-00.02.27-1024x577.jpg" />

The first calibration we had to do was figure out the rotation angle of the handle given the reading of the magnetic sensor, which was used to track the rotations of the motor axis.

<img class="alignnone size-large wp-image-60" alt="2013-11-21 23.19.26" src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/2013-11-21-23.19.26-1024x577.jpg" />

After taking a bunch of sensor readings at known angles, we ran linear regression and found the best fit line to extrapolate the data with. The kind of calibration I&#8217;d always done in FIRST robotics was just offsetting sensor data, so I found this kinda cool.

<img class="alignnone size-large wp-image-56" alt="Calibration" src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/Calibration-1024x576.png" />

Once we had the angle, we chugged through some kinematics equations to get the distance the handle had traveled. Which is dull until it shows up on your screen directly reflecting a physical property of the machine in front of you. Then it&#8217;s exciting. 😀

The next step in the lab was to output a force. That is, specify a force and have the Hapkit to exert it. Sadly, most of the logic involving actually talking to the motor was already programmed in the starter code, and all we needed to do was mess around with some equations (which makes sense given that this course is targeted at students without much programming/engineering experience). But I scanned through the starter code, and gleaned this much &#8211; the motor strength is determined by a PWM through the motor pin, and the duty cycle is the desired torque scaled by some magic function. Now that I write it out, it seems quite obvious.

I was quite surprised at the amount of force the motor exerted &#8211; the Hapkit nearly slid off my desk several times as I was pushing back against its handle!

The next and last sensor to calibrate was the Force Sensitive Resistor.

<img class="alignnone size-large wp-image-61" alt="2013-11-21 23.50.14" src="http://s416.photobucket.com/albums/pp249/KCHuang/Blog/2013-11-21-23.50.14-577x1024.jpg" />

Unfortunately the FSR was not very precise, and so the data read has an error margin of about 30%, not including the fact that you get different readings based on how much surface area your finger shares with the sensor. But given how cheap all the hardware was (the total kit amounts to $50 in cost!), I&#8217;m not surprised. It just adds another dimension to our hapkit to be tinkered with in future labs. >:)