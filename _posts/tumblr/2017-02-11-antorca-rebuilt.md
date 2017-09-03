---
layout: post
title: 'Antorca: Rebuilt'
date: '2017-02-11T01:24:29+11:00'
tags:
- announcement
- development
tumblr_url: https://antorca.tumblr.com/post/157091561132/antorca-rebuilt
---
**TL;DR** - Antorca shall now be based on Debian Sid; LXDE replaced by Xfce; VLC replaced by MPV.Since the recent ‘stuff up’ with the development virtual machine, I’ve taken more care as to how I backup and track changes made. This mostly involves more frequent VM snapshots.

However, in the last blog post I stated that there were now two development ‘branches’ - the old branch (codenamed ”Aberfeldy”, the one that’s publicly available at the moment), and the new branch (codenamed “Crimson”).

I’ve managed to pretty much replicate the Aberfeldy experience, but with Xfce replacing LXDE, MPV replacing VLC, and added a few additional tools. Crimson is also based on Debian Sid (the experimental branch of Debian) instead of Debian testing. This was necessary in order to get access to the latest Firefox packages instead of the extended support release.

Throughout Aberfeldy’s development I made use of two remastering tools - bootcd and Refracta. Refracta had extra compression options and its own installer, but it seriously messed with menu files and a few other settings. Bootcd was far more primitive and basic compared to Refracta but it did the job when it came to making a simple ISO image of the system without modifying menu files, etc. I decided to return to the remastering tool I used during the illume OS days - Remastersys, though I’m actually using a more recent fork of it called Respin. Respin doesn’t have a GUI installer like Remastersys, but the GUI installer I’ve been working could eventually be made compatible with the Respin installer!

Crimson is surprisingly stable despite being based on Debian Sid (which has been considered stable enough for daily use by a number of Debian users). Thus, I have come to the conclusion that ‘version 1’ shall use the Crimson base instead of the Aberfeldy base.