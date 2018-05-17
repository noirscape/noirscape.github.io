---
layout: post
title: "Fixing WASD in vidya games on Linux"
categories: guides
tags: [linux, wasd, keyboard, xset]
image: http://ev1l0rd.github.io/images/code.jpg
---

Sup guys. It's me. Again. Yeah I still suck at openings. What else is new!

Anyway, here's just a fairly short fix for something that I have been stumbling over while playing Video Games on Linux for a while now and that is that when I use the WASD keys to control my character in some video games, it basically does repeat pressses causing the character to glitch forward instead of walking. At first I blamed my shitty keyboard for it (which had other issues such as ghosting as well) but when the issue appeared again on my new keyboard, I decided to look deeper into it. In the end I was able to find the solution: While the game is running, open a Terminal and run

> xset r off

This disables the repeating key behavior in X11. In order to make it permanent (not tested as I do need repeated keys for other tools) create a file at `~/.xinitrc` and put the above command in it. Then make sure it's marked as executable (`chmod +x ~/.xinitrc`) and then X11 should apply it automagically whenever you start it. This might override some other settings you have in other X11 config files, so take care before doing that. ([Credits to Tom Wijsman on StackOverflow](https://superuser.com/a/864156/424839)).

Anyway that's my quick fix for this time. Hope you get some use out of it!

~ Valentijn
