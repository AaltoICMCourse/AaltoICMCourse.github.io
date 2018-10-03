---
layout: page-fullwidth
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
  <div class="large-12 columns t30">
      <img src="http://placehold.it/470x264/6b6351/e1dcd7&amp;text=Width+470+Pixel">
  </div>
  <div class="large-12 columns t30">
      <img src="http://placehold.it/470x264/e05a10/e1e75e&amp;text=Width+470+Pixel">
  </div>
</div>
<div class="row">
    <div class="medium-4 columns t30">
    <img src="{{ site.urlimg }}gallery-example-4.jpg" alt="">
    </div><!-- /.medium-4.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}gallery-example-5.jpg" alt="">
    </div><!-- /.medium-4.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}gallery-example-6.jpg" alt="">
    </div><!-- /.medium-4.columns -->

</div><!-- /.row -->


<div class="row">
    <div class="medium-8 columns t30">
    <img src="{{ site.urlimg }}gallery-example-7.jpg" alt="">
    </div><!-- /.medium-8.columns -->

    <div class="medium-4 columns t30">
      <img src="{{ site.urlimg }}gallery-example-3.jpg" alt="">
      <img class="t30" src="{{ site.urlimg }}gallery-example-8.jpg" alt="">
    </div><!-- /.medium-4.columns -->

</div><!-- /.row -->

## more description
Write more if you want.

## Go to sourcecode
Tell the directory of this example in the original repository
<div class="row">
    <div class="medium-6 columns t30 medium-centered text-center panel">
	<div>
      All unity examples are part of the UnityTensorflowKeras repository. Please check the instructions on the repository's Github page.
	  </div>
	  <div><a class = "radius button small" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a></div>
    </div>

</div><!-- /.row -->


## Questions and exercises
Write the ending questions and exercises here.
### question 1
### question 2

<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>


