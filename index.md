---
layout: page
title: "A Tour de Force of Bobschi"
modified: 2013-10-29
---

---

<div style="text-align: center;">
  <img src="{{ site.base-url }}/images/weheart.png" width="120px" height="120px" />
</div>
<div style="text-align: center;">
<strong>We want games to be a space where everyone feels welcome.<br/>
We think critical thinking in games should be applauded.<br/>
We want to play all kinds of games, made by all kinds of people.<br/>
We think games are for everyone.<br/></strong>
<a href="https://weheart.github.io/">weheart.github.io</a>
</div>

---

<ul class="post-list">
{% for post in site.posts limit:13 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
