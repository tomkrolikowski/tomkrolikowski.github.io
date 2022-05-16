---
layout: post
title: Semantic Segmentation Depth Estimation
type: project
image: demo.jpg
video: empty
sections:
  intro: The need for depth perception in the modern world increases dramatically each year. With the creation of self-driving cars and other smart machines, there is an importance in capturing the way human eyes are able to interpret the 3-dimensional world and efficiently convert it into data computers can understand. Using computer vision, and more specifically convolutional neural networks, the problem of mapping real world images into a depth map becomes possible. Using encoder-decoder CNNs, we can capture the spacial relationship between each pixel in an input image from each layer of the net. 
github: https://github.com/lanbas/442-depth-estimation
---
## Approach

For this project, our group utilized transfer learning using resnet-18 and Unet as pretrained models. We trained each model using the Dense Indoor and Outdoor Depth (DIODE) dataset. Although, to increase the training time, we resized the images in the dataset from 768x1024 to 384x512. After training, our group created a small python script to simulate a lense focusing on a particular depth.

## Indoor Results
<img src="/assets/img/indoorresults.png">
From left to right, RGB image, ground-truth depth map, ResNet18 predicted depth map, and UNet predicted depth examples from the DIODE indoor data set.

## Outdoor Results
<img src="/assets/img/outdoorresults.png">
From left to right, RGB image, ground-truth depth map, ResNet18 predicted depth map, and UNet predicted depth examples from the DIODE outdoor data set.

<div class="foot-icon"> 
<a href="{{page.github}}"><span class="fa fa-github fa-2x" style="color:rgb(0, 0, 0);"></span><a>
