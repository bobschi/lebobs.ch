---
layout: default
title: Choosing a Boilerplate for Responsive Design
---

Having no options is about as bad as it gets. But sometimes, there's just too many to choose from. Yes, I know, first world problem. But a problem nonetheless. I think Randall Munroe over at [xkcd][] really nailed my current problem in his comic ["Brand Identity"][xkcdbrandsrc]:  
<img src="http://imgs.xkcd.com/comics/brand_identity.png" width="600"/><!--![xkcd: Brand Identity][xkcdbrand]-->

I know that the title promised you juicy bits of information about various Frameworks or Boilerplates for Responsive design, but bear with me for a moment. The choices out there are vast. To name a few: [320 and up][320andup], [LESS 4][less4], [foundation][foundation], [MQ Framework][mqframework], [Golden Grid][goldengs], [Fluid Baseline Grid][fbg], [Columnal][columnal], [The Semantic Grid System][semanticgs], [1140px CSS Grid][cssgrid], [The Goldilocks Approach][goldigs], [Inuit][inuit], [BluCSS][blu], [Frameless][frameless], [Gridless Boilerplate][gridless], [Amazium][amazium], [Skeleton][skeleton], [Mobile Boilerplate][html5mp] and [Tiny Fluid Grid][tinyfluid], to name those I know and will talk about. To top it of, you might need to rely on scripts like [respondjs][], [html5shiv][] or [modernizr][] to make sure everything works at the client side. Like when trying to decide which yoghurt to buy, one is confronted with a plethora of choices that all promise lots of things, like a healthier digestive tract, weight loss or better chances with prospective partners. All you have to do is to choose, after weighing all the pros and cons in your head, while all you want is a Simple Responsive Grid(TM).

<!--more-->

