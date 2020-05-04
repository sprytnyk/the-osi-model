
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://github.com/vald-phoenix/the-osi-model/blob/master/LICENSE)
# The OSI model compedium

Table of contents:

- [What is the OSI model?](#what-is-the-osi-model)
- [Main terminology](#main-terminology)
- [OSI model layers](#osi-model-layers)
  * [Table](#table)
  * [Layers in details](#layers-in-details)
  * [Acronyms](#acronyms)
- [Credits](#credits)

## What is the OSI model?
**The OSI Model (Open Systems Interconnection)** is a standardised Reference 
Framework for conceptualising data communications between network.

## Main terminology

**Encapsulation** is preparing & passing the data by any upper layer to the 
Lower layer. That basically means, going from the application layer all the way
down to the physical layer.

**Decapsulation**  is vice-versa encapsulation. This decoding data while going
Upwards from the physical layer till the application layer.

**L7-L5** are called Upper layers or Host layers. They usually work with an
application and not with hardware itself.

**L4-L1** are called Lower layers or Media layers. They usually work with the
hardware.

When data unit is traversing from **L7** to **L1** every unit wraps by a
header, puts on the top of a unit. So when it reaches to **L1** this will look
like this:  
[Bits]  
[Frames]  
[Packets]  
[Segments]  
[Data]  

<div align="center">
<img src="https://upload.wikimedia.org/wikipedia/commons/9/90/Wireshark_3.0.3_screenshot.png">
<p><strong>Figure 1:</strong> Wireshark example of headers.</p>
</div>

The reverse happens when data units go from **L1** to **L7**. Each layer it 
strips headers.

## OSI model layers

### Table

|Level|OSI model layer|Data Unit|Devices|Protocols|
|--|--|--|--|--|
|7|Application|Data|L7 firewall|HTTP, DNS, DHCP, FTP, Telnet, SSH, SMTP, POP, IMAP, NTP, SNMMP, TLS/SSL, GBP, RIP, SIP, etc.|
|6|Presentation|Data|L7 firewall|All the above|
|5|Session|Data|L7 firewall|All the above|
|4|Transport|Segments|L4 firewall|TCP (connection oriented), UDP (connectionless oriented)|
|3|Network|Packets|Router, Multiplayer Switch, Router|IPv4, IPv6, IPSec, OSPF, EIGRP|
|2|Data Link|Frames|Switch, Bridge, NIC, Wireless Access Point|MAC, ARP Ethernet 802.3 (Wired), CDP, LLDP, HDLC, PPP, DSL, L2TP, Ethernet 802.11 (Wireless), SONET/SDH|
|1|Physical|Bits|All the above|Electrical signal (copper wire), Light signal (optical fibre), Radio signal (air)|

### Layers in details

...

### Acronyms

All People Seem To Need Data Processing (L7-L1).  
Please Do Not Throw Sausage Pizza Away (L1-L7).

## Credits

- [Network Fundamentals](https://drive.google.com/file/d/1i1KT_mE-pfsasubSGWZST91XLDGwEfMU/view)
- [OSI Model – Cheatsheet (ATech)](http://aurumme.com/atech/wp-content/uploads/2018/04/OSI-Model-CheatSheet-ATech-Waqas-Karim.pdf)
- [OSI Model Explained](https://youtu.be/vv4y_uOneC0)
