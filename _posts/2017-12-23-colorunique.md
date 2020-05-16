---
layout: blog_post
title: Image Unique-ifier
excerpt: Built an app that efficiently generate images using unique pixel colors.
preview_image: /assets/files/unique_pixels.png
tags: [Java]
---
This is a personal project inspired by an online programming challenge to generate images using unique pixel colors.

There are several different algorithms the program supports. One algorithm is to, for each pixel in the input image, average its surrounding pixels in the output image and find the closest unused color in the colorspace, and remove that color from the colorspace. The program uses a KD-Tree for finding the closest colors efficiently.

Github link is [here](https://github.com/kyranstar/UniquePixels).