---
layout: post
title: Live image boot issue
date: '2017-01-23T22:40:37+11:00'
tags:
- bug
- fix
tumblr_url: https://antorca.tumblr.com/post/156293586207/live-image-boot-issue
---
There appears to be an issue with the live image when attempting to boot from it - the boot sequence ends up trying to boot up the operating system that’s already on the hard disk.The solution to this problem is to type “sr0″ in the command line interface that appears when first booting up the live image (i.e. when the “boot:” menu appears).Please contact me if this problem persists or if this solution is proven to work.
