---
id: 1882
title: Using AppleScript to collect data from your inbox.
date: 2017-03-12T17:15:55+00:00
author: mark
layout: post
tags:
  - applescript
  - coding
  - data
  - email
  - geek
  - graphs
  - petrol
---
There are a host of ways of finding out where the cheapest fuel is for sale near you. I&#8217;ve been subscribed to [PetrolPrices.com](https://www.petrolprices.com/)&#8216;s notifications for years and years, and occasionally even look at the emails. On one such day, realising I had quite the history of local at-the-pump prices, I wondered if I could easily collate and chart this data. Being sat at a Mac, I turned to [AppleScript](https://developer.apple.com/library/content/documentation/AppleScript/Conceptual/AppleScriptLangGuide/introduction/ASLR_intro.html).

I&#8217;d never written any AppleScript before but I knew it must be fairly straightforward to do what I wanted. The basic script that I eventually cobbled together simply loops through all the emails in a set Apple Mail mailbox, taking the subject line and date stamp of each message, then dumps this info into a CSV file. [You can see my script here](/images/fromwp/2017/03/subjects-and-dates-in-mailbox.txt). (That&#8217;s a plain text version so should be viewable in-browser but you can also open or copy/paste in OS X&#8217;s Script Editor.)

The output from my script (the CSV file) is rather messy, containing as it does the whole subject lines, but for me this was easier to deal with afterwards than trying to work out how to run pattern-matching in the AppleScript to remove the chaff. I was also extremely fortunate that PetrolPrices included a fuel price in their email subject line, otherwise I would have _had_ to work out that pattern-matching stuff to search the email body text for the price (and probably given up).

Anyway, post-manual-processing of the output file, here&#8217;s the historical petrol price graph that I was able to produce with the gathered data:

[<img class="aligncenter size-full wp-image-2053" src="/images/fromwp/2017/03/sheffield-petrol-prices.png" alt="" width="900" height="560" srcset="/images/fromwp/2017/03/sheffield-petrol-prices.png 900w, /images/fromwp/2017/03/sheffield-petrol-prices-300x187.png 300w, /images/fromwp/2017/03/sheffield-petrol-prices-768x478.png 768w" sizes="(max-width: 900px) 100vw, 900px" />](/images/fromwp/2017/03/sheffield-petrol-prices.png)

For motorists, that line is a bit depressing. For me, it&#8217;s pleasingly similar [to this one](http://www.racfoundation.org/data/uk-pump-prices-over-time).

<span style="color: #999999;">&#8230;</span>

PS. For those wondering why a post published in March 2017 has a graph that only runs to April 2016&#8230; Well, that&#8217;s because PetrolPrices changed the format of their emails and my previous luck around inclusion of a price in the subject line ran out. Maybe I&#8217;ll work out the required regex/sed/grep/etc for version 2 of my script. (Holding your breath would be ill advised.)

<span style="color: #999999;">&#8230;</span>

PPS. Strictly speaking, the [PetrolPrices.com](https://www.petrolprices.com/) terms and conditions probably forbid me from doing any of this. Back in the real world, however, I don&#8217;t see why the company would have any cause for complaint with the above. If you work at PetrolPrices and disagree, please [get in touch](http://www.sallonoroff.co.uk/blog/about/).

&nbsp;