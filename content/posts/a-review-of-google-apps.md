---
title: A review of Google Apps
date: '2007-07-10T17:45:56.000+02:00'
lastmod: '2007-07-10T20:09:46.000+02:00'
slug: a-review-of-google-apps
tags:
  - Google
---

[Google Apps](http://google.com/a/?ref=justhart.com) has been out there for some time now and when I initially looked at it I wasn’t really sold on the benefits of using the service. To me the free version appeared to function in exactly the same was as a normal Google Account but I’m pleased to report that this is actually not the case.

Some of the key problems I’m faced with today is centralisation and sharing. What I mean to say is that I have so many different email accounts that I’ve really struggled to manage and having some accounts download on a computer while others I check online is not ideal to say the least.

With the recent introduction of Gmail’s POP access you could now check up to 5 other email accounts and have those accounts mail imported to your Gmail account but this just wasn’t cutting it for me. The main reason this system is flawed is evidenced by the fact that Gmail only checks your other POP accounts every 45 – 60 minutes and in my world this just isn’t good enough. I need email immediately – end of story.

My other problem is the ability to share documents, calendars and other information with people in my family which up until Google Apps was a mission.

About two weeks ago I decided to try out Google Apps and went through the process of setting up a new domain, hartmanlife.com, to use with the service. This is a pre-requisite by the way so if you don’t have your own domain or can’t administer your domain name then Google Apps is not for you.

I’ve been very pleased with the results thus far, even despite some inherent flaws with the system and the following is a quick howto on setting up the interface and using Google Apps.  
  
**Create a Google Apps Account**  
Setting up a Google Apps account is as easy as any other process on Google and this really doesn’t need any special mention. You should be able to figure this one out by yourself. The only complicated process when doing this is choosing a domain name to use as your primary Google Apps domain and then verifying that the domain is actually yours but Google really help you through this process.

For my test I registered [www.hartmanlife.com](http://www.hartmanlife.com/?ref=justhart.com) with [GoDaddy](https://www.godaddy.com/?ref=justhart.com) and in doing so I was able to setup my domain to use the full power of Google Apps.

**The Dashboard**

[![Dashboard](/content/images/2007/07/dashboard.jpg)](/content/images/2007/07/dashboard.jpg "Dashboard")

The Apps Dashboard provides not only an overview of your account usage but also contains a Services settings section which allows you to make quick changes to the services available on Google Apps.

**Service Settings**

[![Services](/content/images/2007/07/services.jpg)](/content/images/2007/07/services.jpg "Services")

I decided to point all of the available services to sub-domains on my account so I had to login to my domain control panel at GoDaddy and make some changes to my [DNS](http://en.wikipedia.org/wiki/DNS?ref=justhart.com) settings. Here is a screenshot of what changes I had to make.

![GoDaddy.com DNS Changes](/content/images/2007/07/godaddy.jpg)

By adding these settings for my domain I can now access the various services at the following locations:

-   Email (Gmail): [http://mail.hartmanlife.com](http://mail.hartmanlife.com/?ref=justhart.com)
-   Start Page (iGoogle): [http://start.hartmanlife.com](http://start.hartmanlife.com/?ref=justhart.com)
-   Calendar: [http://calendar.hartmanlife.com](http://calendar.hartmanlife.com/?ref=justhart.com)
-   Docs & Spreadsheets: [http://docs.hartmanlife.com](http://docs.hartmanlife.com/?ref=justhart.com)
-   Web (Google Pages): [http://www.hartmanlife.com](http://www.hartmanlife.com/?ref=justhart.com)

**User Accounts**

[![User Accounts](/content/images/2007/07/user-accounts.jpg)](/content/images/2007/07/user-accounts.jpg "User Accounts")

By accessing the User Accounts menu you can easily add a new account for the domain as well as edit an existing account. You also have the option to deny access to any/all of the Google Apps services for a particular account so certain users can essentially have limited access. There is also a nice usage graph so you can check how much space accounts are using on the server.

**Domain Settings**

[![Domain Settings](/content/images/2007/07/domain-settings.jpg)](/content/images/2007/07/domain-settings.jpg "Domain Settings")

The Domain Settings tab allows you to setup vital information about the primary domain and more importantly it also allows you to add multiple domains to your account.

One of the really cool features is the ability to add your own logo to Gmail and Google Calendar & Docs and while I haven’t yet done this myself I have changed the title bar of my browser so it doesn’t read as Gmail when I’m accessing my mail.

[![Domain Logo](/content/images/2007/07/domain-logos.jpg)](/content/images/2007/07/domain-logos.jpg "Domain Logo")

**Adding Multiple Domains**

[![Domain Settings](/content/images/2007/07/domain-settings.jpg)](/content/images/2007/07/domain-settings.jpg "Domain Settings")

You can also add multiple (or alias) domains to your account under the Domain Settings tab. Adding an alias domain allows you to send and receive email for that domain and it means that as email arrives it is delivered to your Apps Gmail instantaneously – a much better option to POP access.

Physically adding the domain to the control panel is easy however actually making it work is another story. As with your primary domain you will need to modify your [Mail Exchanger](http://en.wikipedia.org/wiki/MX_record?ref=justhart.com) (MX) settings in your DNS in order for you to be able to receive email. The good news is that Google have created step-by-step howtos for almost every single domain registry company including [Cpanel](http://www.cpanel.net/?ref=justhart.com) which I was very impressed with.

In my case however I had to manually edit my DNS zone file and below are the required changes I made to an alias domain I’ve added.

[![DNS Settings](/content/images/2007/07/dns.jpg)](/content/images/2007/07/dns.jpg "DNS Settings")

Something to note about using multiple domains is that if you change the MX records for your domain all email will be sent to Google Apps. This could be a problem if for example you manage a domain that has multiple email accounts but you don’t want to create accounts for those users in Google Apps. Every current email account will need a user account in Google Apps for your users to continue to receive uninterrupted email for an alias domain.

That said, if you have multiple email accounts that forward to one primary account for an alias domain then you can setup a catch-all account in Google Apps that will catch all the email sent to a domain that isn’t associated with a Google Apps account.

**Advanced Tools**

The advanced tools tab is very simplistic and only provides a tool for importing multiple accounts to your new Apps account. I would assume that the advanced tool tab increases when you upgrade to a [Premier Account](http://www.google.com/a/help/intl/en/admins/editions_spe.html?ref=justhart.com) but for the Standard Version it leaves much to be desired.

**Service Settings Tab**

![Services Settings](/content/images/2007/07/service-settings.jpg)Apart from the quick access functions you have on the Dashboard Google have dedicated an entire menu to Service Settings and clicking them will take you to… you guessed it the settings for that service. I’m only hoping that in time more of Google’s services will be added to this menu.

**The Applications**

The **Start Page** application is really cool and modeled off [iGoogle](http://www.google.com/ig?ref=justhart.com). It seems though that a lot of iGoogle’s functionality has been stripped for Start Page so I’m looking forward to future releases that allow true iGoogle interaction

Email, Calendar and Docs & Spreadsheets function exactly as the free community counterparts associated with all Google Accounts. However there are a few marked differences.

-   The customised Title bar and Logo across all these services allowing you to maintain your brand across the platforms.
-   User accounts that belong to the domain are already shared across all the platforms. In Email this means you’ve got all users of the domain as a contact and they’re already authorised as Google Talk users. For Calendar and Docs & Spreadsheets there is a function to share calendars and docs across the domain accounts which means you can now manage family/group life with all your members.

**Google Talk** just can’t be tested unfortunately. I don’t have a PC and the only way to link up your Apps account in Gtalk is to use the PC-based application. I tried at length to add my Google Apps account to the normal [Jabber](http://en.wikipedia.org/wiki/Jabber?ref=justhart.com) servers but it would appear that Google Apps domains won’t yet work with Jabber, unlike Google Accounts.

**Web Pages** seem to work fine. I played around with this briefly for my domain but as I won’t really be using this service I’ll leave the decision-making process up to you on this one.

**My Conclusion**

While I initially thought Google Apps was a waste of time I have to admit to being very wrong. As a family or social group Google Apps can be a very nice tool to collaborate with and it has already allowed me to streamline my communication with my family in a centralised and managed place.

My only real criticism, and potential deal-breaker for some, is that Google Apps accounts don’t work like a Google Account. I was expecting to now login to [Analytics](http://www.google.com/analytics?ref=justhart.com), [Groups](http://groups.google.com/?ref=justhart.com), [Reader](http://www.google.com/reader?ref=justhart.com) and other [standard services](http://www.google.com/intl/en/options/?ref=justhart.com) I use on Google with my new Apps account but this is not possible.

There is no migration tool to move an existing Google Account to Apps and this is seriously lacking IMHO. I’m sure that Google will move to this direction in the future but at the moment it’s really complicated having to log into certain services using my old Gmail details and others using the Google Apps details.

Migrating email from my Gmail account was also a little bit of a pain and the only way to achieve this was to setup POP Access in my new account and allow Google to import my old Gmail email which took nearly a week and a half to complete. It didn’t cost me any time however you should be able to merge the two accounts together as I’m now running two Gmail instances.

The one final thing I’d like to see change and I’m sure it will is the ability to setup different accounts pointing to one Google Apps account. In my case my primary account is justin@hartmanlife.com and any email sent to justin@aliasdomain will come to my hartmanlife.com domain. The problem with this is that I can’t setup say info@aliasdomain to forward to justin@hartmanlife.com which is a small but irritating problem.

So while I’m largely pleased with the Standard Edition I’ve been thinking about a possible move to Premier Edition. For me the $50 per year is a little steep just so I can have more disk space, a 99.9% uptime guarantee and 24-hour technical support. These benefits are more suited for corporate organisations but I simply can not see how a company would want to use this service.

It is a great tool for non-commercial purposes but to roll this out into an organisation posses a huge security and privacy threat. Why would any company want their private communication, business strategy documents and vital financial budgets located on someone else’s server and then pay them to do so?

I’m lost, however I’ll continue using Apps with much joy.
