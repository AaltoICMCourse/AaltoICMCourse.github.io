---
layout: page-fullwidth
subheadline: 
title:  "Pole"
teaser: "Train a agent to balance a pole above its pivot by applying a torque, with either visual/vector observation. "
meta_teaser: 
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/pole/
tags:
    - Games
    - Unity
image:
    thumb:  unity-examples/pole.png
    title: 
    caption: 
    caption_url: 
author: Xiaoxiao Ma
---

In this example, the goal of the agent is to keep the pole's center of mass above its pivot point by applying different torque on it. The only external force is the gravity, which tries to make the pole falling down.

Before the training, the system with agent giving random torque looks like this:
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/pole-before-training.gif" alt="">
	   <p>The pole swings randomly without trained agent.</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

After the training, the agent is doing what we want it to do:
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/pole-after-training.gif" alt="">
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

We also provide another scenario with visual observation(the camera image) instead of vector observation(angle and speed of the system). Because one frame of camera does not tell the velocity, and our agent does not have memeory yet, a velocity indicator graphic is added.

Here is the trained agent with visual observation:
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/pole-visual-after-training.gif" alt="">
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->


### Go to Sourcecode
This Pole example is one of the examples in the the UnityTensorflowKeras repository. Go to the repository from the link below to install it according to the instructions. 
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a>
    </div>
</div><!-- /.row -->
The Pole example is located under [Assets/UnityTensorflow/Examples/Pole](https://github.com/tcmxx/UnityTensorflowKeras/tree/master/Assets/UnityTensorflow/Examples/Pole) directory.

For more information about this example, see [Here](https://github.com/tcmxx/UnityTensorflowKeras/blob/master/Documents/ExamplesList.md#pole).

### Exercises
NA

{: .t60 }
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>
{% include list-posts tag='Unity' %}

