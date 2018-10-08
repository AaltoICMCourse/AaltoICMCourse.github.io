---
layout: page-fullwidth
show_meta: false
title: "Python Examples for Audio"
subheadline: ""
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
permalink: "/examples/python-audio/"
breadcrumb: true
---

Here are the audio related python examples that will be used in the course. Currently those are mostly placeholders. Real contents are coming soon.

<div class="row">
    <div class="medium-6 columns t10 medium-centered text-center panel">
	<div>
      The audio related examples are in the MachineLearningWithAudio repository. Please check the original repository on Github if you want to know more.
	  </div>
	  <div><a class = "radius button small" target="_blank" href = "https://github.com/SopiMlab/MachineLearningWithAudio" >View on Github</a></div>
    </div>
</div><!-- /.row -->


<ul>
	{% for post in site.categories.example-python-audio %}
	  {% assign loopindex = forloop.index | modulo: 2 %}
	  {% if loopindex == 1 %}
		<div class="row">
	  {% endif %}
		<div class="small-6 columns">
		  <h3><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h3>
		  <p class="subheadline">{{ post.categories | join: ' &middot; ' | prepend: '<span class="subheader">' | append: '</span>' }}{% if post.categories != empty and post.subheadline != NULL %} – {% endif %}{{ post.subheadline }}</p>
		  <p>
			{% if post.image.thumb %}<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="{{ post.title | escape_once }}"><img src="{{ site.urlimg }}{{ post.image.thumb }}" class="alignleft" width="150" height="150" alt="{{ page.title escape_once }}"></a>{% endif %}

			{% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% elsif post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}

			<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="{{ site.data.language.read }} {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a>
		  </p>
		</div>
	   {% if loopindex == 0 or forloop.index == forloop.length%}
	  </div><!-- /.row -->
	  {% endif %}
    {% endfor %}
</ul>