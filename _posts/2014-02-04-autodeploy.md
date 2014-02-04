---
layout: post
date: 2014-02-04 14:53:01 +0100
title: "Setting up autodeploy"
category: 'tech'
tags: ['it','jekyll', 'uberspace']
---

Today, I set up autodeploy for my blog as per [this tutorial](http://www.grobmeier.de/autodeploy-jekyll-28012014.html). It will pull any merges I push to bitbucket. I have also set up a github mirror. Uhm. Boring stuff, but still. I'm also kinda shocked that this baby's repo already has around 25Mb ...

P.S.: If you follow that tutorial make sure to turn off mail for this cronjob in crontab. Or run it via daemontools/runwhen. It might migrate this there, but let's see how this works.