  
  

<p align="center">
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_15a239e018104482.png"
id="Image5" data-hspace="4" data-vspace="8" data-border="2" width="456"
height="605" />
</p>

***The internet may not be there when you need it.***

It's easy to take our communications infrastructure for granted, but the
internet, phone, and electrical systems are more fragile than you may
think. Hurricanes, tornadoes, and winter storms knock out power to huge
regions on a regular basis, with large-scale repairs sometimes
stretching to weeks. Even on a good day, these networks require constant
monitoring and maintenance to keep working.

Sometimes there isn't enough bandwidth to go around. It's common to lose
cell service when you're in a crowd because the network is overloaded.
In a natural disaster, phone lines can get jammed as people check on
loved ones. And many regions have no cell service at all.

Using the internet can also be risky. If you're trying to arrange an
abortion in a fascist-run state, there's a real chance your online
activity might be used against you. If you're attending a protest,
simply connecting to the cell network creates metadata that confirms you
were there.

It's good to have options, just in case.

Radio amateurs (a.k.a. hams) have been texting over the airwaves for
decades, using APRS (Automatic Packet Reporting System). But getting a
ham license requires taking a test, and encrypted communication is
strictly forbidden on the ham bands.

LoRa (short for long range) is a radio modulation technique introduced
in 2015 that makes it possible for low-power devices to send data over
long distances, up to several miles.

This project also demonstrates how much you can do with low-power
electronic communications. It's apparent that we need to shift to
renewable energy in the coming years, but we can't sustainably
manufacture enough solar panels and wind turbines to support the level
of energy consumption we're used to in the U.S. and Europe.

**What is LoRa?**

LoRa is short for **Lo**<span style="font-weight: normal">ng
</span>**Ra**<span style="font-weight: normal">nge radio. This protocol
ideal for low-speed data transmission like text chat. It can't be used
to transmit pictures or videos. </span>

LoRa implements chirp spread spectrum (CSS) modulation, meaning that it
is robust to channel noise and resistant to multi-path fading, resulting
in low interference.

  
  

**How far can it transmit?**

In a rural area with clear line-of-site for miles around the range of a
LoRa node can be up to six miles (10kms)! However, in a city where there
are lots of houses at the same level as you and your node, the range is
more likely to be just one to three blocks.

  
  

**What is a mesh network?**

In order for nodes that are far away from each other to communicate,
they will utilize nodes that are in between.

<p align="center">
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_d2d7590c2b9fb475.png"
id="graphics6" data-align="left" data-hspace="4" data-vspace="8"
width="598" height="375" />
</p>

In the example shown above, Alice and Charlie are too far away from each
other to send messages directly using a LoRa node. However, Bob is
located between and within range of both of them and Bob's node passes
the message on.

<p align="center"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_5385a551e512a42c.png"
id="graphics7" data-align="left" data-hspace="4" data-vspace="8"
width="598" height="292" /></p>

In a densely constructed city very high locations can still achieve long
range. For this reason, it is more effective to install your device at a
higher elevation. Installing the device in your second story window is
better than the first floor, and leaving the device on the roof is
better than both of those locations!

  
  

➡️**What is Meshtastic?**

Meshtastic is an open source, off-grid, decentralized, mesh network
built to run on affordable, low-power devices like the
<span style="text-decoration: none"><span style="font-style: normal"><span style="font-weight: normal"><span style="text-decoration: none">Heltec
LoRa32 V3 that comes in the Meshtastic kit from Iffy
Books.</span></span></span></span>

  
  

**What is a lithium-ion battery?**

A lithium-ion battery is a lightweight, high-efficiency battery. It is
more expensive than other types of batteries, but offers a high depth of
discharge, lifespan, charging rate.

  
  

**What is a charge controller?**

A charge controller regulates the voltage and current from the solar
panel to the battery and the load by controlling the charging rate.
Without the charge controller, excess solar power from the panel could
overcharge the battery.

  
  

➡️**What is a voltage regulator circuit?**

<span lang="en-US">A voltage regulator circuit stabilizes fluctuating
inputs to a fixed output to prevent even the slight chance of
overcharging. The MCP1700 is a low-dropout positive (incoming) voltage
regulator. It consumes a fraction (</span>1.6 µA) of what it can deliver
(250 mA) leading to a longer battery life and is ideal for single
lithium-ion batteries.

<p align="center">
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_994191d947a50e8e.png"
id="Image102" data-align="left" data-hspace="4" data-vspace="8"
width="127" height="159" />
</p>
  
  

**What is a decoupling capacitor?**

