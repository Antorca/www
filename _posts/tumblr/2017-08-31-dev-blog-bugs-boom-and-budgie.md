---
layout: post
title: 'Dev Blog: Bugs, Boom, and Budgie'
date: '2017-08-31T08:10:03+10:00'
tags:
- development
- update
- budgie
- bugs
tumblr_url: https://antorca.tumblr.com/post/164822175912/dev-blog-bugs-boom-and-budgie
---
### Bugs

To start things of, Antorca 5.0 beta 2 was released a week ago. Since its release I have discovered some bugs in the custom browser and productivity apps installer. This particular bug involved the installer checking if the app has been installed while the app is being installed.

This isn’t good at all - it’ll always end up saying that the app isn’t installed (unless it has already been installed before that particular scenario). This is because the installer script ends up jumping straight to that check right after initiating an install.

Thus I’ve decided to initiate a rewrite of the installer script in C to allow for process forking (which consequently allows for parent processes to wait for child processes to finish, voilà).

### Boom

> **UPDATE:** A new batch of updates have since resolved this! But now GIMP and BleachBit have been sacrificed because of updates to Python (I choose to go with bleeding-edge upstream updates instead of holding back updates to prevent potentially larger broken packages further down the road due to mismatched dependencies).

A recent update to the Debian Sid branch have caused folders in the file system root directory to be mounted as devices. This has caused an eye-sore on the desktop (where mounted drives are displayed by default), with dozens of directories appearing as devices there. As I write this blog post, I’m still trying to sort out what’s causing this bug. This may end up delaying Beta 3, and even worse - the eventual release of version 5.0.

### Budgie

With the massive stuff-up on the Xfce (i.e. default, or more realistically, the only actual) edition with the root directories, the cards are on the table again for the Budge edition. I’m considering the possibility that somewhere, somehow, a configuration fault in the Xfce edition is causing the root directory issue. So perhaps it’s worth a shot to see whether that issue could be reproducible on another desktop environment in another development virtual machine!