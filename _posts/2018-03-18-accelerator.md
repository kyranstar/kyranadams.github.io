---
layout: blog_post
title: The Racetrack, the Horse, or the Jockey - Effectiveness in Startup Accelerators
excerpt: Built an app that efficiently generate images using unique pixel colors.
preview_image: /assets/files/accelerator.png
tags: [Python, Scikit-learn, Web Scraping, ML, Data Cleaning]
---
As a project under the McNair Center for Entrepreneurship and Innovation, I was tasked with generating and processing data to be used in an economics paper. This paper would analyze the effectiveness of startup accelerator programs, and determine whether the effectiveness was due to the programs, the leadership, or the location.

My ultimate goal was to determine more than 40,000 matchings between about 300 accelerator programs and their cohorts, as well as the dates of graduation. The idea was to find "Demo Day" pages, which are pages that many accelerators use to publicize the graduation of their cohorts. I used a web scraper to download google results for the phase "X demo day", where X is the name of the accelerator, and trained a random forest classifier to find these pages with 80% accuracy. Then, these webpages were associated with certain cohorts of accelerators so that we could analyze them.

