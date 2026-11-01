---
title: Creating a mobile site with Yahoo! Blueprint
date: '2009-02-12T10:43:54.000+02:00'
lastmod: '2009-02-12T10:43:54.000+02:00'
slug: creating-a-mobile-site-with-yahoo-blueprint
tags:
  - Afrigator
  - Blueprint
  - Development
  - General
  - Mobile
  - Yahoo!
---

[Yahoo! Blueprint](http://mobile.yahoo.com/developers/roadmap?ref=justhart.com), in theory, is an amazing and agile mobile development framework. Yahoo! describes Blueprint as…

> …a platform for developing and distributing rich mobile Internet services. It offers a standards-based language, an easy-to-use toolkit, innovative features, and support across multiple runtime environments—allowing developers to maximize their reach across **thousands of mobile devices**.

When we first came across Blueprint at [Afrigator](http://afrigator.com/?ref=justhart.com) we got really excited about the possibilities. Here you can develop a mobile site in a standard XML format and by integrating your mobile application into Blueprint it would interpret the markup, detect the mobile phone a user is on and in turn render an optimised mobile version tailored just for their device.

Well not really! To test it out I created a very simple mobile application that will return all the header information sent from Yahoo! to your webserver about the mobile device. All I did was use a simple _getallheaders_ function wrapped in the Blueprint XML. In theory this simple application should render perfectly across thousands of devices.

Here’s my entire mobile application file which is accessible at [bp.justhart.com](http://bp.justhart.com/?ref=justhart.com).

  
    
      
        
          Mobile Headers
        
      

	 $value) {
		echo "".$name.": ".$value."";
	}
	?>
    
  

Accessing [bp.justhart.com](http://bp.justhart.com/?ref=justhart.com) on my iPhone the application returned the following results which I was really impressed with.

![Mobile Headers Application](/content/images/2009/02/img_0013_2.png)

So now I know the iPhone version works as expected but what about a Nokia 6610? Well the results are really disappointing. Instead of seeing the mobile headers all I get is a screen displaying my site description text (A simple application that shows you the headers from your mobile device.) with a message saying I need to install either Yahoo GO! or Opera Mini to view the application.

I tried to Install Yahoo GO! on the Nokia 6610 but I got another message saying my _Windows Mobile_ device was not supported. How did a Symbian operating system become Windows Mobile? Anyway, I digress, I then installed Opera Mini as this was my only step left but alas more problems exist.

When accessing [bp.justhart.com](http://bp.justhart.com/?ref=justhart.com) from within Opera Mini all I get is the same message, this time in French, asking me to install either Yahoo GO! or Opera Mini. Now I’m not sure if this is a Nokia 6610 problem as Opera Mini won’t work either but Yahoo! Blueprint has just failed a very simple test.

Yahoo! claim that they support thousands of mobile devices and as long as a mobile supports XHTML (including tables, forms and GIF/PNG/JPG images) and CSS2 then it should render perfectly. As you can tell my results are not as expected.

For now Blueprint has been thrown out the window as a new framework for us to develop Afrigator’s new mobile site. If it can’t even handle a 6610 then I have to wonder what phones it really will support.

I wonder if you guys can help me by accessing [bp.justhart.com](http://bp.justhart.com/?ref=justhart.com) on your mobile phone and letting me know what you see. If you manage to see all your mobile headers then you know it’s working. If you do decide to help, please post your mobile phone manufacturer and model in the comment form below. Also, let me know if it works in Opera Mini on your side.
