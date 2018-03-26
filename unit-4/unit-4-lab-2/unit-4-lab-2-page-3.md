# A Hierarchy of Open Protocols

There are billions of devices connected to the Internet, and hundreds of different kinds of devices: laptops, tablets, phones, refrigerators, handheld credit card readers, and so on. How do they all know how to find and talk to each other?**Protocols**\(standards\) ensure that the variety of devices interact with each other smoothly.

There are a lot of protocols! The Internet was designed with several layers of abstraction that sort the protocols according to what part of the process they support.

## Internet Abstraction Hierarchy

This hierarchy of abstractions manages the complexity of the Internet by hiding the details of lower levels of the system. The highest level of abstraction includes the most general features of the Internet that have to work the same across all devices. At lowers levels of abstraction, things get more device-specific.

* **Application Layer Protocols **are the highest level of abstraction because they manage how data is interpreted and displayed to users. These protocols give meaning to the bits sent by lower-level protocols; user and server computers must agree on what the bits mean, and application protocols \(like HTTP\) offer this. Application Layer Examples: browsers use [HTTP](https://bjc.edc.org/bjc-r/cur/programming/4-internet/1-reliable-communication/1-what-is-internet.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment) \(HyperText Transfer Protocol\) to interpret HTML instructions for page formatting. [DNS](https://bjc.edc.org/bjc-r/cur/programming/4-internet/1-reliable-communication/3-address-hierarchy.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment) \(Domain Name System\) converts user-friendly web addresses into IP addresses. Your email inbox may use SMTP \(Simple Mail Transfer Protocol\) to send and IMAP \(Internet Message Access Protocol\) to read email.

* **Transport Layer Protocols **manage the breakdown of a message into packets to be transmitted by lower level protocols and also the reconstruction of the message from the packets upon arrival. Transport Layer Examples: [TCP](https://bjc.edc.org/bjc-r/cur/programming/4-internet/2-communication-protocols/2-tcp.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment) \(Transmission Control Protocol\) simulates a reliable, long-term connection between two computers by only displaying data once all packets have arrived. When speed is more important than accuracy, people use UDP \(User Datagram Protocol\), such as for real-time video streaming, where one missed packet doesn't matter much.[![](https://bjc.edc.org/bjc-r/img/4-internet/IP-suite.png "The Internet protocol suite")](https://en.wikipedia.org/wiki/Internet_protocol_suite)

* **Internet Layer Protocols **manage the pathways that the data packets travel across networks. These protocols treat the Internet like one large network even though the physical reality on the lower level is one of many tiny subnetworks. Internet Layer Examples: Every device on the Internet needs an IP address so other devices can find it. [IP](https://bjc.edc.org/bjc-r/cur/programming/4-internet/2-communication-protocols/1-ip.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment) \(Internet Protocol\) addresses are upgrading from IPv4 to IPv6. Routers use Internet layer protocols to detect and work around network congestion.

* **Network Interface Hardware **\(Link Layer\): All Internet devices connect through a physical interface that uses a protocol to manage the connection to the local network. These local protocols are the least abstract because they deal directly with your physical hardware. Link Layer Examples: You may connect with an Ethernet cable perhaps a WiFi radio antenna inside the case. Both connects computers to a local network router which then connects to an Internet provider. Cell phones use a longer-range cellular connection to a phone carrier.

## Open Protocols

These are all **open standards **meaning that anyone can look up a protocol and code with it to make new hardware or software without any permission. The Internet is probably the largest and most complicated artifact in human history, and it relies on **cooperation! **Despite some governments' attempts to censor the net, the big picture is one of strong cooperative spirit.

Before the Internet, there were several different network protocols that were secrets belonging to particular manufacturers. So if you had a particular brand of computer or router, it could talk only to other computers of the same brand.

Just think...

1. Your T-Mobile cell phone can talk to your friend's Verizon phone.
2. You can send email to someone in a country that's considered an enemy of your country \(from the US to Iran, for example\).
3. An engineer at Microsoft can read a web page at Apple even though their companies are competitors.

#### For You To Do

1. Make sure you understand these important Internet protocols: ![](/assets/talk_with_partner.png)

   1. [**HTTP**](https://bjc.edc.org/bjc-r/cur/programming/4-internet/1-reliable-communication/1-what-is-internet.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment): HyperText Transfer Protocol—the protocol that your browser uses to _access an HTML webpage_

   2. [**DNS**](https://bjc.edc.org/bjc-r/cur/programming/4-internet/1-reliable-communication/3-address-hierarchy.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment): Domain Name System—the hierarchical addressing protocol that is _human-readable_

   3. [**TCP**](https://bjc.edc.org/bjc-r/cur/programming/4-internet/2-communication-protocols/2-tcp.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment): Transmission Control Protocol—the protocol that \_assures reliable transmission \_of data

   4. [**IP**](https://bjc.edc.org/bjc-r/cur/programming/4-internet/2-communication-protocols/1-ip.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment): Internet Protocol - the hierarchical addressing protocol that manages routing of data between computers; we are upgrading from IPv4 to IPv6 for more addresses.

2. Read [Blown to Bits pages 309-312](http://www.bitsbook.com/wp-content/uploads/2008/12/B2B_3.pdf#page=327).



