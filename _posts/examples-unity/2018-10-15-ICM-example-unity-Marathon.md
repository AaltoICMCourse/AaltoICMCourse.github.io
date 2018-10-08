---
layout: page-fullwidth
subheadline: 
title:  "Marathon Environment from Unity ML-Agents"
teaser: "Training the Unity ml-agent's marathon environment."
meta_teaser: 
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/marathon/
tags:
    - Games
    - Unity
image:
    thumb:  unity-examples/hopper.png
    title: unity-examples/marathon-title.gif
    caption: 
    caption_url: 
author: Xiaoxiao Ma
---

Unity ML-Agents' [marathon environment](https://github.com/Unity-Technologies/marathon-envs) contains a lot of commonly used environments that are similar to ones used in modern AI research. It is easy to use our in-editor training to train the agents in the marathon environment as well. 

### Trained Deepmind Hopper
<div class="row text-center">
	<div class="medium-8 columns t30">
       <img src="{{ site.urlimg }}unity-examples/hopper-after-training.gif" alt="">
    </div><!-- /.medium-8.columns -->
</div><!-- /.row -->

### Go to Sourcecode
You need the UnityTensorflowKeras repository to train ML-Agents in editor. Go to the repository from the link below to install it according to the instructions. 
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a>
    </div>
</div><!-- /.row -->

The marathon environments are not included in ML-Agents or UnityTensorflowKeras repositories. You need to download it from its own repository and put the assets into your Unity project.
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/Unity-Technologies/marathon-envs" >View Marathon Environment on Github</a>
    </div>
</div><!-- /.row -->

### Exercises
Pick one of the environments from the marathon environments, setup the scene for training in editor, and train it. You can use the same parameters for neural network and training as specified in [config/marathon_envs_config.yaml](https://github.com/Unity-Technologies/marathon-envs/blob/master/config/marathon_envs_config.yaml) file.


{: .t60 }
<!--
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div>
</div>
-->

