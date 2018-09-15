---
layout: post
title: Antorca “Aberfeldy” build 20170123_1250
date: '2017-01-23T01:40:05+11:00'
tags:
- announcement
- beta
tumblr_url: https://antorca.tumblr.com/post/156254049912/antorca-aberfeldy-build-201701231250
---
A new build of Antorca has been uploaded to the project’s SourceForge project site! I have decided to make some builds public before completing a fully working version of the installer as to iron out other features beforehand. This build, like the previous (but unannounced build) includes a temporary installer (the terminal version of the Refracta installer).

### Download

You can get the 1.86GB ISO image of build 20170123_1250 at SourceForge. One thing that hasn’t been tested yet is if the ISO image can be flashed on to the USB drive. If it succeeds, please contact me via email to notify me of it - this would be greatly appreciated.

#### Login information and installation

One important thing I forgot to mention before releasing the previous build was the login details and how to access Antorca’s installer. The default user on the live image is root, with the password antorca. The installer can be accessed by clicking on the applications menu > System Tools > Install Antorca.

#### Changes and new features

##### New Apps

- Added Kazam screen-casting tool (heavier than RecordMyDesktop, but better performance + better audio-video syncing).
- Added Gdebi so packages can be installed using an interactive GTK dialog rather than using the “dpkg -i [package_name]” command (this will help encourage users who have to download .DEBs of their favourite apps that aren’t in repositories).
- Firefox
  - Added Pepper Flash plugin for Firefox.
  - Disabled automatic HTML5 video playback, and set Pepper Flash permissions to ‘Ask to Activate’ instead of ''Always Activate’.

##### Artwork

- New wallpaper by Yassine Wannessi included (check Desktop Preferences > Wallpaper > Antorca Texture 1 or Antorca Texture 2). Thanks Yassine!

### Reconsidering the version numbering scheme

I have found trying to predict exactly what the ‘version number’ for a release would be due to other commitments which make it difficult for me to work continuously on Antorca and to stick to a schedule! Thus I have started to consider falling back to the standard ‘1.0, 2.0, 3.0, etc’ incremental version numbering scheme compared to the date-based scheme.If I go ahead with this, I may consider avoiding doing minor releases (e.g. 1.1, 1.2, 2.1, 3.5, etc) and just increment the version number regardless of how big of an update the new release is.