# Addresses in a Network of Networks: IP

#### The Internet isn't just a network of computers. It's a _network of networks_. The connection points are called **routers**, networking devices that route traffic between subnetworks on the Internet. How do the routers know where to find the computer you want? Every device on the Internet has a unique **Internet Protocol \(IP\) address**\(or more than one, if it's a router\), like a postal or email address. The Internet Protocol specifies how a router handles a request for another IP address.[![](https://bjc.edc.org/bjc-r/img/4-internet/network-of-networks.jpg "Graph of Internet from UC San Diego Jacobs School of Engineering")](http://jacobsschool.ucsd.edu/news/news_releases/release.sfe?id=685)For You To Do

1. Why does the graph of the Internet look like a tangle in the middle with fireworks on the outsides?
2. Discuss how this shape is related to how people connect to the Internet \(though an Internet Service Provider, etc.\). Write out a brief description and/or explain it to someone else.![](/assets/talk_with_partner.png)
3. Visit [http://bot.whatismyipaddress.com/](http://bot.whatismyipaddress.com/) for your current IP address.
4. Visit [http://ipinfo.io/](http://ipinfo.io/). What information does that page give you?

The amount of detailed information available from an IP address is pretty amazing \(and a little scary\), especially when you think about the ways that information can be used.

![](https://bjc.edc.org/bjc-r/img/4-internet/ipinfo-screenshot.png "Screen shot of http://ipinfo.io/72.229.28.185")Some of the information might have slight inaccuracies. IP addresses often give the location of an Internet service provider, usually from a nearby location.

## IPv4

Each of the four numbers in a typical IP address today is an eight-bit **byte **with a value between 0 and 255 \(see right\). A 32-bit IPv4 \(the "v" stands for "version"\) address is big enough to support 2^32 computers. That's about four billion \(4 · 109\), but there are more than _seven _billion people on Earth, so there aren't enough IP addresses to go around.

**Why does IPv4 support 2 32 computers? **There are 32 bits in an IPv4 address \(see right\), and each bit can be one of two possible values \(0 or 1\). So, there are 2 32 possibilities with thirty-two bits. 

![](https://bjc.edc.org/bjc-r/img/4-internet/ipv4.png "IPv4")

## IPv6

The long-term solution is to increase the length of an IP address. The new IP addresses are 128 bits wide, which is enough to support 2^128\(about 1038\) computers.

![](https://bjc.edc.org/bjc-r/img/4-internet/ipv6.png "IPv6")

#### For You To Do

1. ![](/assets/twoPeopleThinking.png)Is your address in IPv4 of IPv6?

#### If There Is Time...

1. Read [_Blown to Bits_pages 301-306](http://www.bitsbook.com/wp-content/uploads/2008/12/B2B_3.pdf#page=319).

#### Take It Further

Most likely, the router in your home or school uses a protocol that allows all the computers on the local network \(such as in one building\) to share a single IP address on the Internet, which can be cheaper. The router that creates the local network gives each computer a _local address_. For example, although the outside world may think someone's computer has IP address 108.26.181.226, that computer itself might think its address is 192.168.1.11.

* Look up your current local IP address in your system preferences or settings. It's usually under network or internet settings and may be listed with the computer device supporting that connection \(wifi, ethernet, wifi, bluetooth, etc.\).
* The 192.168 _domain _\(the block of IP addresses that all start with 192.168\) is reserved for _local _networks, but no computer on the Internet has an address in that range. Another such domain is 10.0.[ ](http://creativecommons.org/licenses/by-nc-sa/4.0/) 

  




