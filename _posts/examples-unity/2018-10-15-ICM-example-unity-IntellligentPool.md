---
layout: page-fullwidth
subheadline: 
title:  "Intelligent Pool"
teaser: "An example of playing the billiard using sampling based method, and how to combine it with supervised learning."
meta_teaser: 
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
categories:
    - example-unity
permalink: /examples/unity/intelligentpool/
tags:
    - Games
    - Unity
image:
    thumb:  unity-examples/pool-thumb.png
    title: unity-examples/pool-title.png
    caption: 
    caption_url: 
author: Xiaoxiao Ma
---

We use CMA-ES(Covariance Matrix Adaption - Evolution Strategies) to find the optimal solution to a billiard problem. CMA-ES is a sampling based method, where it needs to sample different actions(shooting direction and power in our case), evaluate the final result of those actions and obtain the best of them. CMA-ES uses matrix adaption and 
evalution strategy to improve the sampling distribution, so that it is much easier/faster to find the best action.

### Demo of play billiard using CMA-ES, and the 2D heatmap of action space
<div class="row text-center">
	<iframe width="560" height="315" src="https://www.youtube.com/embed/M-WcPtI0p1Y" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div><!-- /.row -->

CMA-ES is slow, but its result is generally good. Neural network is fast at inference time. Therefore we can use the results from CMA-ES to train a neural network using supervised learning. 

However, the result from neural network is not as good as expected(we will show in the next video). Even though, it is still possible to use the output from neural network as the initial guess of CMA-ES, hence speed up the optimization process.

Here is the demo using a simplified billiard environment:
### Comparison of using CMA-ES only, trained neural network only, and both of them
<div class="row text-center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/0IV3TfTuNBM" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>
</div><!-- /.row -->

The reason why we used the simplified environment is that the billiard game is too hard to learn because of its nature. We probably need much more samples and deeper neural network to generate a ok result.

The article below has a more detailed explanation of the billiard example including what we have tried and why it is hard to train a neural network for this game.

[Intelligent Pool](https://github.com/tcmxx/UnityTensorflowKeras/blob/master/Documents/IntelligentPoolDetails.md)

### Go to Sourcecode
This Intelligent Pool example is one of the examples in the the UnityTensorflowKeras repository. Go to the repository from the link below to install it according to the instructions. 
<div class="row">
    <div class="medium-6 columns t10">
	  <a class = "radius button small" target="_blank" href = "https://github.com/tcmxx/UnityTensorflowKeras" >View on Github</a>
    </div>
</div><!-- /.row -->
The 3D ball example is located under [Assets/UnityTensorflow/Examples/IntelligentPool](https://github.com/tcmxx/UnityTensorflowKeras/tree/master/Assets/UnityTensorflow/Examples/IntelligentPool) directory.

### Exercises
NA


{: .t60 }
<div id="bottom" class="row t30">
    <div class="small-12 columns">
       {% include next-previous-post-in-category %}
    </div><!-- /.small-12.columns -->
</div>
{% include list-posts tag='Games Unity' %}

