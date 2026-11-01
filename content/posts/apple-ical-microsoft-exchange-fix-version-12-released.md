---
title: Apple iCal / Microsoft Exchange fix version 1.2 released
date: '2008-08-28T15:48:20.000+02:00'
lastmod: '2008-08-28T15:48:20.000+02:00'
slug: apple-ical-microsoft-exchange-fix-version-12-released
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

I have updated the [Apple iCal / Microsoft Exchange fix for Leopard](/2008/03/31/apple-ical-microsoft-exchange-fix-for-leopard/) with a bug fix and a few enhancements.

Here are the release notes for this version:

-   Fixed = iCal bug message saying “no data was added to iCal” thanks to Jon Milan.
-   Added = London timezone support thanks to Ryan Hunt.
-   Added = West Coast USA timezone support thanks to Ryan Hunt.
-   Added = Tallinn timezone support thanks to Ryan Hunt.
-   Added = Asia/Muscat timezone support thanks to Steve.
-   Tests = Now confirmed to work on Leopard 10.5.1, 10.5.2, 10.5.3 and 10.5.4
-   Tests = Now confirmed to work on all Apple computers.

**Installing**

If you’ve never installed this fix before then please read the detailed installation instructions [found over here](/2008/03/31/apple-ical-microsoft-exchange-fix-for-leopard/). If you’re upgrading from a previous version please read the detailed upgrade notes below.

**Upgrading from version 1.1**

1\. Delete the folder **/Applications/iCalFix/** in Finder.

![](/content/images/2008/08/delete-icalfix.png)

2\. Download this [Upgrade Script](/ccount/click.php?id=3) to your computer and extract the contents from the ZIP file. The folder contains a Shell script (install.sh) which sets everything up for you.

![ical-installfolder.png](/content/images/2008/03/ical-installfolder1.png)

3\. Right-click on the **install.sh** file, select _Open With_ and then click on _Other_.

![ical-openwith.png](/content/images/2008/03/ical-openwith.png)

4\. Click on **Applications –> Utilities –> Terminal**. If you can’t select Terminal from the Open dialog then select _All Applications_ from drop-down list below.

![ical-openterminal.png](/content/images/2008/03/ical-openterminal.png)

5\. Terminal will open up and the install script will run. When you see the message “Installation Complete.” you can close Terminal.

![ical-terminal.png](/content/images/2008/03/ical-terminal.png)

6\. You can now check if the bug fix was installed correctly by navigating to **/Applications/iCalFix/** in Finder. If you see two files installed in that folder then installation was successful.

![ical-folder.png](/content/images/2008/03/ical-folder.png)

7\. Done. Sit back and enjoy.
