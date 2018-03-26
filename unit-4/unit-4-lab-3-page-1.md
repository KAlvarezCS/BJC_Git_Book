# Cryptography

#### For You To Do

1. Write a secret message to send to a partner. Invent some way of encoding the message. Then send the encode message to your partner. 
2. Your partner will send you an encoded message. When you get it, try to decode it. What strategies are you using to decode it?
3. With another pair of students, compare the methods you used to encode your messages. Was anyone able to decode their message? How?

![](/assets/talk_with_partner.png)

Cryptography is the study of how to convert messages into code \(encryption\) and how to solve codes \(decryption\). Just as TCP enables reliable transmission over an unreliable network, cryptography enables verifiable, secure transmission over an insecure network. [https://youtu.be/ZghMPWGXexs](https://youtu.be/ZghMPWGXexs)

[**Symmetric cryptography**](https://bjc.edc.org/bjc-r/cur/programming/4-internet/3-cybersecurity/2-symmetric_cryptography.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment), uses the same secret key to encode and to decode a message. Symmetric cryptography has been around for thousands of years. The trouble with symmetric cryptography is: how can we keep the key secret?

[**Public key \(asymmetric\) cryptography**](https://bjc.edc.org/bjc-r/cur/programming/4-internet/3-cybersecurity/4-asymmetric_cryptography.html?topic=nyc_bjc%2F4-internet.topic&course=bjc4nyc.html&novideo&noassignment) was created by mathematicians in the 1970s. It uses two different keys for encryption and decryption, so sharing the public encryption key doesn't give away the private decryption key.

Banks use public key cryptography. When users enter their password on a bank's web site, the user's browser uses the bank's public key to encrypt the password before sending it over the Internet. Only the bank can decrypt that password, using their private key.

