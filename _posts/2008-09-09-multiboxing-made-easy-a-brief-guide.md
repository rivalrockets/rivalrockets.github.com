---
id: 161
title: '&#8220;Multiboxing&#8221; Made Easy: A Brief Guide'
date: 2008-09-09T23:24:30+00:00
author: Kit
layout: post
guid: http://rivalrockets.com/blog/?p=161
permalink: /2008/09/multiboxing-made-easy-a-brief-guide/
aktt_notify_twitter:
  - no
  - no
  - no
  - no
  - no
  - no
  - no
  - no
  - no
dsq_thread_id:
  - 77580570
categories:
  - How to
  - Uncategorized
  - WoW
---
<div id="attachment_243" class="wp-caption alignnone" style="width: 410px">
  <a href="/content/2008/09/multibox-sm.png"><img class="size-medium wp-image-243" title="Multibox Screenshot" src="/content/2008/09/multibox-sm-400x250.png" alt="" width="400" height="250" /></a>
  
  <p class="wp-caption-text">
    The simplest way to run two instances of WoW
  </p>
</div>

Brian had mentioned on more than one occasion the practice of &#8220;multiboxing&#8221; which as best as I can define: a single user running two ore more World of Warcraft accounts at the same time.

I had always precieved that there was a certain level of complexity to operating two machines at the same time (multiple keyboards/mice, using KVM, etc.) however, it&#8217;s really quite simple:

  * World of Warcraft permits mulitple instances as-is.
  * WoW also has a &#8216;Windowed mode&#8217; for reducing your gaming experience down to a manageable 1024&#215;768 or even 800&#215;600 window.

Now the final ingredient to this recipe is my trusty **1st-generation G15 keyboard**:

<img class="alignnone size-full wp-image-164" title="g15_550px" src="/content/2008/06/g15_550px.jpg" alt="macro to your heart\'s content..." width="500" height="251" />

Equipped with a _gratuitous_ 18(!) macro keys (which was later revised to a manageable 6 in the second revision), setting ready-made commands up is a snap:

[<img class="alignnone size-thumbnail wp-image-163" style="vertical-align: baseline;" title="g15panel" src="/content/2008/06/g15panel-180x180.png" alt="" width="180" height="180" />](/content/2008/06/g15panel.png)

For this demonstration, my &#8220;slave&#8221; account is my wife&#8217;s level 62 priest who makes a good heal-bot <g>

### The basic multiboxing strategy is as follows:

  1. **Set &#8216;slave&#8217; character to follow the &#8216;master&#8217; character** &#8211; this is accomplished by hard-coding the sequence into a G15 macro titled &#8220;Follow Me&#8221;: 
      1. Alt-Tab, to change focus from the master window to the slave&#8217;s window.
      2. &#8220;/target _<character name>_&#8221; this command, hard-coded to the master character&#8217;s name guarantees the right character is being followed.
      3. &#8220;/f&#8221; &#8211; to set the slave character to follow
      4. Alt-Tab  to return focus to the master&#8217;s window.
  2. **Use slave healer & support functions when necessary** &#8211; this requires the use of multiple &#8220;G-Keys&#8221; my personal preference is to use two macro sets (M1 and M2) one for solo multiboxing, and one for full group use.  This is accomplished in much the same way that the follow command is accomplished: 
      1. Alt-Tab
      2. F1, F2, F3, F4, or F5 to select the desired party member (note: use one G-key per party member)
      3. Cast desired spell
      4. Alt-Tab  to return focus to the master&#8217;s window.

Note that during battle, healers need to be standing still to get their heals cast, so be sure to use the &#8220;stop follow&#8221; command

So the layout for a priest command set on the G15 would go something like this:

<table style="height: 348px;" border="1" width="400">
  <tr>
    <td>
      Quick Heal Slave
    </td>
    
    <td>
      Quick Heal Master
    </td>
    
    <td>
      Psychic Scream
    </td>
  </tr>
  
  <tr>
    <td>
      Normal Heal Slave
    </td>
    
    <td>
      Normal Heal Master
    </td>
    
    <td>
      Fade
    </td>
  </tr>
  
  <tr>
    <td>
    </td>
    
    <td>
    </td>
    
    <td>
    </td>
  </tr>
  
  <tr>
    <td>
      Big Heal Slave
    </td>
    
    <td>
      Big Heal Master
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Aquatic (Master)</span>
    </td>
  </tr>
  
  <tr>
    <td>
      Power Word Shield Slave
    </td>
    
    <td>
      Power Word Shield Master
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Bear Form (Master)</span>
    </td>
  </tr>
  
  <tr>
    <td>
    </td>
    
    <td>
    </td>
    
    <td>
    </td>
  </tr>
  
  <tr>
    <td>
    </td>
    
    <td>
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Cat Form (Master)</span>
    </td>
  </tr>
  
  <tr>
    <td>
      Stop Following Master
    </td>
    
    <td>
      Follow Master
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Travel Form (Master)</span>
    </td>
  </tr>
</table>

This layout resides in memory set one (M1) on my keyboard its purpose is for soloing with the multibox slave assisting the master.

Set 2&#8242;s (M2) macro layout focuses on full party play such as instances or group quests by switching up the layout to cover heals/buffs for up to five party members Note the use of two major spells in columnar format:

<table style="height: 348px;" border="1" width="400">
  <tr>
    <td>
      Quick Heal Slave (P1)
    </td>
    
    <td>
      Big Heal Slave (P1)
    </td>
    
    <td>
      Psychic Scream
    </td>
  </tr>
  
  <tr>
    <td>
      Quick Heal P2
    </td>
    
    <td>
      Big Heal P2
    </td>
    
    <td>
      Fade
    </td>
  </tr>
  
  <tr>
    <td>
    </td>
    
    <td>
    </td>
    
    <td>
    </td>
  </tr>
  
  <tr>
    <td>
      Quick Heal P3
    </td>
    
    <td>
      Big Heal P3
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Aquatic (Master)</span>
    </td>
  </tr>
  
  <tr>
    <td>
      Quick Heal P4
    </td>
    
    <td>
      Big Heal P4
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Bear Form (Master)</span>
    </td>
  </tr>
  
  <tr>
    <td>
    </td>
    
    <td>
    </td>
    
    <td>
    </td>
  </tr>
  
  <tr>
    <td>
      Quick Heal P5
    </td>
    
    <td>
      Big Heal P5
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Cat Form (Master)</span>
    </td>
  </tr>
  
  <tr>
    <td>
      Stop Following Master
    </td>
    
    <td>
      Follow Master
    </td>
    
    <td>
      <span style="color: #888888;">Personal key:<br /> </span><span style="color: #888888;">Druid Travel Form (Master)</span>
    </td>
  </tr>
</table>

Note that the importance of the Start/Stop Following Master commands is not to be underestimated!  To avoid interrupting healing spells during cast, the slave needs to be stationary.  Forcing the master to remember to hold still during critical healing moments is not an effective way to go about it, quickly &#8220;parking&#8221; the healer with the &#8220;Stop Following&#8221; (Alt+Tab, down arrow, Alt+Tab) command resolves this.