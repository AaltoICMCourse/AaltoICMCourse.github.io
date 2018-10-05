---
layout: page
subheadline: Example Template Audio
title:  "The ICM Example Template Audio"
teaser: "Teaser. We can right the short description of the example here. It is shown below the title in the post and in the short description of the list of posts page."
meta_teaser: "This is an example of a beautiful aligned post in the middle. There is no sidebar to distract the reader. The difference to the Page-Template is, that you find meta-information at the bottom of the post."
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-python-audio
permalink: /examples/python/audio/template/
tags:
    - Audio
    - Python
image:
    thumb:  homepage_typography-thumb.jpg
    title: logo.png
    caption: image caption
    caption_url: 
author: Xiaoxiao Ma
---

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

{: .t60 }
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>
{% include list-posts tag='Audio' %}

