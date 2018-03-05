# Address Hierarchy

There are two **hierarchical **addressing systems on the Internet: domain names and IP addresses. People use **domain names **\(like _snap.berkeley.edu_\) to visit websites. Computers translate those domain names to **IP addresses**\(like _128.32.189.18_\) to locate and send data behind the scenes.

A _hierarchy _is an arrangement of things with the broadest or highest category at the top and things ranked into subcategories below. A hierarchy is often depicted as a pyramid.

For example, organizations often use a hierarchical personnel structure with the most powerful people at the top managing people who manage people below them, who manage people below them, and so on. In biology, we use a [taxonomic hierarchy](https://en.wikipedia.org/wiki/Taxonomic_rank): kingdom, phylum, class, order, family, genus, species. And on computers, we store files in a hierarchy of folders within folders.

Before the Internet, there were only small networks of computers \(like the Arpanet which peaked at around 200 computers\), and every computer knew the name of all the other computers on the network. That worked for small networks, but it's not realistic for the 3 billion computers on the Internet now. So now, a hierarchy allows the system to distribute requests for IP addresses to domain name servers across the growing network.

## Domain Name Hierarchy

Recall the structure of a [URL](https://bjc.edc.org/bjc-r/cur/programming/4-internet/1-reliable-communication/1-what-is-internet.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment):![](https://bjc.edc.org/bjc-r/img/4-internet/URL-structure.jpg "parts of a URL")

Just as the path in a URL locates a specific file in a hierarchy of folders on the server,domain names locate a specific website within a hierarchical **domain name system **\(DNS\). The hierarchy of the domain name system simplifies the process of finding the computer with the desired domain name because the DNS servers that help locate domains don't need enormous lists with every host name in the world. Instead, any user's computer only has to know where to find a **root domain **server \(the one that knows where to find the top-level domains such as _.org _and _.edu_\), and _that _server knows where to find the domain \(like berkeley.edu\), and that server knows where its subdomains are \(like snap.berkeley.edu\), and so on.

The root domain may be a country code \(such as _.mx _for Mexico\) or a category code \(like _.gov _for government\). The last two segments of a domain name \(like _berkeley.edu_\) make up the **primary domain**, the main address for a site. **Subdomains **are subsections of primary domains or of other subdomains. For example:

* [**snap**.berkeley.edu](http://snap.berkeley.edu/)
* [**store.parks**.ca.gov](http://store.parks.ca.gov/)

![](https://bjc.edc.org/bjc-r/img/4-internet/hierarchy.jpg "domain name hierarchy")

Question 1

* Which of the following could be a subdomain of the domain _bicycles.com?_
  * about.bicycles.com
  * bicycles.org
  * bicycles.co.uk
  * bicycles.com.org

## IP Address Hierarchy

When we type in a domain name, the browser queries the domain name system to find the**Internet Protocol \(IP\) address**of the server we want to visit. IP addresses are unique numerical addresses assigned to every device on the Internet. Both the domain name syntax and IP addresses are hierarchical; however unlike domain names, IP addresses are hierarchical from right to left \(see right\).

[https://youtu.be/5o8CwafCxnU](https://youtu.be/5o8CwafCxnU)

**What's an undecillion?** One undecillion is 10^36,a billion billion billion billion, a 1 with 36 zeroes after it, 10^9 \* 10^9 \* 10^9 \* 10^9.

#### For You To Do

1. Write an explanation of the DNS and IP address hierarchy.

  




