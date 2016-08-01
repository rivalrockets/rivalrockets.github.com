---
id: 561
title: 'Neatx: Remote Desktop for Linux'
date: 2010-04-18T23:40:31+00:00
author: Kit
layout: post
guid: http://rivalrockets.com/blog/?p=561
permalink: /2010/04/neatx-remote-desktop-for-linux/
aktt_notify_twitter:
  - no
dsq_thread_id:
  - 87451392
categories:
  - Computers
  - Linux
---
I had never even heard of NX technology until I began researching better ways to set up a VNC capable server on an Ubuntu machine that I had planned on running “headless”.  To make matters more confusing, this promising technology is scarcely documented, so I’m putting my findings here.

NX Technology, to briefly summarize, is similar in concept to RDP or Terminal Services on Windows, it basically provides a network ready way to log in and connect to a graphical desktop environment on a computer that you are not physically in front of.  The X Window System, the de-facto graphical backbone for Linux, has been able to send GUI over the network for years, but in practice it has proven inefficient and only feasible on the fastest of networks.  NX on the other hand, uses a combination of compression and caching on top of traditional X11 making for a much more bearable remote desktop experience.  As always, Wikipedia has a <a href="http://en.wikipedia.org/wiki/NX_technology" target="_blank">better explanation</a> than I’m able to provide here.

A company called <a href="http://www.nomachine.com/" target="_blank">NoMachine</a> provides commercial client and server NX software, selling Linux and Solaris server software while providing a free NX client for all the major OSes (including Windows).  Until recently, the only notable freely available NX server for Linux was FreeNX which took NoMachine’s open source core libraries and wrapped it up in a bunch of convoluted script files.  A small team has been incorporating the FreeNX code into an Ubuntu PPA, but have been having trouble maintaining compatibility and releasing bugfixes to the FreeNX code.  One quick glance at the <a href="http://freenx.berlios.de/" target="_blank">author’s site</a> reveals that it has been a couple years since any official <a href="http://en.wikipedia.org/wiki/Software_rot" target="_blank">updates have occurred</a>.   Now here’s where it gets interesting: last year Google GPL’ed its own internal version of the Free NX server called <a href="http://code.google.com/p/neatx/" target="_blank">Neatx</a>, which gives the open source community a fresh platform to work with.

## Installing Neatx on Ubuntu 10.04

I found the process of installing the NX server to be fairly straightforward, using the new PPA add script introduced in 9.10, I added the FreeNX Team PPA repository:

`$ sudo add-apt-repository ppa:freenx-team`

This slick command takes care of finding the FreeNX Team’s Launchpad PPA software repository and adds all the necessary keys etc. to be able to get the software contained within.  After the script has finished its magic you’ll need to update the repository cache:

`$ sudo apt-get update`

Then, install the necessary pieces:

`$ sudo apt-get install neatx-server`

This will gather all of the necessary NX server components and dependencies including things like the OpenSSH server.  And that’s it!  I had to reboot to get the SSH server up and running, but other than that, no additional configuration was required!

<p style="padding-left: 30px;">
  <span style="color: #ff0000;">Update:</span> a comment left by a reader indicated that rebooting the server is not necessary even after a fresh OpenSSH server install, and I am to expect that everything is ready to go as the install finishes (thanks to Woden for the feedback).
</p>

## Connecting to the NX server from another computer

On a your client machine, point the [freely available client](http://www.nomachine.com/download-client-windows.php) from NoMachine to the new Neatx server’s address, accept the key and presto!  You now have a slick remote desktop solution for Linux, congratulations!

[<img style="display: inline;" title="Windows with remote Linux.  Believe it!" src="/content/2010/04/neatxonnomachine_thumb.png" alt="Windows with remote Linux.  Believe it!" width="640" height="521" />](/content/2010/04/neatxonnomachine.png)