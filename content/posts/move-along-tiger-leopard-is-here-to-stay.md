---
title: Move along Tiger - Leopard is here to stay
date: '2007-10-31T11:05:26.000+02:00'
lastmod: '2007-10-31T11:05:35.000+02:00'
slug: move-along-tiger-leopard-is-here-to-stay
tags:
  - Apple
---

On Friday, in true Geek style, I trekked half way across Johannesburg through rain, fog and heavy traffic to the [iStore](http://www.apple.co.za/istore/?ref=justhart.com) in Clearwater for the much anticipated [Mac OS X Leopard](http://www.apple.com/macosx/?ref=justhart.com) launch.

It didn’t disappoint and after meeting some cool Apple people I purchased my copy of Leopard and raced home as quickly as possible so as to install this marvel of an operating system. Now most of you who didn’t do the Geek thing and haven’t yet upgraded from Tiger to Leopard will have read tons of rave reviews about the new OS and rightly so. I figured though that I’d take a look at some of the pitfalls of Leopard and what to look out for when upgrading.

**[Time Machine](http://www.apple.com/macosx/features/timemachine.html?ref=justhart.com)**

This is by far Apple’s flag-ship of the new OS and they’ve punted this new backup solution as the best new feature yet. I am unfortunately not overly impressed.

Time Machine is really the first humanised backup solution to find its way to a personal computer and while the interface and simplicity is just awesome I’m still not convinced about it.

The fundamental flaw in Time Machine is the disk space required to run backups efficiently. What surprised me is that Apple have decided not to compress backed up data using Time Machine so this effectively means that if you’re using 60GB of your hard drive you need at least 60GB on a backup drive to cover the first backup that Time Machine creates.

What happens to each subsequent backup thereafter is a form of incremental backups. Time Machine backs up data every hour (assuming your external drive is plugged in) so any change to a file, application or preference will be written to the backup drive as **new** files. Now this creates a major problem as I’ve got a 120GB drive in my MacBook Pro and I’ve worked out (very roughly) that if I want to keep 6 months worth of backup data I’d need at least a 750GB backup drive to come close to this time line.

If your current backup drive gets full Time Machine starts deleting the oldest backup information from your drive and seeing as I currently only have a 80GB backup drive I can realistically only keep 1 weeks worth of backups on the drive at any given time.

I’m sure this feature is going to evolve as the OS matures but right now this non-compression and the lack of preferences for Time Machine, i.e. ability to change backup frequency, ability to backup online or via iPod, overwriting versus new file backup, make it a solution that falls a little short in my opinion.

Besides which, what am I supposed to do with a 750GB, bulky, external hard drive anyway? I have a MacBook Pro for mobility and now I’m forced to carry a heavy piece of lead around with me just so I can backup…

**[Spaces](http://www.apple.com/macosx/features/spaces.html?ref=justhart.com)**

Now this is a feature that I’ve _really_ been looking forward to in Leopard and for the most part it delivers beyond my expectations. One of the best features of Spaces is that you can pre-define which space to open an application in when you launch it from your Dock or the Applications folder. So, like the very organised individual that I am, I setup my Spaces as follows:

-   Space 1 = Productivity apps (Word, Excel, etc.)
-   Space 2 = Internet apps
-   Space 3 = Development apps
-   Space 4 = Graphics apps and other stuff I don’t know where to put

The amazing part is that as soon as I open Safari (for example) I’m redirected to Space 2 and when I open Word I’m redirected to Space 1. Simple, beautiful and efficient – my desktops are now organised.

Sadly in the last 24 hours this has all stopped working. For some unknown reason opening up apps no longer appear in the pre-defined Space that I’ve configured but rather in the current Space I’m working in and I just can’t understand what went wrong.

**Software Compatibility**

I’ve hacked my Mac by installing my own versions of [Apache2](http://apache.org/?ref=justhart.com), [MySQL5](http://mysql.com/?ref=justhart.com) and [PHP5](http://php.net/?ref=justhart.com) so I was very worried about what an upgrade would do to this. I asked PJ at the launch what would happen and he told me that Leopard would delete it all. Despite this I decided it was still worth upgrading so I did it anyway and the great news is that after the upgrade all of my Linux hacks (including [subversion](http://subversion.tigris.org/?ref=justhart.com)) were still in tact and were left untouched by the upgrade. That said, YMMV!

So far so good and after the upgrade all appeared to be fine with the software installed on my machine but there were two issues. The first was an app I use called [CSSEdit](http://macrabbit.com/cssedit/?ref=justhart.com) which just kept crashing however the developers of this app already had a 10.5 patch which I downloaded and installed and it has been perfect ever since. The second was an Apple Mail task bar plugin that notifies you of new mail as it arrives but this just had to be deleted and I haven’t bothered to try to find a new one.

In true Microsoft style I’ve now discovered some issues with Word and Excel. While I can use these two applications they do tend to crash a lot and typically Microsoft have not yet released any patch to combat this issue in Leopard.

[Gregor](http://groogle.co.za/?ref=justhart.com) has reported that [Cyberduck](http://cyberduck.ch/?ref=justhart.com) is broken (I use [Transmit](http://www.panic.com/transmit/?ref=justhart.com)) but his entire [Adobe CS2 suite](http://www.adobe.com/products/creativesuite/?ref=justhart.com) of software appear to work perfectly under the new OS.

Overall I’m exceptionally impressed with the compatibility of software after the upgrade and I wouldn’t let this area hinder your upgrade to Leopard.

**Command + Tab**

One of the most used keyboard shortcuts I use religiously is switching between applications using Command + Tab. Now this hasn’t broken but if you’re using this shortcut to switch between applications on different spaces there is a really weird bug that seems to have crept in.

Switching apps using this shortcut in the same space is fine but between different Spaces you find that instead of selecting the application straight away you now have to click on the application to make it active. This means that I tab to my app on another Space and then I have to use my mouse to select the current window so I can use the application.

It’s not a deal-breaker for me but definitely something that needs to be addressed.

**Final Thoughts**

With 300+ new features to Leopard (excluding all the other older ones) I am only mildly displeased with 4 of them. If I were you I’d buy a **very large** external hard drive, get your Leopard DVD and get on board for the ride.

I am still blown away by Leopard every time I use it and I’m really pleased with the innovation Apple have created with this release. I do get an impending sense that with the new [Cover Flow](http://www.apple.com/macosx/features/finder.html?ref=justhart.com) integrated into the Finder we’ll soon see a Mac computer that is completely touch screen and keyboard-less.

More to be revealed from Cupertino I guess!
