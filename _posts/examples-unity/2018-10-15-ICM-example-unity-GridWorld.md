---
layout: page-fullwidth
subheadline: 
title:  "Grid World"
teaser: "A basic example where the AI is trained to reach to the destination and avoid the obstacle in a grid world."
meta_teaser: 
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/gridworld/
tags:
    - Games
    - Unity
image:
    thumb:  unity-examples/gridworld-thumb.png
    title: unity-examples/gridworld-title.png
    caption: 
    caption_url: 
author: Xiaoxiao Ma
---

This example shows how to create an environment with visual observation and action [mask](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Design-Agents.md#masking-discrete-actions).

We copied the environment from Unity ml-agents, and modified it to train in editor. Here are the results:

### After training
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/gridworld-after-training.gif" alt="">
	   <p>The agent is able to move the with target while avoiding the obstable</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### Visual Observation
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/banana-collector-after-training.gif" alt="">
	   <p>The input observation of the agent is the image from a top down camera as above</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### Go to Sourcecode
This Grid World example is one of the examples in the the UnityTensorflowKeras repository. Go to the repository from the link below to install it according to the instructions. 
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a>
    </div>
</div><!-- /.row -->
The Grid World example is located under [Assets/UnityTensorflow/Examples/GridWorld](https://github.com/tcmxx/UnityTensorflowKeras/tree/master/Assets/UnityTensorflow/Examples/GridWorld) directory.

For more information about this example, see [Here](https://github.com/tcmxx/UnityTensorflowKeras/blob/master/Documents/ExamplesList.md#gridworld).

### Exercises
NA

{: .t60 }
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>
{% include list-posts tag='Games Unity' %}

