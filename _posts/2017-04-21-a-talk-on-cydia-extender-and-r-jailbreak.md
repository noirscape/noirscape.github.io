---
title: A talk on Cydia Extender, Ext3ndlife and /r/jailbreak.
layout: post
categories: rants
tags: cydia, jailbreak, julioverne
image: https://upload.wikimedia.org/wikipedia/commons/0/09/Cydia_Startseite.png
---

Sup ladies and gentleman. How are you? (I'm fine thanks for asking). It's been a while since this blog has been upd8'ed, but don't think I've gone silent. In fact, today I'm here with you for a completely new topic. Namely, Cydia Extender.

In case you aren't aware (which in this case is likely, since I don't talk about it too much), I love jailbreaking. I hate Apple's strict lockdown on iOS, their complete unwillingness to allow anything that is not distributed through their Store and the inability to modify the system beyond a few standard options.

Thankfully, there is a solution. Jailbreaking. The iOS equivalent to Homebrewing a console, jailbreaking is tons of fun and makes you learn a lot about the system as a whole. Unfortunately, Apple really hates jailbreaking and the security exploits used are patched with each system upd8 (not that I blame them. Fixing gaps in your security is an important thing, especially with phones which for most of us is not just a device to call others with, but a device to store our credentials on, read mail and so on. Effectively it's a second PC.)

The two most recent jailbreaks (iOS 9's Pangu and [Qwertyoruiop](https://yalu.qwertyoruiop.com/)'s Yalu) both were distributed as IPA's and require Apple's ability to allow you to compile any app for any device with a dev certificate. Unfortunately, unless you have a 100$ dev account, the IPA's would be de-signed in a week and were unusable on the device unless you manually reinstalled them. Pangu was able to work around it by from what I could gather is by changing the certificate to an already expired one and then blocking the check servers (note: this might be complete hogwash, but that was what I was able to gather from it! If it is, do not hesitate to contact me so I may improve this sentence).

Unfortunatley Yalu has no such workarounds and the IPA must be reinstalled once a week. Even though there are tools that can extend development certificates (like say [Immortal](cydia://package/com.ahmda.immortal) (link requires BigBoss repo which is one of the defaults), these tools require a jailbreak just to be functional.

As a result, people wanted an alternative from running [Cydia Impactor](http://www.cydiaimpactor.com/) every week to keep their jailbreak. At some point 'saurik' (the person behind Impactor and Cydia itself) heard the voices and in an update released with Impactor a couple months ago, Impactor included a tool called 'Cydia Extender'. Unfortunately for both saurik and the jailbreaking community, Cydia Extender was quickly proven to be utterly useless as it required a developer account to function (which is useless because developer accounts get 1 year certificates, rather than 1 week certificates).

At the time of releasing Impactor, saurik wrote the following two reddit comments towards the Jailbreak community: 

<div class="reddit-embed" data-embed-media="www.redditmedia.com" data-embed-parent="false" data-embed-live="false" data-embed-uuid="970bb857-7de2-41ca-b88a-2e9544bcf999" data-embed-created="2017-04-21T15:53:52.935Z"><a href="https://www.reddit.com/r/jailbreak/comments/5yrw0i/discussion_cydia_impactor_issues_fixed_and/desgj2u/">Comment</a> from discussion <a href="https://www.reddit.com/r/jailbreak/comments/5yrw0i/discussion_cydia_impactor_issues_fixed_and/">[Discussion] Cydia impactor issues fixed and includes Cydia Extender.Does anyone know what it is?</a>.</div><script async src="https://www.redditstatic.com/comment-embed.js"></script>

<div class="reddit-embed" data-embed-media="www.redditmedia.com" data-embed-parent="false" data-embed-live="false" data-embed-uuid="752b6971-cd7d-4241-b4bb-c57529d26488" data-embed-created="2017-04-21T15:54:15.055Z"><a href="https://www.reddit.com/r/jailbreak/comments/5yrw0i/discussion_cydia_impactor_issues_fixed_and/desgtx9/">Comment</a> from discussion <a href="https://www.reddit.com/r/jailbreak/comments/5yrw0i/discussion_cydia_impactor_issues_fixed_and/">[Discussion] Cydia impactor issues fixed and includes Cydia Extender.Does anyone know what it is?</a>.</div><script async src="https://www.redditstatic.com/comment-embed.js"></script>

(Cited in case saurik edits the comments):
> 1) Cydia Extender is not the thing you think it is. 2) Cydia Extender apparently also isn't the thing I thought it was.

> To the extent to which this project was potentially exciting, it essentially became a complete failure five minutes after release, so I'm just going to go to bed and leave it all very vague :/. (Maybe someone else will determine a way in which it is useful ;P.)

In particularly the last sentence gave the Jailbreak community the idea that, if anything, Saurik left the community Cydia Extender for them to modify it to make it work. As a result, multiple people jumped to work on it, and in the next few months various little tools were released that would make Cydia Extender work. However, all of these tools faded when the notorious cracker [julioverne](https://twitter.com/julioverne) got to work on Cydia Extender. Not only did he made the tool work by creating a tweak called Extendlife, he also heavily improved Cydia Extender (and rebranding it to Ext3nder) and made it all possible to install simply by installing two deb files. (Most other utilities required manual user interaction from the teminal, whereas Ext3nder and Extendlife are fully installed and functional from a deb package).

Of course such a great tool and utility would see lots of applause from the Jailbreak community (primarily /r/jailbreak) right? 

Well... sorta. Whereas on /r/jailbreak everyone did applaud the creation of Ext3nder and Extendlife, no actual posts could be made on these tools, as these tools were hosted on verne's repository, which also contained a major crack tweak. As a result, verne's tool as good as it was, could not see any recognition from the biggest jailbreaking community. That is until the following reddit post was made:

<blockquote class="reddit-card" data-card-created="1492790648"><a href="https://www.reddit.com/r/jailbreak/comments/6335zc/meta_he_who_must_not_be_named/?ref=share&ref_source=embed">[Meta] He Who Must Not Be Named</a> from <a href="http://www.reddit.com/r/jailbreak">jailbreak</a></blockquote>
<script async src="//embed.redditmedia.com/widgets/platform.js" charset="UTF-8"></script>

Long story short, the user in question made a plea for explanation from the mods, mentioning that in fact this way of interpreting the rules is in fact kinda stupid.

The mods responded with this comment:

<div class="reddit-embed" data-embed-media="www.redditmedia.com" data-embed-parent="false" data-embed-live="false" data-embed-uuid="d0cfc9a4-db8f-489f-9167-232c486ec94f" data-embed-created="2017-04-21T16:04:55.954Z"><a href="https://www.reddit.com/r/jailbreak/comments/6335zc/meta_he_who_must_not_be_named/dfr7ljp/">Comment</a> from discussion <a href="https://www.reddit.com/r/jailbreak/comments/6335zc/meta_he_who_must_not_be_named/">[Meta] He Who Must Not Be Named</a>.</div><script async src="https://www.redditstatic.com/comment-embed.js"></script>

In which they utterly proved the points made in the thread and proved to 'take a closer look at the tool and put it up for discussion with the mods'. 

Skip forward about 8 days and this post was made on /r/jailbreak: 

<blockquote class="reddit-card" data-card-created="1492790830"><a href="https://www.reddit.com/r/jailbreak/comments/64ogpo/meta_update_regarding_status_of_ext3nder_tldr/?ref=share&ref_source=embed">[Meta] Update regarding status of Ext3nder (tl;dr: Nothing has changed)</a> from <a href="http://www.reddit.com/r/jailbreak">jailbreak</a></blockquote>
<script async src="//embed.redditmedia.com/widgets/platform.js" charset="UTF-8"></script>

(cited in case they backpedal on the post:)

> As many are aware, we have not been allowing posts about Ext3nder as it is currently hosted on a repo that contains piracy. We’ve been asked several times if we would allow it if it was hosted on another repo that has nothing to do with piracy.

> Major discussion can be found here.

> Previously we had said this would be okay, but before making it official, we had to verify the claim that many were making that Saurik “encouraged modifications to Cydia Extender.” It turns out that his words were misinterpreted, as is often the case with this type of thing. Saurik clarified to us that this statement was “only about modifications to Launch Services and Mobile Installation.” Additionally, he said “I also would be upset at someone redistributing Extender in a modified form (as opposed to modifying it using any kind of runtime extension).”

> After inspecting both the Cydia Extender and Ext3nder executables in a disassembler, we found that Ext3nder was indeed just a modified version of Cydia Extender, rather than a tweak for Cydia Extender.

> Because of this, Ext3nder will not be allowed on /r/jailbreak regardless of where it is hosted.

> We understand that this decision is unpopular and will upset many people, but as mods we are obligated to enforce the rules and follow Saurik’s wishes.

> - /r/jailbreak mod team


In short, they asked sauriks stance on the matter, and **while contradicting earlier comments made by saurik** he claimed that he did not want anyone but him working on Cydia Extender and he would dislike any modifications to the tool that weren't 'runtime edits'.

Yeah. Let that sink in for a moment. Saurik claimed that he was against editing the comment and that the statement was 'misinterpreted'. I... wow. I have cited sauriks comments earlier. Go read that. Saying that your statment was misinterpreted, while your original statement had a rather clear implication attached to it (in this case "go on ahead guys, do your best to make it work in whatever way possible, I already tried but failed, go for it!") is backpedaling on your statements and being self-contradicting.

I'm sorry, but on this matter I am going to be very honest here: I hold no respect for saurik on this subject. This change in statements gives out the implication that he is pissed that someone else improved Extender and as a result forbids modifications of Extender.

I also hold no respect towards the /r/jailbreak mods on this matter. I get why you forbid privacy. Reddit doesn't want to be a part of DMCA's, I can get that. I get that Ext3nder is hosted on a pirate repo with a dev infamous for cracking making it. But what I don't get is why you utterly forbid and censor anyone who dares to talk about a tool that isn't even fucking piracy in the first place. You guys allow AppSync posts, despite the fact that about 99% of all AppSync users use the tool for pirated apps (shut up, this is true. hell the dev said things to that extend. if you dont use it for that, good on you, now take your cookie and listen.). You guys allow jailbreaking (obviously given the sub), despite it's legal gray area.

Yet you fuckers purge the mentioning of a tool that many users demanded to work, just because saurik has a petty grudge because someone made Extender work that wasn't him. I understand that saurik is one of the (if not THE) most important devs in the jailbreaking community and losing him might be a hard blow to your subreddit, but you guys to me are UTTER SPINELESS RATS WHO PANDER SPECIFICALLY TO DEVELOPERS AND IGNORE YOUR OWN USERBASE. As a result, I hold NO FUCKING RESPECT for you guys. You worms.

My final message to the mods of /r/jailbreak: Fuck you.

My message to saurik: Grow a pair and get over it. Someone made Extender work. That person wasn't you. Deal with it.

Oof. Needed to get that out of my system! Having said all that, I personally highly recommend Ext3nder and Extendlife. They're straightforward to setup, so use your Google-fu and figure out how to do it (I'm not gonna describe it, bc I don't want someone pissing on the repo with a DMCA strike because the repo contains a cracking tweak).

--
Header image courtesy of Wikimedia Commons.[^1]

[^1]: The usage of this image does not imply that Wikimedia or the uploader endorses my work.
