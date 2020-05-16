---
layout: blog_post
title: Confusing Lepidopterologists
excerpt: Trained a generative adversarial neural network to create new butterflies from historical academic illustrations.
preview_image: /assets/files/butterfly_gif.gif
tags: [ML, Data Cleaning, Python, OpenCV]
---
Training a generative adversarial neural network to generate brand new butterflies. 
Inspired by [this beetle generator by cunicode.](https://www.cunicode.com/works/confusing-coleopterists")

## The Data
The training set consisted of ~1800 butterfly illustrations scraped using opencv from lithographs in 
[Biologia Centrali-Americana]("https://archive.org/details/biologiacentrali41godmrich/page/n3"), an encyclopedia of central American wildlife published at the end of the 19th century.

<img align="right" alt="" class="img-fluid rounded" src="/assets/files/butterfly_grid.webp">

After discovering the aforementioned beetle GAN, I was inspired to write my own scripts to
                            collect the data, which was difficult because of how the butterflies were interlocked in the
                            encyclopaedia pages.


I ended up thresholding each image and then finding bounding rectangles of contours, which
                            could be used to crop out the butterflies. I felt that I had enough datapoints, so I just
                            removed the small number of butterflies that were oriented diagonally or had other
                            artifacts.

## Training

I trained the model using RunwayML, which was a little confusing to use at first but super
                            easy after I understood how it worked, and also pretty cheap. I paid their $10 monthly
                            membership fee and then got the first model training free.

<img align="left" alt="" class="img-fluid rounded" src="/assets/files/butterfly_allsizes.webp"
                             width="400px">

After completing this project, I was honestly really happy with the results! The GAN seemed
                            to have almost the same diversity as the dataset and for most images produced beautiful
                            results.

<img align="right" alt="" class="img-fluid rounded" src="/assets/files/butterfly_single2.webp">

One thing I noticed was that certain images produced were blurry. I originally thought that
                            this was a failure of the training process, but I then realized that this was actually a
                            result of the training data — many of the images were smaller in the book, so when blown up
                            to 1024x1024, they became very blurry.

It's interesting because there is a subtle bias towards which butterflies were smaller in the
                            book. My conjecture is that colorless and drab butterflies, like the one in the bottom left
                            corner in the image above, were probably considered more boring and seem to have been
                            reproduced smaller in the encyclopedia. This made the GAN create blurry reproductions of
                            these and sharp reproductions of the colorful and beautiful butterflies. Not the end of the
                            world!


I produced all of the images and animations in this blog post using Google Colab.

The model is avaiable [here]("https://open-app.runwayml.com/?model=kyranstar/ButterflyBreeder") for you to try out.</a> I might create a few more models from these
                            encyclopedia volumes, so make sure to look out on my instagram [@kpa.pa]("https://www.instagram.com/kpa.pa/")!

<img align="center" alt="" class="img-fluid rounded" src="/assets/files/butterfly_single.webp">