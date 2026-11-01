---
title: Apple iCal / Microsoft Exchange fix for Leopard
date: '2008-03-31T11:01:06.000+02:00'
lastmod: '2008-08-28T15:42:00.000+02:00'
slug: apple-ical-microsoft-exchange-fix-for-leopard
tags:
  - Apple
  - Bugs
  - Exchange
  - General
  - Hacks
  - iCal
  - iCalFix
  - Leopard
  - Microsoft
  - Projects
---

One of the major drawbacks to working on an Apple Mac in a large corporate company is that most IT departments still use Microsoft Exchange Server for email and calendar support.

While we’ve found many a work-around to get email up and running using Apple Mail there remains this irritating bug that prevents Exchange iCal events from syncing correctly with Apple iCal.

The reason this bug exists is because Exchange doesn’t use standard compliant timezone information while Apple does and as a result iCal can’t figure out what the correct timezone is from Exchange iCal invitations. Here’s a quick example of the South African timezone differences between the two.

**Exchange uses this format:**  
`(GMT+02.00) Harare/Pretoria`

**While iCal uses this:**  
`Africa/Johannesburg`

This means that when a meeting request comes in from a Windows PC, iCal can’t read data beyond the GMT+02.00 and it simply adds on 2 hours to the event. So a meeting sent from Exchange, scheduled for 14:00 actually appears in iCal as 16:00. We’ve missed many a meeting as a result!

Over the last few months I’ve spent countless hours trying to find a fix but no one has managed to get this issue resolved – not even Apple. I’ve now resorted to creating my own bug fix which I’m releasing publicly this morning.

**How this bug fix works**

The install script downloads all the necessary files from my server and installs both an AppleScript and Shell script to a folder called iCalFix in your Applications folder.

The AppleScript is then assigned to a Mail Rule and runs whenever an iCal invitation is received. The AppleScript downloads the iCal file to a temporary location and the Shell script then runs on the temp file and replaces any incorrect timezone information.

Once completed the new iCal event is then imported to iCal with all the new timezone data in place. The beauty of this fix is that you don’t need to edit any of the package files for iCal and even your original iCal invitations are left untouched. This means that you can upgrade iCal at a later stage and you should be safe from any data corruption.

**Installation**

1\. Download this [Install Script](/ccount/click.php?id=2) to your computer and extract the contents from the ZIP file. The folder contains a Shell script (install.sh) which sets everything up for you.

![ical-installfolder.png](/content/images/2008/03/ical-installfolder1.png)

2\. Right-click on the **install.sh** file, select _Open With_ and then click on _Other_.

![ical-openwith.png](/content/images/2008/03/ical-openwith.png)

3\. Click on **Applications –> Utilities –> Terminal**. If you can’t select Terminal from the Open dialog then select _All Applications_ from drop-down list below.

![ical-openterminal.png](/content/images/2008/03/ical-openterminal.png)

4\. Terminal will open up and the install script will run. When you see the message “Installation Complete.” you can close Terminal.

![ical-terminal.png](/content/images/2008/03/ical-terminal.png)

5\. You can now check if the bug fix was installed correctly by navigating to **/Applications/iCalFix/** in Finder. If you see two files installed in that folder then installation was successful.

![ical-folder.png](/content/images/2008/03/ical-folder.png)

**Setting up the Mail Rule**

The last step before you can begin using this fix is to setup an email rule that calls the AppleScript file. Click on **Mail –> Preferences –> Rules** and create a new rule that looks identical to the one below.

![ical-mailrules.jpg](/content/images/2008/03/ical-mailrules.jpg)

_If you’d like to read detailed instructions on setting up this particular Mail Rule then make sure you read the readme.txt file located in the Install Script package._

**All done!**

After completing the above steps any new iCal invitations sent from an Exchange server will automatically be converted to the right formats and you will never have an excuse to be 2 hours late for a meeting again!

I suggest that you test this fix out by sending an iCal event from an Exchange server to see if all is working correctly. If the fix isn’t working for you then your exchange server is probably using a different timezone format and you’ll need to read the section in the readme.txt file on _customising timezone support for your country_.

**Caveats**

-   **NB: Make sure you open the readme.txt file in the Install Script folder. This readme file contains important information which isn’t included in this post.**
-   This fix has only been tested on Mac OS X Leopard 10.5.1 and 10.5.2 and there is no guarantee that it will work on previous or future versions.
-   ~We’ve only been able to test this fix on three MacBook Pros and while it worked on all three YMMV.~ We’ve now tested it on about 10 Macs now and it has worked on every one we’ve tested thus far.
-   Before installing or running this fix make sure you backup your iCal first. In iCal click **File –> Back up iCal…** and save a backed up version to your computer.
-   When you recieve an Apple iCal invitation there is a message that pops up in iCal saying that “no data was added to iCal” but when you click OK the iCal event is loaded to iCal anyway. I’m not sure why this happens with iCal but I’m working on a fix for that.
-   I can’t provide support. If you want help in setting up a unique timezone regular expression then I’ll assist with that but any other queries I cant’t respond to – I just don’t have the time, sorry.
