---
title: Two guides on how to mirror two specific sites.
layout: post
categories: guides
tags: mspfanventures, lparchive, mirroring
image: http://ev1l0rd.github.io/images/AM2R_promo_art.jpg
---

Here are two scripts for mirroring two sites. I chose http://lparchive.org and http://mspfanventures.com . Both scripts also have a flag for updating (`-u`). As per usual, these scripts are Linux/Bash shell only.

Both scripts are designed to only download a single instance of their respective archiving tools. (So one LP or one fanventure per script.)

Two additional notes for the mspfanventures script:

- The story ID is what is located after the `s=` part in the URL. It is always a number and it goes up to the `p=` part.
- To get the latest page number, go to the latest page and copy the numbers after the `p=` part.

<script src="https://gist.github.com/ev1l0rd/f3fc43f8df67c151ca2cc17b24e8a117.js"></script>

-> Ev1l0rd.
