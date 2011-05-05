---
layout: default
title: bobschi's BLAHRG
---
{% assign first_post = site.posts.first %}
<div id="post">
  <h2><a href="{{ first_post.url }}">{{ first_post.title }}</a></h2>
  <div id="date">published {{ first_post.date | date_to_string }}</div>
  {{ first_post.content }}
</div>

<hr />