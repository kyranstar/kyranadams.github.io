---
layout: blog_post
title: Global Illumination Pathtracer in Golang
excerpt: Wrote a monte-carlo unidrectional path tracer in Golang for rendering pixar quality (not really) images.
preview_image: /assets/files/pathtracer.webp
tags: [Golang, Graphics]
---
As another project from my senior year of high school, I decided to write a monte-carlo unidrectional path tracer in Golang. 

It features: 
 - Multicore CPU based stochastic unidirectional path tracer  
 - Loading OBJ files  
 - Various material properties  
 - K-D tree acceleration  
 - Supports adaptive sampling  
 - Thin lens model with depth of field effect 
 
Github link is [here](http://github.com/kyranstar/Path-Tracer).