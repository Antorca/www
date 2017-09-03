---
layout: post
title: Starting again? Maybe?
date: '2017-02-08T21:25:26+11:00'
tags:
- development
- issue
tumblr_url: https://antorca.tumblr.com/post/157000338952/starting-again-maybe
---
Silly, silly me! I didn’t quite make enough snapshots of my development virtual machine in between making a great amount of changes on the upcoming preview release of Antorca. Well, actually what happened was I conducted an apt upgrade which seemed to have broken the system (i.e. black screen after trying to boot up). I ended up wiping the development virtual machine and installed the last build of Antorca from an ISO image.

Thinking that all was fine after re-installing, I deleted most of the older snapshots. Upon attempting to create a live ISO image after making the necessary changes, error upon error appeared. Mind you, this doesn’t mean whatever I’ve worked on as of late has horrifically disappeared. In fact, everything is still surprisingly intact. It’s just that I can’t make ISO images for now.

I contemplated how situations like these could be a nightmare in the future if a monumental screw up like this were to happen again. The Debian base system virtual machine which Antorca is based off doesn’t include many of the core features I eventually added to Antorca. Luckily these don’t require a desktop environment (e.g. third party repositories, Flatpak, etc), so I’ve cloned the original base system, did some updates, and added the necessary new core features.

Now what? I’m currently deciding whether to continue working off of the “Aberfeldy” branch of development (the one where the ability to make ISO images have been partially hampered) or the new “fresh start” branch (slightly less risky, I may also have a chance to reduce the bloat-creep).