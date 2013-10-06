---
layout: post
title: Linux and Me
---
I'd like to start off this blog-post with a lot of swear words, some of which you might have never heard. Others, that might make you blush. But I won't, I'm trying to be professional here, people.

There are many articles on Linux, so I am not going to write a detailed explanation of what Linux is and is not. If you don't know what [Unix][] or a [distribution][distro] is, if you have no clue about [FOSS][] and [GNU][], please, consult [Wikipedia][wikiplinux] before reading on, as I am not going to define terms like these.

## So, What's the Problem&#8253;
I wanted to set up a development environment using *Ubuntu 10.10*. I'm doing a project with OpenStreetMap for my Bachelor thesis, and I thought I needed the [mapnik] rendering tool chain to run on my development machine. So I went out to install Ubuntu on the old work laptop of my girlfriend, rad little [HP Compaq 2510p][c2510p]. This is where things started going wrong.

My variant of this 12'' notebook is equipped with an *Intel Core 2 Duo ULV Processor* with *1.20 GHz*, *2 GB* of DDR2 RAM and the *Intel GMA X3100* integrated graphics chip. Everything installed fine right out of the box. Put in the Ubuntu DVD, installed the system and was ready to go within the hour. But somehow the current kernel has problems with the soft-buttons the *2510p* is equipped with. They don't work most of the time, and the volume slider is hit and miss at best. That wouldn't matter too much, since I don't like soft buttons and don't use them, but when the touchpad stopped working after awaking the notebook from sleep, I knew something was fishy. Since I thought that maybe an update or myself fucked things up, I decided to reinstall.

That didn't help. Happy with my squeaky-clean install, I worked a bit, sent it to sleep, some problem after reawaking it. I still wanted to go on. So I went ahead, reinstalled it and made sure that I was using suspend to RAM and not suspend to disk like I did before. Shutting the thing down every evening sure would suck, but I didn't want to reboot every time I take a break from work, since I usually send my notebook to suspension when I do. Some problem after the first reboot.

Since I had now established that reinstalling the machine wouldn't help, I decided to just make do with what I had, and use the mouse. This worked fine for about half a week. Then *Ubuntu 11.04* was released. Curious about Unity, I went ahead and upgraded from *10.04* to *11.04*. Shouldn't have done that. After installing a proprietary driver for the graphics chip, unity wouldn't start anymore. At least I think it was the graphics driver. After trying a few things to fix this and the soft-button issue I found on various forums, I decided that I would reinstall this machine one more time.

I went ahead and installed Ubuntu 11.04 from scratch. When I booted the first time, everything was fine. Starting installing the software I needed, took the PC to the university to show some of the progress I was able to make to my thesis-advisor Wilfried. This is when I make the error that will end my little experiment with Linux: I want to power down the PC, and touch the soft-button for the WiFi & Bluetooth instead. (Yes, I know that's anywhere near the power button, but I was sleepy and not paying attention.) Of course, the WiFi-card is deactivated. This is supposed to happen. When I see that I pressed the wrong button, I go ahead and try to reactivate the WiFi before shutting the notebook down. **I couldn't**. The button stopped working after the first press, and I was not able to get it working again. And I tried, for about a day.

This, and the fact that we had in the meantime managed to set up a server running Ubuntu 11.04 and the tools that we need plus OpenSSH, was the cue for me to minimize my losses and just **stop** this right when it was becoming ridiculous. I really tried to make this work, but it just shouldn't be. Just like my last adventures with Suse or Arch or (K)Ubuntu (8.04, 9.04, 9.10).

I really like the idea of FOSS, and Linux. And maybe I am just too stupid -- which I don't believe, since I can use the server without any problems -- or too stuck on windows -- again, see argument one -- to make this work. Whatever it is, I am **done** with trying to use Linux as an operating system for development and university. It's just not worth the hassle for me. I'm going to stick with Windows 7 -- which is great, by the way -- until I get myself a MacBook Pro or a new Laptop running Windows 8. I like my Linux the way I like my sewer plants: far away, and only with a remote connection.

[gnu]:			http://en.wikipedia.org/wiki/GNU_General_Public_License
[foss]:			http://en.wikipedia.org/wiki/Free_and_open_source_software
[distro]:		http://en.wikipedia.org/wiki/Linux_distribution
[unix]:			http://en.wikipedia.org/wiki/Unix
[wikiplinux]:	http://en.wikipedia.org/wiki/Linux
[mapnik]:		http://mapnik.org/
[c2510p]:		http://h20000.www2.hp.com/bizsupport/TechSupport/Document.jsp?objectID=c01057682&lang=en&cc=us&taskId=101&prodSeriesId=3355633&prodTypeId=321957