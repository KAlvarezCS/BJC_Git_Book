# Reliable Transmissions on Unreliable Networks: TCP

When you send a message over the Internet, your computer divides it into small chunks called **packets **that it sends individually, each on its own path. A packet can include any kind of data: text, numbers, lists, etc. Computers, servers, and routers are fairly reliable, but every once in a while a packet will be lost, and devices on the Internet need to tolerate these faults.

The **Transmission Control Protocol**\(TCP\) guarantees reliable transmission by breaking messages into packets, keeping track of which packets have been received successfully, resending any that have been lost, and specifying the order for reassembling the data on the other end. This process is what makes the Internet a **packet switching **network.

[https://youtu.be/AYdF7b3nMto](https://youtu.be/AYdF7b3nMto)

* The **computers \(including servers\) at the two endpoints **\_of a communication run the **Transmission Control Protocol **\(TCP\) that divides up the packets and guarantees reliable transmission.

* The **routers at every connection-point **on the Internet run the **Internet Protocol **\(IP\) that transmits packets from one IP address to another \(not caring that sometimes a packet will be lost and not knowing anything about the purpose or meaning of a packet\).

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/4-internet/U4L3-TCP.xml#present) It provides a simulation of unreliable data transmission by Internet Protocol.
   1. **Click the green flag** to initialize the incoming transmission variable before each experiment.
   2. **Click either character** to enter a message for it to send to the other one. [![](https://bjc.edc.org/bjc-r/img/4-internet/TCP.png "picture of TCP project stage")](http://snap.berkeley.edu/snapsource/snap.html#open:https://bjc.edc.org/bjc-r/prog/4-internet/U4L3-TCP.xml)
2. ![](/assets/talk_with_partner.png)Compare the result with what you sent. What problems do you see?

TCP works by including additional information along with each packet so that the receiving computer can keep track of how many packets it has received, re-request any missing packets, and reorder the packets to reconstruct the original message. In this simulation, a packet either arrives correctly \(even if it's out of order\) or it doesn't arrive at all. But on the Internet, it's possible for a packet to arrive with erroneous data, so the real TCP has to check for errors and request re-transmission of packets with errors too.

#### If There Is Time...

1. Read [Blown to Bits pages 306-309](http://www.bitsbook.com/wp-content/uploads/2008/12/B2B_3.pdf#page=324).

#### Take It Further

1. Build a simple TCP. Resolve the unreliability so that messages are received reliably despite the limitations of IP packets. **You'll need to change **the definitions of:

   1. ![](https://bjc.edc.org/bjc-r/img/4-internet/internet-transmit.png "internet transmit \(\) to \(\)")
   2. ![](https://bjc.edc.org/bjc-r/img/4-internet/read-internet-data.png "read internet data with \(\)")

**Do **_**not **_**change **the definition of ![](https://bjc.edc.org/bjc-r/img/4-internet/send-IP.png "send IP packet \(\) to \(sprite\)"). That block simulates the unreliable network. You could "solve" the problem by rewriting this block to simulate a perfect network instead of an imperfect one, but that misses the point.

To solve this problem, you'll need a way to keep track of the order of the data and a way to re-request missing packets:

* First, solve the problem of packets arriving out of order. You can include extra header information in addition to the packet data in order to help the receiver reconstruct the message. This will require cooperation by both sender and receiver \(that is, changes to both grey blocks\).
* Then, solve the problem of packets not arriving at all. That is, make the transmission reliable even though IP is unreliable. This, too, will require changing both sender and receiver.



