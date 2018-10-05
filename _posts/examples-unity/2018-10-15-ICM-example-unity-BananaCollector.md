---
layout: page-fullwidth
subheadline: 
title:  "Banana Collectors"
teaser: "A copy of the Unity ML-Agents' Banana Collector environment. The agents are trained to collect bananas, shoot at each other and avoid the bad bananas. Discrete action branching is used in this example."
meta_teaser: 
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/bananacollector/
tags:
    - Games
    - Unity
image:
    thumb:  unity-examples/banana-thumb.png
    title: unity-examples/banana-title.png
    caption: 
    caption_url: 
author: Xiaoxiao Ma
---

This example shows how to create an environment where the action space is discrete with action branching, the agents can interact with each other. and how to use raycasting results as the agent's observations.

We copied the environment from Unity ml-agents, and modified it to train in editor. Here are the results:

### Before Training
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/banana-collector-before-training.gif" alt="">
	   <p>The movement of agents are random before training</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### After Training
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/banana-collector-after-training.gif" alt="">
	   <p>Agents can shoot at each other and collect the good bananas</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### Go to Sourcecode
This Banana Collectors example is one of the examples in the the UnityTensorflowKeras repository. Go to the repository from the link below to install it according to the instructions. 
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a>
    </div>
</div><!-- /.row -->
The Banana Collectors example is located under [Assets/UnityTensorflow/Examples/BananaCollectors](https://github.com/tcmxx/UnityTensorflowKeras/tree/master/Assets/UnityTensorflow/Examples/BananaCollectors) directory.

For more information about this example, see [Here](https://github.com/tcmxx/UnityTensorflowKeras/blob/master/Documents/ExamplesList.md#bananacollectors).

### Exercises
NA


{: .t60 }
<!--
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div>
</div>
-->

