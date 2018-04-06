---
id: 1878
title: Apple Airport firmware updates.
date: 2015-07-03 15:52:55 +00:00
author: mark
layout: post
tags:
  - airport
  - apple
  - firmware
  - hardware
  - software
  - hints
---
If you've owned and operated an Apple Airport device for any length of time you'll probably be aware that you can downgrade to older, previously-installed versions of firmware if you should ever need or want to. It's a fairly trivial thing to do with Mac OS X's Airport Utility &#8211; finding the feature is the hardest part![^fn-downgrading]

But what about if you want to try an older firmware on an Airport that has only ever run the current version? Well, that's a little bit less straight-forward&#8230; but not terribly difficult to do.

Firstly, take a peek at [http://apsu.apple.com/version.xml](http://apsu.apple.com/version.xml). I can't say for certain, but since it's sitting there on an Apple webserver I guess this is how your Airport checks to see if there are any updates available. Regardless, this XML file provides links to a number of firmware files (&#8220;.basebinary&#8221;) for each Airport model.

Unfortunately, _version.xml_ doesn't use the Airport model names you're familiar with. Instead it uses Product IDs that appear to have no relation to a device's model or order numbers. However, a mix of persistence and good fortune led me to discover that _/Contents/Resources/en.lproj/AirPortSettings.strings_ inside the Airport Utility app deciphers these IDs. Here they are:

**0 = AirPort Base Station**
  
**1 = AirPort Base Station**
  
**102 = AirPort Express 802.11g**
  
**104 = AirPort Extreme 802.11n (1st Generation)**
  
**105 = AirPort Extreme 802.11n (2nd Generation)**
  
**106 = AirPort Time Capsule 802.11n (1st Generation)**
  
**107 = AirPort Express 802.11n (1st Generation)**
  
**108 = AirPort Extreme 802.11n (3rd Generation)**
  
**109 = AirPort Time Capsule 802.11n (2nd Generation)**
  
**113 = AirPort Time Capsule 802.11n (3rd Generation)**
  
**114 = AirPort Extreme 802.11n (4th Generation)**
  
**115 = AirPort Express 802.11n (2nd Generation)**
  
**116 = AirPort Time Capsule 802.11n (4th Generation)**
  
**117 = AirPort Extreme 802.11n (5th Generation)**
  
**119 = AirPort Time Capsule 802.11ac**
  
**120 = AirPort Extreme 802.11ac**
  
**3 = AirPort Extreme 802.11g**

So now you know the ProductID for your Airport, you can go back to _version.xml_ and copy the correct URL of the firmware version you're interested in. Paste it into a web browser and you'll download the file. Then simply go back to Airport Utility, choose &#8220;other&#8230;&#8221; in that version drop-down menu and point Finder at your freshly downloaded .basebinary file.

Now cross your fingers that A) the downgrade works ok, and B) achieves what you were hoping for.

Oh, and remember, if having followed these instructions anything does go wrong with your base station, it is absolutely, categorically not my fault.

{% include mydots.html %}

**PS.** Huge thanks to Laszlo Pusztai whose [2013 blog post on downgrading an Airport Extreme](http://www.laszlopusztai.net/2013/02/11/downgrading-airport-extreme-to-7-6-1/) actually got us most of the way there.

[^fn-downgrading]: Marco Arment has covered it before &#8211; see [www.marco.org/2013/05/21/aebs-wifi-downgrade](http://www.marco.org/2013/05/21/aebs-wifi-downgrade) for details.
