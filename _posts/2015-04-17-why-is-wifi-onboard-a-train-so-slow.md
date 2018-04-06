---
id: 1873
title: Why is wifi onboard a train so slow?
date: 2015-04-17 20:04:15 +00:00
author: mark
layout: post
tags:
  - public transport
  - wireless
  - mobiles
---
If you've ever tried to use wifi onboard a train in Britain you'll know it to be an exercise in futility and frustration. I'm sure i'm not the only one that has heard or read someone complain about the experience, or even thought to themselves &#8220;I might as well just use 3G&#8221;.

You don't have to massage the little grey cells for very long though to realise that 3G is all the train's wifi service can be using for internet connectivity too. The tin box speeding through the British countryside isn't plugged into an ethernet port back in Kings Cross, some spindle of cat5 cable viciously unwinding as it goes.

Icomera, a company you've almost certainly never heard of before, provides the wifi kit used by East Coast Trains. You can read all about their solution [here](http://www.icomera.com/solutions/east-coast-uk/), but this is the bit we're interested in:

> _East Coast trains carry up to 500 passengers at speeds up to 125mph (200kmph) through 400 miles of urban, suburban and rural areas. The Icomera Moovbox M800 was identified as the only solution that could deliver the level of service required in the challenging environments. By combining up to eight 3G/HSPA modems with a broadband satellite link and implementing Icomera’s patented seamless switching technology, East Coast passengers can enjoy high speed Internet access throughout their journey._

Right, so the trains use a mix of 3G and satellite broadband &#8211; how fast is that &#8220;high speed internet access&#8221;?

[Wikipedia has lots to tell us about 3G](https://en.wikipedia.org/wiki/3G). The most pertinent information I took from that article before falling asleep is that to meet _technical_ standards, 3G only need offer a peak speed of 0.2Mbps. Of course, many telecoms providers now offer speeds that far exceed that minimum standard but we're not talking more than 22Mbps in an absolute best case scenario (HSPA+). Personal experience certainly tells me that it's nowhere near that fast &#8211; I'm fairly sure the best speed test result i've ever had a 3G link was around 3Mbps. As for satellite broadband, [Wikipedia suggests](https://en.wikipedia.org/wiki/Satellite_Internet_access) that the average download speed is just 1Mbps. Meanwhile, [this article](http://www.networkworld.com/article/2457722/service-providers/a-new-breed-of-broadband-satellites-could-have-you-living-on-a-desert-island.html) about the launch of &#8220;upto 50Mbps&#8221; broadband satellites suggests that the typical speed existing systems in the US give is around 12-15Mbps.

Now it's time for some beer-mat mathematics. Let's be hugely generous and assume that Icomera's eight 3G modems each bring 22Mbps to the party and the satellite system a further 15Mbps. Further, let's ignore how all these modems actually work together (and all associated technical overheads involved) and just assume their connection speeds easily sum together to provide us a nice round maximum speed that is made available to the train's wifi users. I make that 191Mbps. Not bad, except it's potentially being shared by hundreds of passengers. If only 100 passengers share it, that's 1.9Mbps each. But you'll only see 0.38Mbps if the train is full to capacity and everyone is trying to use wifi. And remember this is taking place in A RAINBOW-LADEN PERFECT DREAM WORLD OF IDEAL NETWORK CONNECTIVITY. 0.38Mbps in paradise. Hmm.

Come back to damp and dirty reality where those 3G modems are getting a shitty signal as they whip along at 100mph, all the various bits of networking kit involved have overheads, some part of the system is faulty, and there's contention over those paltry 3G signals with all the mobile-phone-toting passengers who aren't trying to use the train wifi (not to mention all those not on the train but connected to the same mast), and you'll hopefully realise why you're sat there complaining about the speed of the wireless connection.

Hopefully [4G](https://en.wikipedia.org/wiki/4G) will improve matters somewhat&#8230; but then again, there are more people, with more devices, looking to use such services. So maybe in future i'll try to remember to pack a book.

{% include mydots.html %}

**PS.** Most of the above also applies to the wifi we're increasingly being offered aboard buses too. But i'm sure you'd already worked that out.
