---
layout: post
title: Getting out of Emergency mode on Ubuntu 17.04
image: http://ev1l0rd.github.io/images/Code.jpg
---

Note: This was executed on Ubuntu 17.04. Instructions may differ if you do not run Ubuntu.

So here's an interesting little conundrum that took me a little while to solve. When I booted my PC this morning, I was not greeted by my login screen, rather I was greeted by the following message: "FSCK for /dev/sdc1 failed. Please run again MANUALLY" (or something to those lines). Thankfully, there was a note on what command to execute (`fsck -fy /dev/sdc1` for the curious). So I ran the command. Realizing that FSCK is the rough equivalent of Windows' CHKDSK for ext4 filesystems, I ran it twice for good measure. I rebooted. And I was greeted by a terminal window putting me in 'Emergency Mode'. This time there was no useful command, nothing. Only the advice for me to check out the journal logs.

At first I thought it might have been a boot issue. After all, I had Windows 8 updated today and I have heard the horror stories with updates on Windows overriding the Ubuntu partition. So after booting my live CD and running [boot-repair](https://help.ubuntu.com/community/Boot-Repair)'s recommended options, I tried again. Still no luck. With me close to giving up (I had been checking the interwebs for the past hour), I decided to scroll to the end of the log (heres a tip: type a big number, then it scrolls to the end when running `journalctl`!) and io and behold: There was another fsck error message. Why it hadn't informed me like before, I do not know, but I ran fsck on that partition (twice for good measure), and then it booted.

This is of course all my own fault. Yesterday evening, I unplugged my system while it was running (great, yes im very smart /s) and as a result, it shut down in an incorrect state. So as a tip for next time: Don't do that. Unless of course you didn't do something like that, then you should look for new hardware and use this to backup your current data.

I have seen others with these error messages, and no real answer for it. I hope this at least helps others.
