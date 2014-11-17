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

Hi, my name is Florian, and I like [design]({{ site.url }}/tags/#design); [computers]({{ site.url }}/tags/#computers); [cooking, eating and drinking](https://genussspechte.in/) as well as [photography]({{ site.url }}/tags/#photography) and [people]({{ site.url }}/tags/#people).

This site is about me, and only me. I've also just started a little project with a friend, called "[Die Genußspechte](https://genußspechte.in/)", where we collect places where we've spent time eating and drinking with friends and that we enjoyed spending time at, as well as little eassay about stuff that we like and recipes. It's currently a work in progress, so don't expect too much when you go there.

For now, all that's left to do is blog to fill this up, and tweak this baby as I go along.

Ciao,  
&nbsp;&nbsp;&nbsp;&nbsp;Florian

---

<ul class="post-list">
{% for post in site.posts limit:7 %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span></a></article></li>
{% endfor %}
</ul>
