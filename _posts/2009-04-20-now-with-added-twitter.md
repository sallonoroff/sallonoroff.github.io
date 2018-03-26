---
id: 445
title: Now with added twitter feed.
date: 2009-04-20T13:59:25+00:00
author: mark
layout: post
tags:
  - this blog
  - twitter
  - wordpress
  - coding
---
As you should have already spotted, the blog now features my latest twitter updates (&#8220;tweets&#8221;) in the sidebar. It wasn't difficult to get the feed in place (i just installed the [Twitter Widget](http://wordpress.org/extend/plugins/twitter-widget/)) but i've had a bit of a headache getting it looking right. The CSS of the [Simplex theme](http://wordpress.org/extend/themes/simplex) i currently use for the blog was doing some nasty stuff with tweets that contained URLs, be they actual links or just usernames in the twitter @username convention. In hacking the theme's CSS (_/simplex/style.css_) to try and overcome this things ended up looking mighty squashed up. I thought i'd resolve it with some padding or margins but i ran into problems with my new CSS being ignored by the browser in favour of existing code. Fortunately a very kind soul told me about &#8220;_! important_&#8221; which forces use of the CSS line you want to use and all was sorted. Sure it's probably not the best solution but this thing already employs a few cheap hacks anyway.

For those of you that are interested, here's the code (based on some i found [here](http://www.designisphilosophy.com/css/create-a-twitter-box-in-your-sidebar-20081106/) btw) that i tagged onto the end of the _style.css_ file to sort things out&#8230;

<code>
#twitter_div {
  padding-top: 10px;
}

#twitter_div span {
  color: #000000;
}

#twitter_div ul li {
  border-bottom-style: solid;
  border-bottom-width: 1px;
  border-bottom-color: #EEEEEE;
  padding: 10px 0 10px 5px ! important;
}

#twitter_div ul li a {
  text-decoration: none;
  background: none;
  padding: 0;
  display: inline;
}

#twitter_div ul li a:hover {
  text-decoration: none;
  background: none;
  background-color:#E8C8C8;
  padding: 0;
  display: inline;
}
</code>
