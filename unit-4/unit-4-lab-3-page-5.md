# Cybersecurity

There are many cybersecurity risks on the Internet. The various kinds of cyber warfare and cyber crime can have widespread and potentially devastating effects. Accessing risks and implementing protective measures for cybersecurity issues has software, hardware, and human components.

![](https://bjc.edc.org/bjc-r/img/icons/headphones.png "Set Up Your Headphones or Speakers")

If your connection blocks YouTube, [watch the video here](http://scratch.mit.edu/discuss/youtube/AuYNXgO_f3Y).

### The Lack of DNS Security

The hierarchy of the DNS makes the system more efficient; when you visit [snap.berkeley.edu](http://snap.berkeley.edu/), your computer only has to know where to find an _edu name server. That server only has to know where to find the berkeley.edu server. And that server directs your computer to snap.berkeley.edu_.

There are millions of such DNS requests every second, and if all of those requests had to begin at the same few root domain servers, those servers would be flooded with too many requests. Instead, DNS servers remember \(cache\) the results of host name queries made to root domain servers, and they provide these non-authoritative answers for most requests. However, if the IP address of the site you are requesting changes before before the non-authoritative answer is updated, you may be sent to the wrong site. DNS was never intended to be perfectly secure.

A perfectly secure Internet could easily end up preventing anonymous publishing. To prevent fraud, it's important to be able to verify the source of a message. But if the source of a message can be verified, the message can't be anonymous. That's problematic both for privacy and for freedom of speech.

### Common Security Issues for Users

Software has _bugs_\(even finished software written by professionals\). And people can use those bugs for bad purposes \(such as crashing your computer or implanting spy software to collect everything you type, including passwords\). Software developers try to prevent security bugs and fix them when they turn up, but not every software developer distributes fixes promptly. \(And not every computer user keeps up with software updates perfectly!\)

This is especially a problem on smartphones. If you have an Android phone and a security bug is found, Google fixes it, but they don't send the fix directly to your phone. Google sends new system releases to the phone manufacturers, who may take some time to install local modifications available only on their phones. Only after that do the phone manufacturers send the modified Android code to carriers, who also may take some time to install carrier-specific modifications. Security fixes can come more quickly on iOS phones, because Apple can send updates to you directly, no matter which carrier you use.

The general name for programs that try to affect your computer badly is _malware_. One kind of malware is called a _virus_. Computer viruses make copies of themselves \(just as biological viruses do\) and try to spread themselves over the network to other computers. People use \_antivirus software to help prevent these attacks. People also use firewalls to limit the kinds of connections \(HTTP requests, incoming mail, etc.\) outsiders can make to your computer. \(Both your computer and your router probably run firewall software.\)

Another common attack strategy is called _phishing_: an attacker sends you an email that appears to be from some official organization \(such as your bank\) and tricks you into giving information to the attackers \(such as your bank password\).

### Distributed Denial of Service \(DDoS\) Attack

A _Denial of Service_\(DoS\) attack consists of sending a lot of requests to a server at the same time \(for instance, requests for a web page or some data\). This can overload the server's network bandwidth. A DoS attack doesn't destroy data or collect passwords; it just causes a temporary inability to reach the targeted server so other users of that server are denied service.

A variant is the _Distributed Denial of Service_\(DDoS\) attack, in which the attacker first uses viruses \(or similar self-spreading software\) to take control of many \(sometimes tens of thousands of\) computers around the world. This network of infected computers is called a _botnet_. The attacker then launches a DoS attack from all of the victim's computers \(called _zombie computers_\) at the same time. Besides increasing the number of simultaneous server requests, DDoS makes it harder to determine who is at fault, since the attack seems to come from many innocent people.

#### For You To Do

1. Consider the following question: Which of the following are existing vulnerabilities of the Internet, according to experts?

   1. A physical attack that involves cutting fiber-optic cables

   2. Attacking electrical systems that control the energy grid.

   3. Eroding the trust and confidence that the general public has in their online privacy and secure online transactions.

   4. All of the above



