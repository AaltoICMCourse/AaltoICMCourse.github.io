---
layout: page
subheadline: Example Template
title:  "The ICM Example Template"
teaser: "Teaser. We can right the short description of the example here. It is shown below the title in the post and in the short description of the list of posts page."
meta_teaser: "This is an example of a beautiful aligned post in the middle. There is no sidebar to distract the reader. The difference to the Page-Template is, that you find meta-information at the bottom of the post."
breadcrumb: true
header:
    title: Intelligent Computational Media
    background-color: "#EFC94C;"
categories:
    - examples-python-audio-visual
permalink: /examples/unity/template/
tags:
    - Games
    - Unity
image:
    title: logo.png
    caption: image caption
    caption_url: 
author: Xiaoxiao Ma
---
*Feeling Responsive* shows metadata by default. The default behaviour can be changed via `config.yml`. To show metadata at the end of a page/post just add the following to front matter:
<!--more-->

~~~
show_meta: true
~~~

If you don't want to show metadata, it's simple again:

~~~
show_meta: false
~~~


## Other Post Formats
{: .t60 }
{% include list-posts tag='Games Unity' %}

