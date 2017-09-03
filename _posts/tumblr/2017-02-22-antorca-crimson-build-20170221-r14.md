---
layout: post
title: Antorca “Crimson” build 20170221-r14
date: '2017-02-22T00:49:09+11:00'
tags: []
tumblr_url: https://antorca.tumblr.com/post/157558796537/antorca-crimson-build-20170221-r14
---
The first public build of the new Crimson development branch is out now! It’s a completely re-built distribution based on Debian Sid (the experimental branch of Debian). Despite using the latest packages, it is mostly stable enough for daily use (use it for development at your own risk!).

### Download

The build’s ISO image weighs in at 1.4GB (that’s 500MB lighter than the last Aberfeldy build!). It’s available at the build’s folder in the project’s SourceForge page.

Install at your own risk! To install the image on to a hard disk, navigate through the start menu by going into the System category and selecting System Installer. When partitioning your disk for installation, set aside at least 256MB for an extended partition containing a linux-swap partition, whilst the main partition (which holds the system files and home folder) should be formatted as ext4 and could take up however much space you need it to.

> **Username:**	root
>
> **Password:**	antorca

### What’s new

#### Added

- Geary email client with modern GNOME-based interface and conversation-layout for email threads.


- Geany integrated development environment complete with all plugins offered on the Debian repositories.


- MPV media player added alongside VLC media player.

#### Changed

- Based on Debian Sid instead of Debian Testing (Stretch).


- Default desktop environment is now Xfce instead of LXDE.


- Removed GNOME Software.


- Changed default desktop font to DejaVu Sans for readability on a wider range of monitors and display modes.


- Generic application names in the menu is now default.

#### Fixed

- Live boot issue by temporarily using Respin for ISO remastering instead of Refracta Snapshot.