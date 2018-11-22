---
layout: post
title: "Closed source, open source. Why closed source software damages the Homebrew scene."
tags: [switch, nintendo, hacking, homebrew]
categories: rants
published: false
---

So it's been three months. So much for frequent blog updates. Anyhoo, here goes.

A lot of people don't seem to be able to fully understand the importance of open source vs. closed source software. As a result, I'd like to share some accounts of closed source software in the Homebrew scene (3DS and Switch) and explain in some detail as to why each and every single one of these products or their developers are not to be trusted.

Before that though, let me quickly explain the difference between open source and closed source.

## Difference

It's actually fairly straightforward. If a program is closed source, you can't look at the source code. If a program is open source, you can look at the source code.

The main advantage of the latter is that it's possible for anyone to check and make sure that you didn't slip anything dangerous in your program. While you can still 100% hold and enforce the copyright on your source, even if it's open, most people make the choice to also license the code under a Free license. A Free license grants others the explicit right to modify and change your code, as long as it is under the same license.

With this established, let's take a look at some Homebrew projects that eiter have gone or are closed source from both the 3DS scene and the Switch scene.

## 3DS scene

### UnbanMii

Holding the dubious honor of the first ever released malware title on the 3DS, UnbanMii can best be defined as a shitshow. Originally intended to be a program that could be used to unban 3DS devices during banwaves, the program was released closed source and shortly afterwards was [revealed to have been leaking console specific data](https://gbatemp.net/threads/all-3-methods-to-get-unbanned-from-recent-ban-wave.450679/page-82#post-7474096) without the users explicit consent.

Combined with the fact that one of the devs quite simply put went extremely unhinged and denied all allegations while the other developers immediatley stepped forward and apologized (as well as nuking the gathered data), this is the first documented case of a Homebrew program going closed source with damaging results towards end-users.

### Themely

Coming in under a close-followup, Themely is another interesting case-study on both how not to behave as a developer and how just not to behave towards a community in general.

Themely was a theme manager for the Nintendo 3DS made by Erman1337, who also ran a site called 3dsthem.es on which themes were hosted. Shortly after releasing UnbanMii, Themely was made closed source. While the source code for the lost open source version can still be found online, the future versions of the program intentionally reverted localization options (done so to get underneath having to get approval from contributors to relicense the GPL code) and were released as closed source software.

This goes in tandem with the fact that Erman claimed about a week before making Themely closed source that "Unbanmii was a genius idea", as well as over the course of the next few months making himself hated by the entire scene. (Alienating GBATemp by claiming he couldn't trust the site after getting warned for making extremist statements, alienating r/3dshacks in much the same manner after attempting to make a reddit thread his new thread, closing all support channels by temporarily hiding the issue tracker, buying up the domain switchthem.es and parking it with gay furry porn, the list kinda continues.)

This all eventually results into Erman unprompted removing 3dsthem.es while not supplying a backup (going against his original promise, although 3dsthem.es was backed up beforehand by an independent group), archiving Themely (before removing it a couple weeks later) and dissapearing completely.

## Switch scene

### SX OS

Just read [here](https://noirscape.github.io/rants/2018/07/05/fuck-tx.html). tldr;

- Stealing code.
- Likely Team Gateway.
- Using shills to defend their product.
- Bricking code in original release.

This is like a checkbox list of why closed source software in the homebrew scene is dangerous.

### DZ

Without going into the general unhinged nature of the developer behind this tool, DZ was eventually renamed to Tinfoil™ after the original developer for Tinfoil (Adubbz) quit working on Tinfoil.

Then blawar (the DZ developer) claimed to have trademarked the name Tinfoil, which resulted in the more or less "official" fork by XorTroll having to be [renamed](https://gbatemp.net/threads/community-name-vote-suggestions-for-tinfoil.522399/). Later it was found that no official trademark exists in TESS, yet the rename went through anyway, renaming the fork to GoldLeaf.

Yikes.

## Conclusion

Don't run closed source software on a homebrew device
