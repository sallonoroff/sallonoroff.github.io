---
id: 1701
title: Fullscreen Firefox in Mountain Lion.
date: 2012-08-14 12:07:02 +00:00
author: mark
layout: post
tags:
  - browser
  - firefox
  - osx
  - software
  - hints
---
I started using OS X Mountain Lion in earnest yesterday (so you can expect a post detailing my thoughts on this new version of the OS sometime in the next few weeks/months/years) and almost immediately ran into a big annoyance with Mozilla Firefox.

In Mountain Lion, Firefox treats fullscreen mode like, well, like fullscreen mode on the PC. That is to say, it thinks you want to run a kiosk and auto-hides all the chrome. That's fine, except that when you do move the pointer to the top of the screen to get to the address bar or search bar or any other toolbar, the OS X menu bar for Firefox and Firefox's own toolbars appear simultaneously. And they overlap. And it's all rather frustratingly useless. Naturally, i assumed that i'd be able to alter Firefox's behaviour in Preferences but apparently not. You have to use the config editor.

To access the config editor you need to type _about:config_ into the address bar and hit enter.

Now click the twee _I'll be careful, I promise!_ button and you're in.

You want to locate the _browser.fullscreen.autohide_ preference in the huge list (the search box should help with this).

Change the value of _browser.fullscreen.autohide_ to _false_.

And that's it. Now you should have Firefox working more like Safari and Google Chrome do &#8211; ie. how you'd expect.

{% include mydots.html %}

**PS.** I haven't yet worked out how to force the bookmarks toolbar to stay visible in fullscreen Firefox. My bookmarks are there when Firefox is windowed but the moment you make it Fullscreen the bar vanishes. If anyone has spotted the relevant preference in the config editor, please do shout up.
