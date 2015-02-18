---
layout: page
title: Brady Bytes
tagline: A dev and design blog.
---
{% include JB/setup %}

<div class="posts">
  {% for post in site.posts %}
    <p><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
    <p>{{ post.content | strip_html | truncatewords: 50 }}</p>
  {% endfor %}
</ul>


