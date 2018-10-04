---
layout: page-fullwidth
show_meta: false
title: "Lectures"
subheadline: ""
header:
    title: Intelligent Computational Media
    background-color: "#4286f4;"
permalink: "/lectures/"
breadcrumb: true
---
<ul>
	{% for post in site.categories.lecture %}
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