A decoupling capacitor will help smooth out short-term voltage spikes
found in noise in the power supplies. For example, if the voltage
suddenly drops, it’ll have enough power to counter act this change. If
the voltage suddenly increases, it’ll be able to absorb that power.

  
  

***Now it's time to learn how to make your own!***

***Parts***

  
  

**Included in your kit:**

<div align="center"><table width="100%" data-cellpadding="5" data-cellspacing="0"
style="page-break-inside: auto">
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td width="50%"
style="background: transparent; border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Heltec LoRa32 V3</span></p></td>
<td width="50%"
style="background: transparent; border: 1px solid #000000; padding: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_5c70b5d2f2b5aa98.png"
id="graphics1" data-align="left" data-hspace="4" data-vspace="8"
width="288" height="143" /><br />
<br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• 6-Volt, 6-Watt monocrystalline solar
panel</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_286cc10bd882e125.png"
id="Image23" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="202" height="198" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• TP4056 battery charger
board</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_17209c6874deb621.jpg"
id="graphics2" data-align="left" data-hspace="4" data-vspace="8"
width="234" height="216" /><br />
<br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Button-top 18650 lithium-ion
battery</span></p>
<p><br />
</p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_ed87d71acf0e297f.png"
id="Image19" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="211" height="100" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• 18650 battery clip</span></p>
<p><br />
<br />
</p>
<p><br />
<br />
</p>
<p><br />
</p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_3332376d9402b44b.png"
id="Image41" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="211" height="148" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• MCP1700-3302E low-dropout (LDO)
regulator</span></p>
<p><br />
<br />
</p>
<p><br />
</p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_3355a71e1802ed38.png"
id="Image29" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="48" height="140" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• 100uF electrolytic
capacitor</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_23016a00889b247c.png"
id="Image18" data-hspace="4" data-vspace="8" data-border="0" width="94"
height="224" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• 100nF ceramic capacitor</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_b9ae402fb6b8da43.png"
id="Image17" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="76" height="205" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Perfboard</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• SH1.25 port and plug
connectors</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_4aec7b4e8b6ee5d0.jpg"
id="graphics3" data-align="left" data-hspace="4" data-vspace="8"
width="209" height="202" /><br />
<br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Barrel plug</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_e44a547bf41b0665.jpg"
id="graphics13" data-align="left" data-hspace="4" data-vspace="8"
width="230" height="85" /><br />
<br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• 3/32" heat shrink tubing (~2" long)
x2</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_e550f70b553ec3f2.png"
id="Image24" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="96" height="190" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Cable tie bases</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_fcd86f4a2bce2bdc.jpg"
id="graphics14" data-align="left" data-hspace="4" data-vspace="8"
width="288" height="174" /><br />
<br />
</p></td>
</tr>
</tbody>
</table>

  
  

  
  

**Parts you'll need to provide yourself:**

  
  

<table width="100%" data-cellpadding="5" data-cellspacing="0"
style="page-break-inside: auto">
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td width="50%"
style="background: transparent; border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Weatherproof enclosure</span></p>
<p><span style="text-decoration: none">(See the step titled “Choosing a
waterproof enclosure) </span></p></td>
<td width="50%"
style="background: transparent; border: 1px solid #000000; padding: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_78bfa788d5f20f56.png"
id="Image26" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="182" height="138" /> </span></p></td>
</tr>
<tr class="even">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Brick (optional; for weighing down the
enclosure)</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_569dc723d5d8c665.png"
id="Image27" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="154" height="89" /> </span></p></td>
</tr>
<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Electrical tape</span></p></td>
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_81ba75ee823d6c99.jpg"
id="graphics8" data-align="left" data-hspace="4" data-vspace="8"
width="135" height="142" /><br />
<br />
</p></td>
</tr>
</tbody>
</table>

  
  

  
  

**You’ll also need the following tools and supplies.**

