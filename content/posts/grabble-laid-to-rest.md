---
title: Grabble laid to rest
date: '2009-04-20T11:00:23.000+02:00'
lastmod: '2009-04-15T22:51:32.000+02:00'
slug: grabble-laid-to-rest
tags:
  - General
  - Grabble
  - Open Source
  - Projects
  - Search
  - Technology
---

![Grabble](/content/images/2009/04/grabble-small.jpg)In 2006 I was fascinated with search. So much so that I learnt all that I could about search engines and SEO and this was largely driven by the fact that I was in complete awe of Google at the time. All of this inspired me to start a South African search engine and during 2006 I launched [Grabble](http://www.grabble.co.za/?ref=justhart.com).

![Old Grabble](/content/images/2009/04/picture-50-500x295.png "Old Grabble")

Because I only understood the theory of search engine technology it wasn’t as easy as I had thought to start my own and implementing the technology was an extremely complicated experience. My very first version was powered by [Lucene](http://lucene.apache.org/?ref=justhart.com) but as it was powered by Java (and TomCat) I had great difficulty in getting it to work as expected.

I then ran a version of [mnoGoSearch](http://www.mnogosearch.org/?ref=justhart.com) which was run as a Perl command line utility and while this one seemed to give me the best results I had resource issues which hampered my efforts. What I soon figured out was why Google has a few hundred thousand servers powering their search engine and after about a week of indexing South African websites I ran out of disk space. With about 8 million records indexed I had used up my 80GB hard drive.

So, in the end Grabble went PHP and while I retained some indexing capabilities from mnoGoSearch I also tapped into Yahoo to help out. At the time Yahoo didn’t have a search API so I had to do a lot of hacking to get results returned from Yahoo. In particular, Yahoo provided all the image, news, videos, blogs, sport and forum search results.

While being in awe of Google I also felt that total dominance of only a few players in the market wasn’t a good thing. I believed, esoterically at the time, that local search needed to be dominated by a local company. These beliefs I still hold true to heart and I feel that it’s critical that competitors exist. There is something very uncomfortable in knowing that one or two companies hold the majority of the world’s data and I was convinced that Grabble would be a _winner_.

Almost three years later and I’ve been debating what to do with Grabble. For the last two months the site hasn’t even been operational (well web search anyway) and while I didn’t want to close it down completely I also had to face the reality that Grabble was never going to dominate and I simply did not have the time to maintain it any longer.

Then along came [4hoursearch](http://www.4hoursearch.com/?ref=justhart.com) – a website powered by the [Yahoo BOSS](http://developer.yahoo.com/search/boss/?ref=justhart.com) search API and running off [Google AppEngine](http://appengine.google.com/?ref=justhart.com). I stumbled across this site by chance and realised that they had released their source code under GPL. Subsequent to this finding I have now moved Grabble onto this Python software and my **final** version of Grabble has now been hatched.

[![Final version of Grabble](/content/images/2009/04/picture-52-500x221.png "picture-52")](http://www.grabble.co.za/?ref=justhart.com)

What this final version does is allow me to keep the site up for those who still want to use it and at the same time it gives me an opportunity to say goodbye. Running through the Yahoo BOSS API means that I don’t have to worry about indexes any longer and living on the Google AppEngine means technology is now taken care of.

I have learnt so much about search through my efforts with Grabble and I hold it very close to my heart. While it never took off it did give me an opportunity to expand my knowledge and experience in an area I felt passionate about and the learning curve I’ve gone through has certainly helped define where I am today.
