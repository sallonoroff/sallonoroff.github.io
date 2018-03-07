---
id: 325
title: Problems with WordPress.com Stats.
date: 2009-03-11T14:44:03+00:00
author: mark
layout: post
tags:
  - skeltoac
  - statistics
  - stats
  - this blog
  - wordpress
---
After seeing how simple it was to install the spam-blocking [Akismet plugin](http://wordpress.org/extend/plugins/akismet/) (which is working very well thanks &#8211; about 100 spam comments blocked in 5 days) on here, i thought i&#8217;d give the [WordPress.com Stats plugin](http://wordpress.org/extend/plugins/stats/) a try too since it appeared to offer an equally painless setup. Which it was. It couldn&#8217;t really get any simpler. Sadly, my positive first impressions were marred by the fact it didn&#8217;t appear to be working properly.

The plugin adds a widget to your WordPress dashboard and a new &#8220;Blog Stats&#8221; page accessible from the Dashboard menu. I could see from the widget that statistics were being collected&#8230;

<img class="aligncenter size-full wp-image-326" title="wp_stats_on_dashboard" src="/images/fromwp/2009/03/wp_stats_on_dashboard.jpg" alt="wp_stats_on_dashboard" width="429" height="400" srcset="/images/fromwp/2009/03/wp_stats_on_dashboard.jpg 429w, /images/fromwp/2009/03/wp_stats_on_dashboard-300x279.jpg 300w" sizes="(max-width: 429px) 100vw, 429px" />

&#8230;but when everytime i attempted to complete the WordPress.com login (Stats are linked to the WordPress.com account with the API Key you used during installation of the plugin) it just brought back the login screen. No errors. No feedback of any sort. Just a refresh of the login prompt. Ad nauseum. The same thing happened on the Blog Stats page too. I wondered if it was just a problem with Firefox, so i launched Chrome and tried that&#8230; to no avail. I had a google or two about the problem and found several other instances of people suffering with the same issue but no-one able to give a solution. So i cut out the middlemen and emailed the plugin&#8217;s author, [Andy Skelton (skeltoac)](http://skeltoac.com/) of [Automattic](http://automattic.com/), to see if he could offer any pearls of wisdom. Here&#8217;s what he had to say:

> _&#8220;Thanks for the report. I have never seen this problem in real life, though I&#8217;ve heard of it. The technology we use to embed the WordPress.com login is standard web stuff. We don&#8217;t have anything out of the ordinary there. I can only assume your browser is doing something strange, such as following a security setting that prevents cookies from being set by the embedded site._
> 
> _This is one of those unhappy responses about me being unable to do anything about it. I&#8217;d really have to have your computer in front of me. So the best I can say is this: mess around with your browser settings, try different browsers, and if you learn anything please post the results where others will benefit. I wish I could have done more.&#8221;_

Not the response i&#8217;d really been hoping for but it was good to receive a reasonably prompt, personal reply to what was essentially a whingey support request. Anyway, buoyed by the news that there was nothing complicated going on, i took Andy&#8217;s suggestion of trying some other browsers. Firefox and Chrome on the PC had failed but i still had Firefox, Safari, Camino and Opera to try on the Mac. Unsurprisingly, Firefox failed just as it had on the PC but with Safari and Camino it worked. Once i&#8217;d completed the WordPress.com login i could see the lovely visitor numbers graph on the dashboard widget and all the detailed statistics in the Blog Stats page. And then when i tried Opera i got a clue to where the problem may lie&#8230;

<img class="aligncenter size-full wp-image-328" title="wp_cert_warning" src="/images/fromwp/2009/03/wp_cert_warning.jpg" alt="wp_cert_warning" width="506" height="385" srcset="/images/fromwp/2009/03/wp_cert_warning.jpg 506w, /images/fromwp/2009/03/wp_cert_warning-300x228.jpg 300w" sizes="(max-width: 506px) 100vw, 506px" />

Approving use of this certificate allowed Opera to get into the Stats too. So is it something about Firefox&#8217;s default security settings that mean we can&#8217;t get around this &#8220;faulty&#8221; certificate? I assume so but to be honest, i&#8217;m not sure. I&#8217;ve not yet found any setting in Firefox that gets me around this though (of course) that&#8217;s not to say it isn&#8217;t possible. Meanwhile, Andy Skelton has passed on my &#8220;findings&#8221; to WordPress&#8217; Systems people to investigate.

So, until WordPress sort something or i find a workaround for Firefox, i&#8217;m stuck switching to another browser whenever i want to see the detailed Stats. Shame.