<table width="100%" data-cellpadding="5" data-cellspacing="0"
style="page-break-inside: auto">
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td width="50%"
style="background: transparent; border-top: 1px solid #000000; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0.04in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Soldering iron</span></p></td>
<td width="50%" data-valign="top"
style="background: transparent; border: 1px solid #000000; padding: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_690ecbdca1a51711.png"
id="Image33" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="211" height="104" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Lead-free solder</span></p></td>
<td width="50%" data-valign="top"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_a5c00efd78c3422d.png"
id="Image32" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="211" height="80" /> </span></p>
<p><br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Helping hands tool (optional, but makes
things easier!)</span></p></td>
<td width="50%" data-valign="top"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_aaa50533be01bb17.png"
id="Image6" data-align="left" data-hspace="4" data-vspace="8"
width="186" height="241" /><br />
<br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Wire strippers (or use wire
cutters/scissors... even a knife will work in a pinch)</span></p></td>
<td width="50%" data-valign="top"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_79fc8f246b5256db.jpg"
id="graphics4" data-align="left" data-hspace="4" data-vspace="8"
width="288" height="143" /><br />
<br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Drill with bits that can drill through
your weatherproof enclosure</span></p></td>
<td width="50%" data-valign="top"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_f7a7a01d22e9deea.jpg"
id="graphics5" data-align="left" data-hspace="4" data-vspace="8"
width="261" height="174" /><br />
<br />
</p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• Heat gun (or hair dryer)</span></p></td>
<td width="50%" data-valign="top"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><span
style="text-decoration: none"><img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_bf8b27727dccb25.png"
id="Image34" data-align="bottom" data-hspace="4" data-vspace="8"
data-border="0" width="176" height="125" /> </span></p></td>
</tr>

<tr class="odd">
<td width="50%"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: none; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0in"><p><span
style="text-decoration: none">• That glue that seals the washer in
place</span></p></td>
<td width="50%" data-valign="top"
style="background: transparent; border-top: none; border-bottom: 1px solid #000000; border-left: 1px solid #000000; border-right: 1px solid #000000; padding-top: 0in; padding-bottom: 0.04in; padding-left: 0.04in; padding-right: 0.04in"><p><br />
</p></td>
</tr>
</tbody>
</table>
</div>
  
  

➡️***Building your node***

**»** **Solder battery clip wires to TP4056 battery charger**

<p align="center">
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_124f131bce09ed03.png"
id="Image3" data-align="left" data-hspace="4" data-vspace="8"
width="264" height="182" />
</p> 
  
*The battery clip and wires*

<p align="center">
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_3ecf752bcf3fa19f.png"
id="Image1" data-align="left" data-hspace="4" data-vspace="8"
width="258" height="184" />
</p>
  
  

*The TP4056 battery charger*

<p align="center">
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_df1d0d4672d2396b.png"
id="Image2" data-align="left" data-hspace="4" data-vspace="8"
width="365" height="172" />
</p>
  
  

*The soldering iron*

The red wire from the battery will connect to the B+ soldering hole and
the black wire will connect to the B- solder hole.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_1b80def5d0b87da4.png"
id="Image9" data-align="left" data-hspace="4" data-vspace="8"
width="572" height="351" />  
  
  

The red wire from the battery will connect to the B+ through hole and
the black wire will connect to the B- through hole.

Clip the excess wire off the ends. <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_7f684cea5f2915c8.png"
id="Image10" data-align="left" data-hspace="4" data-vspace="8"
width="356" height="331" />  

  
  

**»** **Solder 20-gauge wire to TP4056 input**

*T <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_b3d33b1366be7251.png"
id="Image12" data-align="left" data-hspace="4" data-vspace="8"
width="665" height="300" />  
he 20-gauge wire* <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_7781da4c7ec89694.png"
id="Image11" data-align="left" data-hspace="4" data-vspace="8"
width="272" height="188" />  

The red wire will be in the through hole next to the +, and the black
wire will be in the through hole on the other side of the USB
connection. Clip off excess wire. <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_f014fc889567de2a.png"
id="Image13" data-align="left" data-hspace="4" data-vspace="8"
width="359" height="231" />  
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_3e48b0730144f844.png"
id="Image15" data-align="left" data-hspace="4" data-vspace="8"
width="284" height="165" />  

**» Solder skinny wire to TP4056 output**

*The skinny wire* <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_1e907368e9eb52d5.png"
id="Image35" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="238" />  

The red skinny wire will be connected to the OUT+ through hole and the
black skinny wire will be connected to the OUT- through hole. <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_1ecbca5a2dcad632.png"
id="Image42" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="266" />  

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_cb843b5a7a0e4a6b.png"
id="Image43" data-align="left" data-hspace="4" data-vspace="8"
width="342" height="203" />  
  
  

**» Cover the TP4056 with electrical tape and heat shrink**

*Why? Heat shrink and electrical tape will help protect your soldered
connections.*

  
  

Use electrical tape to cover all of the soldered joints.

Then wrap the 1/2inch diameter heat shrink tubing around the TP4056.
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_b550ea071f293d2.png"
id="Image44" data-align="left" data-hspace="4" data-vspace="8"
width="335" height="149" />  

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_29362632c795cd6a.png"
id="Image45" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="182" />  
  
  

