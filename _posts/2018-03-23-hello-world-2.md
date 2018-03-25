---
title: hello world. (2)
date: 2018-03-23T23:39:00+00:00
last_modified_at: 2018-03-24T11:02:00+00:00
layout: post
tags:
  - first post
  - this blog
  - wordpress
  - jekyll
  - github
---
You may have noticed that things started to look a little different around here a few days ago. It's not just the (style)sheets that have been changed though - the whole backend of this thing is different. I've ditched the self-hosted [Wordpress](https://wordpress.org/) installation and moved everything over to [Jekyll](https://jekyllrb.com/), atop [GitHub Pages](https://pages.github.com/). I thought that warranted use of [another](/blog/2008/11/hello-world/) _Hello World_.

I'll spare you the full details of how I shifted everything over to Jekyll &mdash; it's not a particularly unique undertaking[^fn-readme] &mdash; suffice to say, [this tool](https://ben.balter.com/wordpress-to-jekyll-exporter/) dealt with converting the 380 existing posts and, after one false-start trying to build it from scratch, [Poole](http://getpoole.com/) provided the basis of the new site. So the basic setup really took no time at all. Of course, it took quite a bit longer to get the site looking and functioning how I wanted, and there are still quite a few minor things left to sort out[^fn-todolist].

The change is primarily a cost-saving exercise, since I really don't write that much here anymore, but also a time-saving one too hopefully. I won't have to work on keeping Wordpress (and a variety of plugins and themes) up-to-date. Nor will I have to worry too much about taking regularly backups. Furthermore, you - dear reader - should find the site to be a whole lot snappier, thanks to it all being static HTML and CSS, served from GitHub's network. On the down side, there's no more commenting on posts (and i've lost all the old comments), i've currently no analytics to monitor visitor numbers[^fn-nostats], and [the blog's rss feed](http://www.sallonoroff.co.uk/blog/atom.xml) has had to change.

Anyway, I hope you like the changes overall. And if you spot anything that looks broken, it probably is, so please let me know.

[^fn-readme]: I've saved a list of guides and other people's blog posts that helped me to [the repository's Readme file](https://github.com/sallonoroff/sallonoroff.github.io/blob/master/README.md), if you're interested.

[^fn-todolist]: I'm not entirely happy with post layout, there are some broken video embeds, image-handling in imported posts needs tidying, lots of footnotes want neatening up, there are far too many [tags](/blog/tags)...

[^fn-nostats]: Long-time readers will recall I was using Wordpress Stats, after [removing Google Analytics](/blog/2013/05/beginning-a-google-diet/), but of course that's no longer possible. It's a little disappointing to find that GitHub Pages doesn't have some sort of basic statistics.
