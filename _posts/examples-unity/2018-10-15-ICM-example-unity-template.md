---
layout: page
subheadline: Example Template Unity
title:  "The ICM Example Template Unity"
teaser: "Teaser. We can right the short description of the example here. It is shown below the title in the post and in the short description of the list of posts page."
meta_teaser: "This is an example of a beautiful aligned post in the middle. There is no sidebar to distract the reader. The difference to the Page-Template is, that you find meta-information at the bottom of the post."
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/template/
tags:
    - Games
    - Unity
image:
    thumb:  homepage_typography-thumb.jpg
    title: logo.png
    caption: image caption
    caption_url: 
author: Xiaoxiao Ma
---

This is the template of a example page. You can use markdown format to right as in github readme.

## Video
You can insert a video using iframe like this;
<div class="flex-video">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/hokkA77ib3c" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div>

## Image
If you want to insert images/gifs, you can directly use any html you want, or as following examples
<div class="row">
  <div class="large-6 columns">
      <img src="http://placehold.it/470x264/6b6351/e1dcd7&amp;text=Width+470+Pixel">
  </div>
  <div class="large-6 columns">
      <img src="http://placehold.it/470x264/e05a10/e1e75e&amp;text=Width+470+Pixel">
  </div>
</div>

## more description
Write more if you want.

## Go to sourcecode
Maybe then a link to the repository or others, you can use any html, or this button:
{% include alert success='<a href="https://github.com/tcmxx/UnityTensorflowKeras">Check on Github</a>' %}

## Questions and exercises
Write the ending questions and exercises here.
### question 1
### question 2

{% include next-previous-post-in-category %}
{: .t60 }
{% include list-posts tag='Games Unity' %}