*If you just want to browse through the list of frameworks, please [jump right on in](#thelist). If you are wondering about the thinking behind it, please consult [this part](#norantyranty) of this post.*

When I hacked together the old red-white-black skin of my block last year, I quickly decided upon using [HTML5Boilerplate][html5bp] with [320 and up][320andup], since [Mobile Boilerplate][html5mp] didn't exist back then, I was just to stupid to find it or I don't remember correctly. Doesn't really matter. I made a choice, went with it, and became progressively more unhappy with it. I never learned to use the HTML5 Boilerplate tool set at all. At that time, I just didn't have the time to figure *all* the stuff out, I had my head full and just wanted something that worked well, and I wanted it fast.

But upon revisiting my decision late in December, when thinking about a redesign as the current red-white-black one has so many flaws, I really began to regret the choice. While it was too feature rich, simply too much back then, it was even now, with my head pretty much free and focused on the task at hand. So my quest for the One True Boilerplate/Framework(TM) began. And it has not yet ended ...

<h2 id="norantyranty">Asking the Right Questions</h2>

This will come to no surprise to you, but out from the mass of questions that we might ask--"Why am I reading this?", "When will we finally get to the interesting part?" or "What framework should I pick? Am I making the right choice?"--the last ones are not amongst those that I would consider "correct". The most important question is "What problem am I trying to solve, and how can the framework or boilerplate help me with that?". Others might be "Do I want a framework or a boilerplate?", "Is this too complicated?", "Is there documentation? Is it good?", "Are there tools, like bookmarklets?" or "Is this still being developed or is it already dead and forgotten?".

While I can not answer the most important question for you, I certainly can provide some answers to the later questions, that might help. To give you an idea of what I am looking for, I will answer the most important question before I'll continue to the overview:

> I am looking for a boilerplate that comes with a responsive grid, a reset CSS and sensible typographic basics. I don't want a full-fledged framework.

<h2 id="thelist">The List</h2>

I will be assigning one of two categories to each item on the following list. 'boilerplate', for packages that do a few basic things. 'framework' for packages that are more feature-rich, offer additional tools like their own build tools, and make a lot of assumptions about the things that you may use, and add things like jQuery pre-emptively.

### [320 and up][320andup] <small>\#framework</small>

![On desktop at 480 x 1024 px][320andup480x1024]  
![At desktop at 1280 x 1024 px][320andup1280x1024]

You can either use this as an extension of HTML5 Boilerplate or Mobile Boilerplate, or as a standalone kit. It is a device agnostic boilerplate. It includes a grid system based on LESS Framework 4 and features five media query increments at 480 px, 600 px, 768 px, 992 px and 1382 px, allowing for very grained fine control, and has media queries in place to serve up higher resolution content for higher resolution displays. There are two different versions available, one with multiple linked style sheets and another one with one style sheet with multiple media queries. It has some typography defaults in place.  
![On iPhone, portrait ][320andupiphonep]  
![On iPhone, landscape ][320andupiphonel]

* License: [MIT license][mit]
* Current Version: 2.04 committed to github on [November 22nd, 2011][320andupgh]
* Last Commit: November 22nd, 2011 on [github][320andupgh]
* Size on disk: 284 KB multiple style sheets and 236 KB for single style sheet
* Additional resources: comes with a background image for the grid at highest width as well as the LESS-sources for the styles.
* Well documented code!

This is a very, very handy tool. But it is as complicated as it is powerful. For the different versions, there are five JavaScript libraries included--imgsizr, jquery-1.6.2.min, modernizr-2.0.6.min, respond.min & selectivizr.min--and the code that you need to work through is spread over eleven or five files: one index file showing you how to wire things up, two JavaScript files as well as eight or two CSS files respectively. If you want to use the .LESS-files, you need to install a less compiler.  
![On iPad, portrait][320andupipadp]  
![On iPad, landscape][320andupipadl]

A nice touch: if you dig around the images that come with the framework, you are practically delivered a check list and manual about what images you are going to need to provide optimal experience for iOS users.

Personal opinion: While it seems very well designed, robust and well coded, and worked great for me in the past, I have realized that it is simply too much for me. First responsive framework I tried, and pretty nice to use. Seems very robust and well coded to me.

### [1140px CSS Grid][cssgrid] <small>\#boilerplate</small>

![][cssgrid480x1024]  
![][cssgrid1280x1024]

The 1140px CSS Grid System includes a grid of twelve columns with gutters "about 40 px wide at full width" ... The 1140  CSS Grid was designed to work best on 1280 px monitors,  with realignment of columns for lower resolution screens. The grid system itself consist of three CSS files: one for the grid, one for you styles and one for Internet Explorer compatibility. There are two media query increments, one at 767 px and one for 767 px up to 1440 px, the maximum width of the grid. Another media query is in place so you can provide higher resolution assets for Retina Display devices like the iPhone 4S.  
![][cssgridiphonep]  
![][cssgridiphonel]

* License: [CC BY-SA 3.0][ccbysa3au]
* Current Version: 2.0
* Last Commit: unknown, no public repository available.
* Size on disk: 36 KB
* Additional Resources: PhotoShop Template (based on how the grid renders in WebKit)

Personal opinion: I love the fact that this boilerplate is so spartan and small. Just three files that you need to include, only one dependency, the css3-mediaqueries script to enable media queries in browser that don't support them. This should be pretty fast!  
![][cssgridipadp]  
![][cssgridipadl]

But there where a few things that I didn't like: The author included those pesky hidden OS X folders (__MACOSX) and files (.DS_STORE) into the ZIP. Sloppy. If you have a page using the grid open in a WebKit-browser on iOS turning the device from portrait in to landscape mode will break the layout engine. Also, I don't really like the fact that there is no public repository for this

### [Amazium][amazium] <small>\#framework</small>

![][amazium480x1024]  
![][amazium1280x1024]

Amazium comes packed with 960.gs. Four media queries adjust the layout of your website to your view port. It comes with a reset.css, as well as some basic typographic styles. Nice detail: custom styles for bullet points, Trademarks, subtext as well as styles for buttons and blockquotes. Amazium also provides default styles for forms and tables. It provides image resizing out of the box, as well as resizing of YouTube and Vimeo embeds! Another nice touch: a 404 page is included as well. It comes packing various jQuery-plugins, while jQuery itself is pulled from Google's CDN.  
![][amaziumiphonep]  
![][amaziumiphonel]

* License: couldn't find any
* Current Version: 1.0 
* Last Commit: September 17th, 2011, see the changelog on the homepage
* Size on Disk: 184 KB

Personal opinion: One thing I noticed on the iPad as well as on my iPhone was that when switching between landscape and portrait mode there were about two to three seconds when I couldn't take a screen shot. Apparently, some resources where being downloaded. Part of the screen stayed white for about a second, until the layout was resized. Please remember, those are highly personal impressions, that might just mean that my iPhone 3Gs is getting really old and that, maybe, I should replace it. But all in all, I like it. It's pretty, and seems functional and robust.  
![][amaziumipadp]  
![][amaziumipadl]

Due to the fact that I could not find any information about the license, I would strongly **advice you against using it**, as whatever license the author might choose in the future might not be compatible with your requirements.

### [BluCSS][blu] <small>\#boilerplate</small>

![][blucss480x1024]  
![][blucss1280x1024]

BluCSS features for distinct stages of size: desktop, laptop, tablet and mobile, realized via media queries. The grid resides in a container 1000 px wide and has ten columns. After applying Eric Meyer's reset CSS, BluCSS applies some basic styles, which might not be everybody's cup of tea. Responsive image resizing comes included, and is realized through classes. No JavaScript, very spartan.  
![][blucssiphonep]  
![][blucssiphonel]

* License: couldn't find any
* Current Version: unclear
* Last Commit: unclear
* Size on Disk: 16 KB

Personal Opinion: Very spartan, very minimal, which is great. The basic styles are not my cup of tea, so I would remove those if I were to work with it.  
![][blucssipadp]  
![][blucssipadl]

The absence of a license worries me. I like things stated explicitely. If you publish something, please make sure to explicitely state what people may do and what people may not do to whatever you are publishing. Licenses are a great tool for that. If you don't care about putting your projects under the protection of a license, just say so: "No license, public domain. Have fun!".

### [Columnal][columnal] <small>\#boilerplate</small>

![][columnal480x1024]  
![][columnal1280x1024]

According to Columnal's homepage, it's grid system is a remix of various other systems, most notably [1140px CSS Grid System][cssgrid]'s fluid grid with a width of 1140px and 960.gs' subcolumns. Per expectation, it's grid is divided into twelve columns. It won't work in Internet Explorer 6 to 8, though, which degrade to a fixed width layout. Image and video resizing is built in, as well as some basic typographic styles.  
![][columnaliphonep]  
![][columnaliphonel]

* License: [CC BY-SA 3.0][ccbysa3us]
* Current Version: 0.85
* Last Commit: Appears to have happened on November 22nd, 2011
* Size on Disk: 68 KB
* Additional tools: A PDF to be printed, to help you sketch your project. Wireframing templates, for Adobe Illustrator and Balsamiq Mockups! AWESOME!

Again, a rather spartan boilerplate. Includes Eric Meyer's reset.css version 2.0. No JavaScript, just CSS. Awesome. Only two caveats: it consists of 9 CSS files, which means a lot of http-requests when loading the page, and, alas, Columnal too has got problems with switching from portrait to landscape mode on my iOS devices.  
![][columnalipadp]  
![][columnalipadl]

Personal opinion: I love the goodies, and the ideas seem pretty solid. I loooooove the goodies you get. However, I never warmed up towards 960.gs or 1140px CSS Grid System, so I guess I will not try this.

### [Fluid Baseline Grid][fbg] \#framework

![][fbg480x1024]  
![][fbg1280x1024]

Fluid Baseline Grid features a minimal three-column folding grid, with columns 31.333% wide and gutters at 2% width between the columns. It was build with the ideals of fluid-column layouts, baseline grids and mobile-first responsive design in mind. It's resolution independent and device agnostic. It comes with very nice typographic standards in place, after using normalize.css to preserve useful defaults and fix common bugs and inconsistencies. The six size stages are realized through media queries in a central style sheet. Respond.js is in place to fix issues with IE6/7/8.  
![][fbgiphonep]  
![][fbgiphonel]

* License: [The Unlicense][unlicense]
* Current Version: 1.0.1
* Last Commit: October 24th, 2011 on [github][fbggh]
* Size on Disk: 64 KB

Fluid Baseline Grid makes a lot of assumptions about what you are going to use: Google Analytics is included into the example index.html. Again, Switching from portrait to landscape seems to break the layout on iOS, which is kinda annoying.  
![][fbgipadp] .
![][fbgipadl]

Personal opinion: It seems very well documented, with sensible defaults in place. There is even a future reading section on the page. I also love how every big design decision is explained, followed with a pointer to instructions on how to change stuff, if you don't like it. I guess this is one of the favourites to be included in my html5-jekyll-boilerplate, despite the obvious problems I could identify for me.

### [foundation][foundation] \#framework

![][foundation480x1024]  
![][foundation1280x1024]

Foundation is one of the most mature frameworks I have come across so far. Currently at version 2.1, it has become very powerful. It has a solid in place, which is divided into twelve columns, and a mobile grid which is divided into four columns. There are nice default styles in place for about everything you can think of: buttons, forms, typography, even UI-elements like panels and alerts. This is much more than a simple responsive grid boilerplate, it is a framework for web and web app development as well as a sophisticed rapid prototyping tool. It sports orbit, a jQuery image slider tool and Reveal for modals,  
![][foundationiphonep]  
![][foundationiphonel]

* License: [MIT license][mit]
* Current Version: 2.1
* Last Commit: January 21st, 2012 on [github][foundationgh]
* Size on Disk: 244 KB
* Additional Tools: Gems for Ruby on Rails and Compass/SASS!

The framework is very, very well documented with examples and a nice little Q&A page. However, to harness it's full power, you will need to learn the specifics of this very powerful framework. Maybe installing SASS and Compass might not be a bad idea, which in my eyes makes the learning curve very steep for this framework. But the benefits might be worth it, as you gain a very powerful tool.  
![][foundationipadp]  
![][foundationipadl]

Personal opinion: exceptionally powerful and interesting tool. I would love to try this out, especially because of the very solid basic styles and grid.

### [Frameless][frameless] \#boilerplate

![][frameless480x1024]  
![][frameless1280x1024]

Even if its creator answers the question "Is Frameless responsive" with a definitive no, as it's grid is fixed width, not fluid, I guess it falls into the broader definition that I incorporated for this selection. The design principles are explained in detail on the page, as they differ a bit from what logic is generally used to design grids.  
![][framelessiphonep]  
![][framelessiphonel]

* License: [CC0][cc0]
* Current none
* Last Commit: December 19th, 2011 on [github][framelessgh]
* Size on Disk: 12 KB
* Additional Tools: A PhotoShop file for a grid with 48 px wide columns and 24 px wide gutters, guides for columns up to 2560 px as well as overlay masks for some screen sizes.

What really bothers me is the fact that there is no "compiled" CSS version of Frameless, only LESS and SCSS templates. However, the reason for this gets clearer, once you browse through the source code. Installing a simple gem and learning LESS and SCSS won't hurt.. 
![][framelessipadp]  
![][framelessipadl]

Personal opinion: I dig the simplicity. It's minimal and to the point. It might be an interesting choice for me, although I initially wanted to stay away from LESS and SCSS.

### [Gridless Boilerplate][gridless]
### [Golden Grid][goldengs]
### [The Goldilocks Approach][goldigs]
### [HTML5 Boilerplate][html5bp]
### [HTML5 Mobile Boilerplate][html5mp]
### [Inuit][inuit]
### [Less 4][less4]
### [MQ Framework][mqframework]
### [The Semantic Grid System][semanticgs]
### [Skeleton][skeleton]
### [Tiny Fluid Grid][tinyfluid]

Further Reading
---------------

* [15 Responsive CSS Frameworks Worth Considering](http://bit.ly/15frameworks)
* [10 Tools & Frameworks for Responsive Design](http://bit.ly/10frameworks)
* [Less Framework 4 -- An adaptive CSS grid system](http://bit.ly/less4)
* [Zurb Foundation](http://bit.ly/zurbfoundation)
* [320 and Up -- The ‘tiny screen first’ boilerplate extension](http://bit.ly/le320andup)
* [Adactio: Journal--One Web](http://bit.ly/AqIxvb)

[speckyboy]:		http://bit.ly/15frameworks
[fuelurcoding]:		http://bit.ly/10frameworks
[oneweb]:			http://bit.ly/AqIxvb
[xkcdbrandsrc]:		http://xkcd.com/993/
[xkcdbrand]:		http://imgs.xkcd.com/comics/brand_identity.png
[xkcd]:				http://xkcd.com/
[csswhiz]:			http://bit.ly/therealhtml5bp
[csswhizpi]:		http://bit.ly/therealhtml5bpcomments

[320andup]:			http://bit.ly/le320andup
[320andupgh]:		http://bit.ly/320andupgh
[amazium]:			http://bit.ly/amazium
[blu]:				http://bit.ly/blucssgs
[cssgrid]:			http://bit.ly/cssgs
[columnal]:			http://bit.ly/columnal
[fbg]:				http://bit.ly/fluidbaseline
[fbggh]:			http://bit.ly/fluidbaselinegh
[foundation]:		http://bit.ly/zurbfoundation
[foundationgh]:		http://bit.ly/zurbfoundationgh
[frameless]:		http://bit.ly/frameless
[framelessgh]:		http://bit.ly/framelessgh
[goldengs]:			http://bit.ly/goldengs
[goldigs]:			http://bit.ly/goldigs
[gridless]:			http://bit.ly/grdless
[html5bp]:			http://bit.ly/html5plate
[html5mp]:			http://bit.ly/mobileplate
[inuit]:			http://bit.ly/inuitgs
[less4]:			http://bit.ly/less4
[mqframework]:		http://bit.ly/mqframework
[semanticgs]:		http://bit.ly/semanticgs
[skeleton]:			http://bit.ly/skeletn
[tinyfluid]:		http://bit.ly/tinyfluid

[respondjs]:		http://bit.ly/rspndjs
[html5shiv]:		http://bit.ly/html5shiv
[modernizr]:		http://bit.ly/mdrnizr

[mit]:				http://opensource.org/licenses/mit-license.php
[ccbysa3au]:		http://creativecommons.org/licenses/by/3.0/au/
[ccbysa3us]:		http://creativecommons.org/licenses/by-sa/3.0/us/
[unlicense]:		http://unlicense.org
[cc0]:				http://creativecommons.org/publicdomain/zero/1.0/

[320andup480x1024]:		http://placehold.it/600x140
[320andup1280x1024]:	http://placehold.it/600x140
[320andupiphonep]:		http://placehold.it/600x140
[320andupiphonel]:		http://placehold.it/600x140
[320andupipadp]:		http://placehold.it/600x140
[320andupipadl]:		http://placehold.it/600x140

[cssgrid480x1024]:		http://placehold.it/600x140
[cssgrid1280x1024]:		http://placehold.it/600x140
[cssgridiphonep]:		http://placehold.it/600x140
[cssgridiphonel]:		http://placehold.it/600x140
[cssgridipadp]:			http://placehold.it/600x140
[cssgridipadl]:			http://placehold.it/600x140

[amazium480x1024]:		http://placehold.it/600x140
[amazium1280x1024]:		http://placehold.it/600x140
[amaziumiphonep]:		http://placehold.it/600x140
[amaziumiphonel]:		http://placehold.it/600x140
[amaziumipadp]:			http://placehold.it/600x140
[amaziumipadl]:			http://placehold.it/600x140

[blucss480x1024]:		http://placehold.it/600x140
[blucss1280x1024]:		http://placehold.it/600x140
[blucssiphonep]:		http://placehold.it/600x140
[blucssiphonel]:		http://placehold.it/600x140
[blucssipadp]:			http://placehold.it/600x140
[blucssipadl]:			http://placehold.it/600x140

[columnal480x1024]:		http://placehold.it/600x140
[columnal1280x1024]:	http://placehold.it/600x140
[columnaliphonep]:		http://placehold.it/600x140
[columnaliphonel]:		http://placehold.it/600x140
[columnalipadp]:		http://placehold.it/600x140
[columnalipadl]:		http://placehold.it/600x140

[fbg480x1024]:			http://placehold.it/600x140
[fbg1280x1024]:			http://placehold.it/600x140
[fbgiphonep]:			http://placehold.it/600x140
[fbgiphonel]:			http://placehold.it/600x140
[fbgipadp]:				http://placehold.it/600x140
[fbgipadl]:				http://placehold.it/600x140

[foundation480x1024]:	http://placehold.it/600x140
[foundation1280x1024]:	http://placehold.it/600x140
[foundationiphonep]:	http://placehold.it/600x140
[foundationiphonel]:	http://placehold.it/600x140
[foundationipadp]:		http://placehold.it/600x140
[foundationipadl]:		http://placehold.it/600x140

[frameless480x1024]:	http://placehold.it/600x140
[frameless1280x1024]:	http://placehold.it/600x140
[framelessiphonep]:		http://placehold.it/600x140
[framelessiphonel]:		http://placehold.it/600x140
[framelessipadp]:		http://placehold.it/600x140
[framelessipadl]:		http://placehold.it/600x140