*In this picture there is a hole for the troubleshooting lights on the
TP4056 to shine through. While this may make troubleshooting easier,
it's not necessarily recommended, especially if you are installing this
node outside.*

**» Heat the heat shrink**

Using the heat gun or hair dryer, heat the heat shrink until the it
molds around the TP4056.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_c7d6e7c22cbd8735.png"
id="Image46" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="217" />  
  
  

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_5df075cd203f1197.png"
id="Image47" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="175" />  
  
  

Electrical tape around the edges since the heat shrink might not fully
mold around the ends.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_4a2e7750b14e9b4b.png"
id="Image48" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="227" />  
  
  

**» Solder the voltage regulator components**

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_bf9ceab908b4cd96.png"
id="graphics9" data-align="left" data-hspace="4" data-vspace="8"
width="455" height="262" />  
Arrange your breadboard or perfboard with the connected holes in a
vertical orientation. You will end up using five rows and three columns,
as marked below.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_b8e0ca81943a9720.png"
id="graphics10" data-align="left" data-hspace="4" data-vspace="8"
width="503" height="489" />  
  
  

Insert the ceramic capacitor with the numbers facing down into row 1.
The left leg will be column 1 and the right in column 3.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_c1deebb92cacd335.png"
id="Image50" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="329" />  
  
  

Insert the electrolytic capacitor into row 2. One leg is longer than the
other. The short leg goes in column 1 and the long leg into column 3.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_d73a78250eee4d6a.png"
id="Image51" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="327" />  
  
  

  
  

The LDO will be inserted into row 3 with the flat side facing down. The
legs will go into columns 1, 2 and 3.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_19085eee1eb0b001.png"
id="Image52" data-align="left" data-hspace="4" data-vspace="8"
width="250" height="220" />  
  
  

This is what your perfboard will look like from the bottom.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_9e823d06e03da20d.png"
id="graphics11" data-align="left" data-hspace="4" data-vspace="8"
width="275" height="214" />  
  
  

After you solder all of the through holes, clip the extra wire. <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_557f0c02234ff7c7.png"
id="Image56" data-align="left" data-hspace="4" data-vspace="8"
width="262" height="250" />  

**» Solder the rest of the components to the perfboard**

Solder the skinny wires from the TP4056 to row 4. The black wire goes
into column 1 and the red wire into column 2.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_fc24ce53cee52b03.png"
id="Image55" data-align="left" data-hspace="4" data-vspace="8"
width="307" height="290" />  
  
  

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_695aa56be0c386b.png"
id="Image57" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="265" />  
  
  

  
  

Solder the SH1.25 connector wires to row 5. The black wire will go i
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_5ad74272d9781ce3.png"
id="Image58" data-align="left" data-hspace="4" data-vspace="8"
width="281" height="295" />  
nto column 1 and the red wire will go into column 3.

*A side view of the completed assembly* <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_e13ede92588467a5.png"
id="Image60" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="201" />  
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_3177c4869128bef8.png"
id="Image59" data-align="left" data-hspace="4" data-vspace="8"
width="260" height="187" />  

  
  

  
  

  
  

**» Alternate mounting option**

*If you plan to leave this outside, or just want a compact way to carry
the components around, you will need to enclose the node in something
waterproof. However, if you know you will only be using the node inside,
you may wish to forgo the waterproof enclosure and mount all of the
components to the rear of the solar panel.*

*If you choose to go this route, you can skip through the steps that
pertain to the outdoor enclosure. Pick back up at the step called
**“Solder the power cable to the barrel connector”.***

*Remember, if you have access to a roof or tall outdoor space, this will
give your node the best range!*

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_a9a8cdd51d70de6.png"
id="graphics12" data-align="left" data-hspace="4" data-vspace="8"
width="365" height="555" />  
  
  

**» Drill a hole for the power cable in the weatherproof enclosure**

*There will be an unavoidable small hole in your weatherproof enclosure
for the power line. Placing the hole on the bottom will hopefully keep
rain from dripping into the hole and then the electronics. We will also
be adding a weep hole to allow any water that does get in to leak out.*

*Depending on what your enclosure looks like you may want to change the
placement of the holes.*

  
  

Drill a small hole in the enclosure for the power wire. This should be
around 1/4”.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_fb48f416c0c0fe68.png"
id="Image62" data-align="left" data-hspace="4" data-vspace="8"
width="331" height="261" />  
  
  

  
  

**» Drill a hole for the antenna in the enclosure**

