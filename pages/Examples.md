---
layout: page
show_meta: false
title: "Examples"
subheadline: "Applications of Computational Intellicence"
header: no
permalink: "/examples/"
---

<ul>
	{% for post in site.categories.examples-python-audio-visual %}
	  <div class="row">
		<div class="small-12 columns b60">
		  <p class="subheadline">{{ post.categories | join: ' &middot; ' | prepend: '<span class="subheader">' | append: '</span>' }}{% if post.categories != empty and post.subheadline != NULL %} – {% endif %}{{ post.subheadline }}</p>
		  <h2><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
		  <p>
			{% if post.image.thumb %}<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="{{ post.title | escape_once }}"><img src="{{ site.urlimg }}{{ post.image.thumb }}" class="alignleft" width="150" height="150" alt="{{ page.title escape_once }}"></a>{% endif %}

			{% if post.meta_description %}{{ post.meta_description | strip_html | escape }}{% elsif post.teaser %}{{ post.teaser | strip_html | escape }}{% endif %}

			<a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}" title="{{ site.data.language.read }} {{ post.title | escape_once }}"><strong>{{ site.data.language.read_more }}</strong></a>
		  </p>
		</div><!-- /.small-12.columns -->
	  </div><!-- /.row -->
    {% endfor %}
	
	{% for post in site.categories.examples-unity-games %}
    <li><a href="{{ site.url }}{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
</ul>