# Public Key Encryption

The methods so far all have a basic weakness: the encryption method or key needs to be kept secret. But keeping the key private is almost as hard as keeping the message private. In 1976 Ron Rivest, Adi Shamir, and Len Adleman devised an ingenious method \(now known as RSA\) that allows a person to announce publicly how anyone can encode a message to him so that only he is able to decipher it. The information, which is given away to everybody, is called the _public key_. The information which is needed for deciphering \(the _private key_\) is known only by the person for whom the message is intended. If Bob wants to send Alice a secret message, he enciphers it with Alice's public key. Then no one else can decipher it, even knowing her public key. Only her private key can undo the encryption, and you can't figure out the private key from the public key.

If your connection blocks YouTube, [watch the video here](http://scratch.mit.edu/discuss/youtube/YEBfamv-_do), but start it at 2:25. [https://youtu.be/YEBfamv-\_do](https://youtu.be/YEBfamv-_do)

#### For You To Do

1. It may seem incredible that Alice can make her encryption key public and still no one except her can decrypt her message. The public key method relies on some mathematics and on some limitations on the speed of current computers. Read "Secrecy Changes Forever" \([Blown to Bits pages 178-181](http://www.bitsbook.com/wp-content/uploads/2008/12/B2B_3.pdf#page=196)\) to understand some of how this works.

Here is a model of public key encryption \(from [wikimedia.org](https://commons.wikimedia.org/wiki/File:Public_key_encryption.svg)\)

![](https://bjc.edc.org/bjc-r/img/3-lists/525px-Public_key_encryption.png "Diagram of public key encryption")

#### For You To Do

1. With a partner, discuss how this method is different from symmetric cryptography described on previous pages. Would you trust this method to work to send a credit card number?

#### If There Is Time...

It's also possible to use the private key for encryption and the public key for decryption. That's no good for secret messages \(why not?\), but it's useful for _**digital signatures**_. I use my private key to encrypt a message; you use my public key to decrypt it. If you get a meaningful message as the result, that proves that the message was encrypted with my private key. \(If I want both secrecy and digital signing, I encrypt the message with my private key to sign it, then encrypt the encrypted result \_again \_with your public key to keep it secret. You decrypt it twice, first with your private key and then with my public key.\) This is a nice example of \_composition of functions: \_the output from the first encryption is the input to the second encryption.

### Secure HTTP

Secure HTTP connections \(those that use **https://**instead of **http://**\) use a protocol called _Transport Layer Security_\(TLS\) or maybe an older version called _Secure Sockets Layer_\(SSL\). Both are based on public key cryptography. With SSL/TLS, the site you are visiting sends its public key, and your browser uses it to encrypt the information you send.

If your connection blocks YouTube, [watch the video here](http://scratch.mit.edu/discuss/youtube/kBXQZMmiA4s), but start it at 4:40.

![](https://bjc.edc.org/bjc-r/img/icons/headphones-mini.png "Set Up Your Headphones or Speakers")[https://youtu.be/kBXQZMmiA4s](https://youtu.be/kBXQZMmiA4s)

#### **Open Standards Help Security**

In order to work properly, a cryptographic function has to be easy for the private key holder to invert, but hard for anyone else to invert. How do we know what "hard" means? For example, current cryptographic methods rely on the difficulty of finding prime factors of very large numbers. There's no proof that someone won't come up with a fast way to do that, but people are pretty confident about it because the problem has been well studied by many mathematicians. \(On the other hand, when quantum computers become practical, factorization will be easy, and new cryptographic methods will be needed.\)

What makes it possible for mathematicians to study the difficulty of breaking Internet cryptography is that the method used—the cryptographic function—is openly published. This may seem strange; if you want to keep secrets, shouldn't you keep the technique secret, too? But secret algorithms can have weaknesses that go undiscovered until some bad guy exploits them. Open standards allow an algorithm to be studied before it is used in practice.

### Certificate Authorities

Public key cryptography doesn't solve all the problems, because someone might publish a fake public key pretending to be someone \(say, Alice\). Then someone might accidentally encrypt their message for Alice using the faker's key, and then the faker can read the message. In practice, this is partly fixed by relying on trusted third parties, called Certificate Authorities, to _issue public keys_. In your browser's security options you can see all of the Certificate Authorities that it trusts.

#### Take It Further

1. Read "The Key Agreement Protocol" and "Public Keys for Private Messages" \([Blown to Bits pages 181-183](http://www.bitsbook.com/wp-content/uploads/2008/12/B2B_3.pdf#page=199)\) for more details on Public Key Encryption.



