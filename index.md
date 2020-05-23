---
layout: index
title: "Welcome to Amazing Covers"
permalink: /
---

{% for post in site.posts %}
<div class="post">
	<img src="{{ post.image | relative_url }}" alt="{{ post.title }}" width="25%" />
	<h2><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h2>
	<h5>Posted on {{ post.date | date: '%B %d, %Y' }} in {{ post.category }}</h5>
</div><!-- end /.post -->		
{% endfor %}