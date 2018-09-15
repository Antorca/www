---
layout: post
title: Antorca “Aberfeldy” build 20170127_1150
date: '2017-01-27T12:24:04+11:00'
tags:
- announcement
- beta
tumblr_url: https://antorca.tumblr.com/post/156449017717/antorca-aberfeldy-build-201701271150
---
Yet another new build of Antorca has been uploaded to the project’s SourceForge project site! This build may still have issues with booting from the live ISO image. The build’s SourceForge folder has a read me file which describes how to work around the issue.

### Download

You can get the 1.91GB ISO image of build 20170127_1150 at SourceForge.

#### Login information and installation

The default user on the live image is root, with the password antorca. The installer can be accessed by clicking on the applications menu > System Tools > Install Antorca.

##### What’s new

- Added GNOME Software for friendlier app management.
- Added support for Flatpak.
- Added Xpad for quick note taking.

##### Changed

- Re-enabled media autoplay in Firefox (for HTML5 content only).
- Multitouch trackpad support via xserver-xorg-input-mtrack driver.
- Replaced default wallpapers and font in About dialog.

##### Fixed

- None (live boot issue still being fixed).

##### Things to test

- Flatpak packages could be installed and updated.
- Trackpad works as it should on a non-multitouch trackpad.
- Trackpad works (with gestures like two-finger scrolling) on a multitouch trackpad.
- Flash content works and HTML5 video autoplays.