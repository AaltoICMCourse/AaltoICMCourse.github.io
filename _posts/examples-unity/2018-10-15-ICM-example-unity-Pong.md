---
layout: page-fullwidth
subheadline: 
title:  "Pong"
teaser: "Traing the agent to play the classic Pong game! You can either train it by show it how to play using supervised learning or let it play with itself using reinforcement learning."
meta_teaser: 
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/pong/
tags:
    - Games
    - Unity
image:
    thumb:  unity-examples/pong.png
    title: 
    caption: 
    caption_url: 
author: Xiaoxiao Ma
---

### Trained agent using supervised learning
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/pongSL-after-training.gif" alt="">
	   <p>Trained with 30000 samples from gameplay of myself. The result is not good enough. The agent does not know how to react if it have never seen similiar observations in the training samples.</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### Trained agent using reinforcement learning and selfplay
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/pongRL-after-training.gif" alt="">
	   <p>The agent plays much better than the one with supervised learning. It even learns to hit the ball with the edge of racket to create harder situation for the opponent.</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

Another extra demonstration in this example is showing how to use supervised learning to initialize the neural network used for reinforcement learning. Generally, this can speed up the training process.
### Trained agent using reinforcement learning and selfplay, with weights initialized from supervised learning
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/pongSLRL-after-training.gif" alt="">
	   <p>Compared with the agent trained with RL only, it does less unnecessary movement. Even though it tries to keep the racket at the bottom for some unknown reason.</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->


### Go to Sourcecode
This Pong example is one of the examples in the the UnityTensorflowKeras repository. Go to the repository from the link below to install it according to the instructions. 
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a>
    </div>
</div><!-- /.row -->
The Pong example is located under [Assets/UnityTensorflow/Examples/Pong](https://github.com/tcmxx/UnityTensorflowKeras/tree/master/Assets/UnityTensorflow/Examples/Pong) directory.

For more information about this example, see [Here](https://github.com/tcmxx/UnityTensorflowKeras/blob/master/Documents/ExamplesList.md#pong).

### Exercises
NA

{: .t60 }
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>
{% include list-posts tag='Unity' %}

