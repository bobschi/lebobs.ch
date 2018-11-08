---
layout: post
date: 2017-10-30 11:39:27 +0100
title: Running gollum wiki as a service under macOS High Sierra
---

So, I ran into an interesting problem. I have this pretty sweet setup that takes care of synching it and keeping my `gollum` wikis alive in the background. It's two shell scripts and two `launchd` plist-files.

Everything worked fine, until I decided to upgrade to macOS High Sierra. I had been on Sierra until then, and since GPG Tools where already functional enough for High Sierra, and APFS promised a few performance gains for my machine, I applied the upgrade. I was pretty happy about the result, until I tried to access one of my local wikis.

![My helpful screenshot]({{ "/images/gollum-1.png" | absolute_url }})

Fuck.

So after some checking, and running `gollum` manually from the terminal, I figure out that everything was there; for some reason, when I run gollum via `launchd`, it can't access what's in my home folder. Apparently, nobody else has so far run into this problem, or I am missing something pretty obvious that everybody else knows. But let's investigate a bit ...

So, I first check on my other local wikis, and voila, some problem. However, my local `jekyll`---which is the static site generator that powers this blog---is running just fine in the background. That's interesting. So maybe it's not something to do with the upgrade, but some problem with `gollum`, or the way it interacts with the system.