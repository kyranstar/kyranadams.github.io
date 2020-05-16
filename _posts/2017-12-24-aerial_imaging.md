---
layout: blog_post
title: Aerial Imaging Project for UT Austin Engineering Curriculum
excerpt: Built an app that efficiently generate images using unique pixel colors.
preview_image: /assets/files/aerial_image1.webp
tags: [Arduino, Hardware]
---
This is an Arduino based project to be used in the University of Texas at Austin engineering curriculum. It is an aerial release mechanism that will drop student designed payloads remotely from a height of 100 feet.

We used Arduino, plexiglass lasercut case, RF24 radio module and Adafruit BMP085 pressure module

[This is the Github Repository](http://github.com/WasabiFan/aerial-release-system)

It consists of two parts: the ground control module, and the release module. The ground module sends signals to the release module to control the release of a student's project. This is an improvement over the earlier system, where payloads were released via a 100 foot string attached to a mechanism. The new system also alerts the user when a barometric pressure difference of 100 feet is achieved in the release module.

![](/assets/files/aerial_image2.webp)
![](/assets/files/aerial_image3.webp)
![](/assets/files/aerial_image4.webp)