---
id: 1902
title: Download YouTube videos without dodgy software.
date: 2015-11-16 14:07:06 +00:00
author: mark
layout: post
tags:
  - hints
  - videos
  - web
  - youtube
  - software
  - malware
---
You've found a video on Youtube that you'd like to download to watch later offline. Or maybe you want to save a copy of a YouTube video for posterity. Or perhaps you uploaded a clip to YouTube and no longer have the original but want one. So, how do you do that? Well, there are hundreds of free programs, websites and browser toolbars, add-ons, add-ins and extensions that purport to help you do this. The problem with the majority of these is that they're plain useless if you're lucky and serve-up [malware](https://en.wikipedia.org/wiki/Malware) if you're not.

Fortunately, there's a fairly simple way to do it using just your web browser of choice and the free, open-source, cross-platform and generally awesome [VLC media player](http://www.videolan.org/vlc/):

  * Copy the URL of the YouTube video you're wanting to save
  * Start VLC and go to &#8220;Open Network&#8230;&#8221;
  * Paste in the youtube link, then click Open
  * The video will start playing. Pause it and go to the media information window
  * The &#8220;Location&#8221; field should contain a (long, complicated-looking) URL &#8211; this is a link to the actual video file &#8211; copy it
  * Now go back to your browser, paste that URL into the address bar and hit enter
  * You have video! (depending on browser used the file will either ask to be saved or start playing automatically, in which case you can just do File > Save As)

I'm not sure what the container and video format are of these saved files are yet but they play happily enough in VLC. It would be nice to know though &#8211; please let me know if you work it out!

The other limitation of this method that you should be aware of is that there's no way choosing video quality &#8211; again, shout up if you know how to get at one of the particular qualities that YouTube has stored.

If the above looks too convoluted for you, then you might try [youtubeinmp4.com](http://youtubeinmp4.com/), which, despite being covered in ads and looking a bit dodgy, does appear to do something extremely similar but makes the process as simple as pasting in the YouTube link. I've grabbed a few videos using the site and, as far as I can tell, not caught anything nasty. Your mileage may vary, of course. Obviously you should take precautions before visiting the site, just in case.

{% include mydots.html %}

**Update:** Alternatively, [saveitoffline.com](http://www.saveitoffline.com) looks like an even better website to try if you don't fancy the VLC option. Just paste in the vid URL and you're presented with links to all the various formats and qualities that YouTube has available for that clip. I'm not sure you could want for more.
