---
id: 430
title: 'Proof of Concept: The Economic Server Build'
date: 2009-03-16T23:10:24+00:00
author: Kit
layout: post
guid: http://rivalrockets.com/blog/?p=430
permalink: /2009/03/proof-of-concept-the-economic-home-server-build/
aktt_notify_twitter:
  - no
dsq_thread_id:
  - 77580673
categories:
  - Computers
  - PC Builds
---
Last weekend I had just received all the parts to complete what I felt was a pretty exiting build.  With the primary goal of low power consumption and secondary goal of fits-in-my-house, I chose MSI's new <a href="http://www.amazon.com/gp/product/B001R1X0I0?ie=UTF8&tag=rivalroccom-20&linkCode=as2&camp=1789&creative=390957&creativeASIN=B001R1X0I0" target="_blank">"Nettop" barebone</a>:

### MSI Wind Nettop 100

  * Intel Atom 330 (Dual-core with Hyperthreading!)
  * Small Form Factor (11.8" x 9.5" x 2.6")
  * Low Power Consumption (31 Watts idle, according to my Kill-A-Watt)

Okay, so now for some pictures:

<div id="attachment_431" class="wp-caption alignnone" style="width: 810px">
  <img class="size-full wp-image-431" title="msi-netserver" src="/content/2009/03/msi-netserver.jpg" alt="msi-netserver" width="800" height="594" />
  
  <p class="wp-caption-text">
    Here we see that the machine is quite an exercise in minimalism.
  </p>
</div>

<div id="attachment_432" class="wp-caption alignnone" style="width: 810px">
  <img class="size-full wp-image-432" title="drive_bay" src="/content/2009/03/drive_bay.jpg" alt="drive_bay" width="800" height="542" />
  
  <p class="wp-caption-text">
    Rather than waste what few bay expansion options I had, I opted to install this SATA hot-swap bay in place of a seldom-used CD drive for future storage/backup needs!
  </p>
</div>

<div id="attachment_433" class="wp-caption alignnone" style="width: 810px">
  <img class="size-full wp-image-433" title="msi-netserver-front" src="/content/2009/03/msi-netserver-front.jpg" alt="msi-netserver-front" width="800" height="314" />
  
  <p class="wp-caption-text">
    Here is a shot of the front of the "mini-server" after the SATA bay was installed. Note the presence of the multi-card reader...
  </p>
</div>

### MSI "Net_server_" Final Specs

  * CPU:  Intel Atom 330 Dual-core @ 1.6GHz with HTT 
      * This processor appears as four logical cores to the OS which could come in handy for dealing with many threads at once (simultaneous background tasks and multiple server requests)
  * Memory:  2GB SODIMM 
      * For the stripped down Linux Distro I'm using, this is overkill.  But at $19 there was no reason not to go for max capacity!
  * Storage:  74GB Raptor 10,000 RPM 
      * A trusty old standby from a previous PC build, rated at twice the lifetime of standard hard drives and for continuous operation, this is server-grade stuff.
  * Network: Gigabit Ethernet

## Conclusion

So far, I've been quite pleased with how the build went---there were a couple of snags when I set out to install the OS from a USB stick, my advice: just plunk down the cash for an external CD drive and save yourself the grief.

### Low Power Consumption, Kills 66% Fewer Baby Seals!

Operating between 30-40 watts, the Nettop platform sucks far less electricity from the wall than my daily PC (which _idles_ at around 150 watts!), the Intel Atom has some serious "green" cred. (sorry Brian, I couldn't avoid using the preppy word <g>).  Not to mention, stands to take a chunk out of monthly power bill.