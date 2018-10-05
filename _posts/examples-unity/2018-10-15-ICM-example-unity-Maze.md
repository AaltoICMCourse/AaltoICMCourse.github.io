---
layout: page-fullwidth
subheadline: 
title:  "Maze"
teaser: "Train a agent to go through a basic maze, with either visual/vector observation."
meta_teaser: 
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/maze/
tags:
    - Games
    - Unity
image:
    thumb:  unity-examples/maze.png
    title: 
    caption: 
    caption_url: 
author: Xiaoxiao Ma
---

This example is a more complicated version of the [Grid World](/examples/unity/gridworld/). The goal of the agent(yellow) is to reach the target(green) while avoiding the walls(red) within certain amount of steps.

We provide two types of training scenarios. One uses vector observation and the other uses visual observation. The results are shown below:

### Maze using vector observation
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/maze-after-training.gif" alt="">
	   <p>The agent is able to reach the goal most of time.</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### Maze using visual observation
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/maze-visual-after-training.gif" alt="">
	   <p>It takes longer time to train the agent with visual observation, but the result is similiar.</p>
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### Go to Sourcecode
This Maze example is one of the examples in the the UnityTensorflowKeras repository. Go to the repository from the link below to install it according to the instructions. 
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a>
    </div>
</div><!-- /.row -->
The Maze example is located under [Assets/UnityTensorflow/Examples/Maze](https://github.com/tcmxx/UnityTensorflowKeras/tree/master/Assets/UnityTensorflow/Examples/Maze) directory.

For more information about this example, see [Here](https://github.com/tcmxx/UnityTensorflowKeras/blob/master/Documents/ExamplesList.md#maze).

### Exercises
#### Exercise 1
Change the dimension of the maze and train your agent using vector observation.


{: .t60 }
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>
{% include list-posts tag='Unity' %}

