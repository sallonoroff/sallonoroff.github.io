---
id: 78
title: Uncategorized.
date: 2009-01-22T15:09:31+00:00
author: mark
layout: post
tags:
  - this blog
  - wordpress
---
I decided that i prefer to use Tags in this blog rather than Categories&#8230; so i converted all the existing Categories to Tags and went to disable Categories. Only i can't find anywhere in the WordPress settings to turn off all reference to them and thus all my posts were left reading &#8220;Posted in Uncategorized &#8230;&#8221; under the title. Messy.

Fortunately WordPress&#8217; inbuilt editor means you can simply edit out bits you don&#8217;t want, so i was able to just delete (well, comment-out) all references to &#8220;the_category&#8221; i found in the Simplex theme. If you want to so the same you&#8217;ll need to fiddle with _index.php_, _single.php_, _archive.php_ and _search.php_.
