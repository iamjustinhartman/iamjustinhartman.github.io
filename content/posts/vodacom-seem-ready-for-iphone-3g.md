---
title: Vodacom seem ready for iPhone 3G
date: '2008-07-21T15:37:00.000+02:00'
lastmod: '2008-07-31T02:03:10.000+02:00'
slug: vodacom-seem-ready-for-iphone-3g
tags:
  - Apple
  - General
  - Hacking
  - iPhone
  - Vodacom
---

After [upgrading my iPhone firmware](/2008/07/21/first-iphone-20-firmware-hack-in-south-africa/) it’s clear to me now that Vodacom’s iPhone network is alive and kicking.

I upgraded Colin’s iPhone on a Cell C network and none of the localisation functions had kicked in like it did on my Vodacom phone. The real bitch in all of this is that EDGE/GPRS doesn’t work on my iPhone while it does on Colin’s.

The new version 2.0 firmware no longer has a menu to set you APN key like on previous versions so I decided to see if I could manually change this in one of the preferences files on my iPhone. Look at what I discovered in the XML file:

![](/content/images/2008/07/iphone-apn.jpg)

The APN key has now been set by the network as _iphone.vodacom.za_ and nothing I do can change this setting as it simply overwrites the string each time.

The result of this is that each time I try connect I get an error message saying _“Could not activate cellular data network: You are not subscribed to a cellular data service”_.

Seeing as Colin’s Cell C iPhone connects to EDGE without any problems I have to believe that Vodacom are going to enforce a data package subscription when the iPhone is officially launched in SA. I also bought a data bundle from Vodacom to see if this would work but I still get that pesky message.

The fact that my iPhone is completely localised, as opposed to Cell C’s network, is interesting to say the least. It’s a little scary though because as a Vodacom subscriber I can see I’m going to have problems with an unofficial iPhone down the line.
