---
id: 554
title: Two point eight.
date: 2009-06-11 14:33:37 +00:00
author: mark
layout: post
tags:
  - this blog
  - wordpress
---
I've just upgraded this thing to WordPress 2.8 using the automatic-built-in-updater-thingy.

It appears to have worked OK but you never know, i might find something amiss soon. If you spot anything looking decidely wrong or behaving pear-shapedly please do let me know (via a comment/email/smoke signal/etc). Thanks.

{% include mydots.html %}

**Update:** Aw, shit. The &#8220;Tag Cloud&#8221; widget (the bit you see as &#8220;Common Tags&#8230;&#8221; on the right) is no longer cloud-like. It's just a list. Ug-er-lee.

{% include mydots.html %}

**Update #2:** Ah-ha. Sorted the Tag Cloud problem. Turns out that the cloud was known as _#Tag_Cloud_ but in WordPress 2.8 has become _#Tag_Cloud-2_ (why?!). So to fix, i've had to alter all references appropriately in the CSS files (_/simplex/style.css_ and _/simplex/css/default.css_). Lovely.