*If you are using an ammunition box as your enclosure, the best place
for the antenna hole will be on the lid close to the hinge.*

*You can also place your antenna inside of the enclosure, but it is
weatherproof and mounting it outside may give you more range.*

Use a 1/4” drill b <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_2b66124f671993fa.png"
id="Image63" data-align="left" data-hspace="4" data-vspace="8"
width="320" height="239" />  
it and drill a hole for the antenna.

  
  

**» Drill a weep hole in the bottom of the enclosure**

Drill a small 1/8” hole in the bottom of the enclosure to serve as a
weep hole. Place it on the opposite side of the enclosure than the power
cable hole. This will allow any water that gets in to the enclosure to
leak out.

  
  

  
  

**» Run the power cable through the bottom**

Run the thick power wire through the 1/4” hole at the bottom of the
enclosure.

After doing so, use this glue to seal the hole and cover it in duct
tape. <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_d9ea8e800131c1a0.png"
id="Image64" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="286" />  
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_acf5c1e6780312fc.png"
id="Image83" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="271" />  

**» Solder the power cable to the barrel connector**

Before you solder, slip the thinner heat shrink around one red cable,
one black cable, and then slip the thicker heat shrink around one pair
of wires. This will mean each connection is protected <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_e7b6b7c91872ec8e.png"
id="Image66" data-align="left" data-hspace="4" data-vspace="8"
width="370" height="263" />  
by it's own heat shrink but also by the larger heat shrink around it!

  
  

Solder the power wire to barrel connector. Match up the red wire and the
black wires!

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_7a13ab8e40496c3a.png"
id="Image67" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="191" />  
  
  

**» Heat shrink the power cable**

Use a heat gun or hair dryer to shrink the heat shrink to the wires.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_778da89443eeab4e.png"
id="Image69" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="245" />  
  
  

  
  

**» Solder the SH1.25 port to the LoRa32**

To power your LoRa32 at 3.3V (instead of 5V via the USB-C port), you’ll
need to solder wires to the pin holes labeled
<span style="font-weight: normal">3V3</span> and
<span style="font-weight: normal">GND</span>. Connect the red wire on an
SH1.25 connector to 3V3 and the black wire to GND.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_fec1210752927ccc.png"
id="image48.png" data-align="bottom" data-hspace="2" data-vspace="2"
data-border="2" width="258" height="209" />

  
  

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_84c430aff46974c4.png"
id="Image70" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="253" />  
  
  

  
  

**» Arrange the components within the enclosure**

Choose a location in your enclosure for your LoRa32. Find a cable tie
base, remove the paper from the back, and press it down where you want
the LoRa32 to go.

Secure the board with a cable tie and trim off the end.

Use a cable tie an <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_219a697203859deb.png"
id="Image72" data-align="left" data-hspace="4" data-vspace="8"
width="253" height="230" />  
d base to attach your voltage regulator board.

Thread the antenna through the hole in the top of the enclosure and use
the bottom nut to secure it. If you have a washer with a large surface
area you can also seal the washer in place with glue.

Connect the antenna cable to the LoRa32 in the spot where the green
square is in the previous picture. <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_e0e2590a0c8e03ba.png"
id="Image79" data-align="left" data-hspace="4" data-vspace="8"
width="290" height="258" />  

Use a cable tie and base to attach your voltage regulator board

Attach the <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_7b1bfdd6a0d12667.png"
id="Image73" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="242" />  
TP4056 the same way.

Use a command strip to attach the b <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_9fd409a0553798c5.png"
id="Image75" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="257" />  
attery clip. <img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_11759bf16a4b070d.png"
id="Image74" data-align="left" data-hspace="4" data-vspace="8"
width="362" height="246" />  

**» Connect power**

Insert the battery into the clip (make sure the + side on the battery
matches the + side on the clip!).

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_5f6138d474aebc41.png"
id="graphics15" data-align="left" data-hspace="4" data-vspace="8"
width="508" height="340" />  
Connect the barrel plug to the barrel plug end on the solar panel.

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_4b45a681d4225366.png"
id="Image80" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="245" />  
  
  

**» Your node should power on!**

<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_355af7e03be6ef99.png"
id="Image81" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="289" />  
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_1102fa556400218e.png"
id="Image82" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="259" />  
<img
src="images/Zine%20Let&#39;s%20Make%20a%20Solar-Powered%20Chat%20Network%20v5_htm_fc73fe8656079d5.png"
id="Image85" data-align="left" data-hspace="4" data-vspace="8"
width="438" height="255" />  
  
  

  
  
