---
title: How to swap Control and Command keys on PowerPC
date: '2006-12-21T00:17:14.000+02:00'
lastmod: '2007-06-01T02:19:07.000+02:00'
slug: how-to-swap-control-and-command-keys-on-powerpc
tags:
  - Debian
  - Ubuntu
---

As a previous Apple OS X user I find that having to use the control key on my keyboard versus the Apple command key a real pain in the backside. Most Windows users don’t have a problem with this as the transition from Windows to Linux is easy with regards to using the control key. I’ve searched and asked and low and behold nearly a month later I now know how to swap the two around.

In Ubuntu and Debian it’s not as simple as configuring a shortcut or keymap and it requires a little bug-fix to get it working just as I’m used to it coming from OS X. Here’s a little step-by-step HOW-TO on how to achieve this on both an iBook G4 keyboard as well as the standard Apple USB keyboard.  
  
**iBook G4 Keyboard (I guess this will work on most Apple notebooks)**

Create a file in your home directory called .Xmodmap by following these steps.

In a terminal window type:

> `cd $home   vim .Xmodmap`

In this new file add these two lines:

> `keycode 115 = Control_L   add Control = Control_L`

From your terminal window:

> `xmodmap ~/.Xmodmap`

Restart your computer and the next time you log in to Ubuntu or Debian it will prompt you to load your .Xmodmap file. Select it from the right side of the window and move it to the left and then load it. Once done your left apple key is now a ctrl key.

**Standard Apple USB Keyboard**

Follow the exact same steps as above but instead of inserting two lines in the .Xmodmap insert the following:

> `remove Control = Control_L   remove Mod4 = Meta_L   keycode 0x25 = Meta_L   keycode 0x73 = Control_L   add Control = Control_L Control_L   add Mod4 = Meta_L`

The second example above will make both your Apple command keys control keys, disabling your control key completely and adds a bit more functionality for the larger Apple keyboards.

For both of these instructions you can also go into your keyboard shortcuts in gnome and change Alt+Tab application switching to Ctrl+Tab to allow you to switch between applications using your command+tab keys.
