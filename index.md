---
layout: page
title: Open labbook
tagline: Peter Søgaard Jørgensen
---
{% include JB/setup %}

    
## Notebook

Below you will find the latest notebook entries organized by date.
Click [archive](http://psjorgensen.github.io/archive.html), [categories](http://psjorgensen.github.io/categories.html), [tags](http://psjorgensen.github.io/tags.html) to see all posts by date, topical category and tag, respectively.


<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



## About the web platform

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)
