---
layout: page
show_meta: false
title: "Unity Examples"
subheadline: "machine learning applications in games"
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
permalink: "/examples/unity/"
breadcrumb: true
---

<div class="row">
    <div class="medium-6 columns t30 medium-centered text-center">
	<p>
      All unity examples are part of the UnityTensorflowKeras repository. Please check the instructions on the repository's Github page.
	  </p>
	  <a class = "radius button small" href = "" >View on Github</a>
    </div>

</div><!-- /.row -->

<ul>
	{% for post in site.categories.example-unity %}
	  <div class="row">
		<div class="small-12 columns b60">
		  <h2><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
		  <p class="subheadline">{{ post.categories | join: ' &middot; ' | prepend: '<span class="subheader">' | append: '</span>' }}{% if post.categories != empty and post.subheadline != NULL %} – {% endif %}{{ post.subheadline }}</p>
		  <p>
			{% if post.image.thumb %}<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="{{ post.title | escape_once }}"><img src="{{ site.urlimg }}{{ post.image.thumb }}" class="alignleft" width="150" height="150" alt="{{ page.title escape_once }}"></a>{% endif %}

			{% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% elsif post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}

			<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="{{ site.data.language.read }} {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a>
		  </p>
		</div><!-- /.small-12.columns -->
	  </div><!-- /.row -->
    {% endfor %}
</ul>