---
id: 530
title: WordPress.com Stats problem solved.
date: 2009-05-14T12:19:54+00:00
author: mark
layout: post
tags:
  - statistics
  - stats
  - this blog
  - wordpress
---
My long-time <span style="text-decoration: line-through;">readers</span> reader may recall some grumbling about [the WordPress.com Stats widget not working properly](http://www.sallonoroff.co.uk/blog/2009/03/problems-with-wordpresscom-stats/) for me in Firefox3. Well, i&#8217;m happy to report that i appear to have solved the problem. And i&#8217;m also awfully embarrassed to tell you the solution.

Seeing that the widget has been updated recently i tried looking at the stats in Firefox again (i had been switching to other browsers if i wanted to see the stats) but was disappointed to see no change in behaviour. Given that a bigger issue has never been made of this problem i decided that it _must_ be an error on my part and undertook some more searching. It didn&#8217;t take too long to come across [this blog entry](http://foolswisdom.com/firefox-3-saved-cookies-still-too-tasty-by-default/) where something sounded very familiar in the [comments](http://foolswisdom.com/firefox-3-saved-cookies-still-too-tasty-by-default/#comments) section&#8230;

> _Is this what&#8217;s blocking WordPress.com Stats from working on my self-hosted blog via the Blog Stats tab in the Dashboard when I&#8217;m using Firefox 3.0b3 and Epiphany?_
> 
> _If I click the Blog Stats tab, I get a login dialog, even though I&#8217;m logged in to WordPress.com already._
> 
> _If I go to dashboard.wordpress.com and access my stats directly (without the iframe), it works fine._
> 
> _Actually, yeah, I can confirm that setting **network.cookie.cookieBehavior**_ _to 0_ _in **about:config**_ _fixes the Blog Stats tab._

I scrambled to load _about:config_ myself, gave this a try and lo&#8230; it worked. I could see my graph within Firefox3. O frabjous day! Callooh! Callay!

Of course, my joy turned to shame when i realised that _[network.cookie.cookieBehavior](http://kb.mozillazine.org/Network.cookie.cookieBehavior)_ is available in Firefox&#8217;s preferences for any idiot to see. It is simply the set of cookies checkboxes in Privacy options. I&#8217;d just had &#8220;Accept third-party cookies&#8221; turned off. What a fucking berk I am.

<img class="aligncenter size-full wp-image-531" title="ffcookiespref" src="/images/fromwp/2009/05/ffcookiespref.jpg" alt="ffcookiespref" width="452" height="110" srcset="/images/fromwp/2009/05/ffcookiespref.jpg 452w, /images/fromwp/2009/05/ffcookiespref-300x73.jpg 300w" sizes="(max-width: 452px) 100vw, 452px" />