---
title: hello world (2).
date: 2018-03-23T23:39:00+00:00
layout: post
tags:
  - first post
  - this blog
  - wordpress
  - jekyll
  - github
---
You may have noticed that things started to look a little different around here a few days ago. It's not just (style)sheets that have been changed though - the whole backend of this thing is different. I've ditched the self-hosted [Wordpress](https://wordpress.org/) installation and moved everything over to [Jekyll](https://jekyllrb.com/), atop [GitHub Pages](https://pages.github.com/). I thought that warranted use of [another](/blog/2008/11/hello-world/) _Hello World_.

I'll spare you the boring details of how I shifted everything over to Jekyll - it's not a particularly unique undertaking[^fn-readme] - suffice to say, after one false-start, I based things on [Poole](http://getpoole.com/) and basic setup subsequently took no time at all. Of course, it took quite a bit longer to get the site looking and functioning how I wanted, and there are still quite a few things left to sort out[^fn-todolist].

The change is primarily a cost-saving exercise, since I really don't write that much here anymore, but also a time-saving one too hopefully. I won't have work on keeping Wordpress, and a variety of plugins and themes, up-to-date. Nor will have to worry too much about taking regularly backups. Furthermore, you - dear reader - should find the site to be a whole lot snappier, thanks to it all being simple HTML and CSS, served from GitHub's network. On the down side, there's no more commenting on posts (and i've lost all the old comments), i've currently no analytics to monitor visitor numbers[^fn-nostats], and [the blog's rss feed](http://www.sallonoroff.co.uk/blog/atom.xml) has had to change.

Anyway, I hope you like the changes overall. And if you spot anything that looks broken, it probably is, so please let me know.

[^fn-readme]: I've saved a list of guides and other people's blog posts that helped me to the repository's Readme file, if you're interested.

[^fn-todolist]: I'm not entirely happy with post layout, there are some broken video embeds, image-handling in imported posts needs tidying, there are **far** too many [tags](/blog/tags)...

[^fn-nostats]: Long-time readers will recall I was using Wordpress Stats, after [removing Google Analytics](/blog/2013/05/beginning-a-google-diet/).
