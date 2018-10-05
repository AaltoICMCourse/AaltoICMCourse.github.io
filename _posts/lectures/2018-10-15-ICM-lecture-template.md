---
layout: page
subheadline: Lecture Template
title:  "Lecture1 - template plapla"
teaser: "Teaser. This is the lecture teaser."
meta_teaser: "This is an example meta_teaser."
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - lecture
permalink: /lectures/template/
tags:
    - Lectures
image:
    thumb:  lecture-thumb-placeholder.png
    title: lecture-title-placeholder.png
    caption: image caption
    caption_url: 
author: Xiaoxiao Ma
---
*Feeling Responsive* shows metadata by default. The default behaviour can be changed via `config.yml`. To show metadata at the end of a page/post just add the following to front matter:
<!--more-->

### Insert a video
<div class="row text-center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/0IV3TfTuNBM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div><!-- /.row -->

### Insert an image
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/pongRL-after-training.gif" alt="">
	   <p>The agent plays much better than the one with supervised learning. It even learns to hit the ball with the edge of racket to create harder situation for the opponent.</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### insert codes
```csharp
//create the model. the styleTransferModelData.bytes is the binary files provided that contains all needed pretrained data of the network.
var styleTransferModel = new UniversalStyleTransferModel(CNTK.DeviceDescriptor.GPUDevice(0), styleTransferModelData.bytes);
//build it with specified dimentions
styleTransferModel.CreateModelWithDimensions(contentSize, styleSize);

// Get the raw data of content and style imagefrom the Unity Texture2D object using helper functions.
var tempContentTexture = Images.GetReadableTextureFromUnreadable(contentTexture);
byte[] contentBytes = tempContentTexture.GetRGB24FromTexture2D(contentResize);
```

### grid
<div class="row">
  <div class="small-4 columns">
      <img src="http://placehold.it/303x170/6b6351/e1dcd7&amp;text=Width+303+Pixel">
  </div>
  <div class="small-4 columns">
      <img src="http://placehold.it/303x170/e05a10/e1e75e&amp;text=Width+303+Pixel">
  </div>
  <div class="small-4 columns">
      <img src="http://placehold.it/303x170/fabb00/771e1e&amp;text=Width+303+Pixel">
  </div>
</div>


## Other Post Formats
{: .t60 }
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>
{% include list-posts tag='Lecture' %}

