---
layout: default
title: Blog Archive
permalink: /archive/
---
 
# Blog Archive
 
{% if site.posts.size > 0 %}
<ul class="post-list">
  {% for post in site.posts %}
  <li>
    <a class="post-title-link" href="{{ post.url }}">{{ post.title }}</a>
    <span class="post-date">{{ post.date | date: "%b %-d, %Y" }}</span>
  </li>
  {% endfor %}
</ul>
{% else %}
*No posts yet — check back soon!*
{% endif %}
 
