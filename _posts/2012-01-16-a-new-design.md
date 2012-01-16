---
layout: post
title: A New Design
teaser: Working on a new design, again. This blog is turning out to be more about me finding out how I can get various things to work and fit my requirements than writing.
categories:
  - meta
---

I have started working on a new design for the blog. I have made some very unlucky choices and stupid mistakes with the old one, and I'm trying to improve what's already here so I can look at it again. Here's a few of my grievances:

* I haven't planned for pictures in the old design
* I made a few stupid mark up choices
* Less colour!
* `strong`-tags break the vertical rhythm in the old design by increasing line height for some reason
* With the old design, displaying more than one paragraph of text on the front page looks butt ugly
* Actually, that ribbon is ugly as hell, it needs to go!
* Posts without teasers looked stupid
* Thanks to jekyll's, I needed to be careful about what characters I used in my teasers as well as do manual masking. That sucks!
* update to html5boilerplate 2.0

And here's some of the ideas I'm toying around with:

* I don't want to write teasers any more
* Increase my posting frequency by interlacing with shorter posts and links
* Think up categories and ways to mark them visually (especially focus on the difference between full post, short post and link)
* I need a working fall back font for the flourishing, ffs!
* I'm toying around with the idea of setting all headlines in lower case
<del>* I want my posts on the index-page fully, without comments</del>
* If you want to comment, you will be taken to the article view
* Pictures
<del>* My branch layout for this blog's repository.
	* "default" branch for the status quo
	* "wip" and bookmarks for new blogposts
	* "design" for work on the design</del>
* Is there a way I can maybe later migrate this to a python blog engine? Maybe something flask driven, on my own server?

I need a category list. And, as I can easily do that, post types.

I want the following post types:

* text
* link
* photo
* video
* quote
* tweet

I want the following categories:

* meta
* personal
* computers
* hci
* design

While I am pretty sure about the post types---they are pretty standard ones---I am not too sure about the categories. They still don't feel right to me. And I need to find a way to get content online without the need to be at my workstation. Why can there be no comprise? A blog software or CMS that uses a DVCS and that I can edit via a web interface and in my favourite editor. Like github or bitbucket wikis allows me to. :(