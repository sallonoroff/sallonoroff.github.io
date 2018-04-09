---
id: 1972
title: Make a bootable USB drive with createinstallmedia.
date: 2015-11-23 14:24:13 +00:00
author: mark
layout: post
tags:
  - apple
  - hints
  - installer
  - utilities
  - mac
  - osx
  - usb
---
If you're a Mac user, it can't have escaped your attention that all updates to OS X come via the Mac App Store nowadays. Most of the time this is great &#8211; a welcome advance in the software world &#8211; but sometimes, like when you need to re-install the whole OS, a 5GB download isn't particularly convenient. Especially if you've a flakey internet connection. Or if your only means of downloading the file is the computer in front of you that needs said OS installation.

So the answer? Bootable USB installers for OS X. Download that 5GB file once, then use any old USB stick[^fn-yourusb] with Apple's _createinstallmedia_ utility to create a bootable drive you can use again and again. And again. [Apple even provides the instructions on how to do this](https://support.apple.com/en-us/HT201372). Lovely stuff.

If you want a bit more hand-holding through the process then I heartily recommend [Dan Frakes](http://danfrakes.com)' how-to guides over at Macworld. These are particularly useful if you need to make a drive for installing OS X Lion (10.7) or Mountain Lion (10.8), since the createinstallmedia tool didn't exist back then and the process is a little different (but no more difficult). Here are the necessary links:

[Mac OS X 10.7 Lion](http://www.macworld.com/article/1161069/software-system/make-a-bootable-lion-installer.html)
  
[Mac OS X 10.8 Mountain Lion](http://www.macworld.com/article/1167857/software-system/how-to-make-a-bootable-mountain-lion-install-drive.html)
  
[Mac OS X 10.9 Mavericks](http://www.macworld.com/article/2056561/how-to-make-a-bootable-mavericks-install-drive.html)
  
[Mac OS X 10.10 Yosemite](http://www.macworld.com/article/2367748/os-x/how-to-make-a-bootable-os-x-10-10-yosemite-install-drive.html)
  
[Mac OS X 10.11 El Capitan](http://www.macworld.com/article/2981585/operating-systems/how-to-make-a-bootable-os-x-10-11-el-capitan-installer-drive.html)

And if you're hoping to make a bootable USB installer for Snow Leopard (Mac OS X 10.6) then there is, sort of, a way to do it. You'll need an image of the Snow Leopard install DVD first though, of course. [Take a look at this Macworld article for instructions](http://www.macworld.com/article/2023548/dvd-less-snow-leopard-installation-on-older-mac.html).

[^fn-yourusb]: Your USB stick needs to have space to fit the OS X installer &#8211; so at least 8GB. And make sure you've nothing precious saved on it, because it will get blanked during this procedure. You might also want to find one that has decent read/write speeds, since this will reduce the amount of time it takes to create a bootable installer and to install OS X onto to your Mac.
