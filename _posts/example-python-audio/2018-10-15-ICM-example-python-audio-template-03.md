---
layout: page-fullwidth
subheadline: Example Template Audio 03
title:  "The ICM Example Template Audio 03"
teaser: "Teaser. We can right the short description of the example here. It is shown below the title in the post and in the short description of the list of posts page."
meta_teaser: "This is an example of a beautiful aligned post in the middle. There is no sidebar to distract the reader. The difference to the Page-Template is, that you find meta-information at the bottom of the post."
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-python-audio
permalink: /examples/python/audio/template03/
mediaplayer: true
tags:
    - Audio
    - Python
image:
    thumb:  homepage_typography-thumb.jpg
    title: logo.png
    caption: image caption
    caption_url: 
author: xx
---

### Insert audio
[mediaelement.js][1] is like magic. It's browser and device support is perfect. To activate the video or audio player just set the following variable in front matter to `true`.

~~~
mediaplayer: true
~~~

To use the player just use some HTML5-magic like...

{% highlight html %}
<audio src="http://path-to-file.com/music.mp3" type="audio/mp3" controls="controls"></audio>
{% endhighlight %}

#### Comfort Fit - »Freeze The Cut«
<audio src="http://archive.org/download/music_from_all_around_the_world/05._music_from_all_around_the_world_-_comfort_fit_-_freeze_the_cut_opolopos_emotional_draft_remix.mp3" type="audio/mp3" controls="controls"></audio>
[Download Compilation ›](https://archive.org/details/music_from_all_around_the_world)
{: .t30 .button .radius}

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
<!--
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div>
</div>
-->