---
layout: post
title:  "Cryptography and Other Techs"
date:   2015-11-26
categories: privacy
---


## I

People may tend to believe that the world of cryptography and other security-enhancing technologies is an labyrinth of dark arts and complications. I have to say that I am among them, or seemingly so. I believe that there has to be some kind of very basic and clear guiding principles behind all of these mess, as with every complicated system/human mindset/etc, and even the most advanced encryption methods are merely application of these princeples. 

Cryptography is one of the most important building block in this realm. Its main aim is to prevent the others from understanding what you say. The earliest form of encryption, shift cipher, is basically used from Julius Caesar to WWII. With longer and more dynamic keys, the Enigma Machine that German used in WWII can be seen as an ultimate form of classic cryptography.

In the end, even the formidable Enigma is beaten by the most genius of minds, such as Marian Rejewski and Alan Turing. Then came the idea of Public Key:

1. If Alice encrypted message M with Bob's public key, then only the Bob can decrypt this message (Encryption);
2. The above procedure are vulnerable to Man-in-the-middle attack: Bob need to ensure the message is indeed from Alice herself. That is, Alice encrypt M with her own private key, and only her public key can be used to decrypt it. (Signature)

The next problem is how to make sure 1) the public key of Alice is indeed matched to herself and 2) everybody know everybody's public key. There are two main solutions:
1. Centralized: Public Key Infrastructure (PKI), a set of system to do the related managing work. Within this system a certificate authority (CA) will issue your public key a certificate: "Yes, this is indeed Alice herself, here is her detail..."

2. Distributed: Web of Trust. A chapter of Cory Doctorow's Novel [Little Brother](http://craphound.com/category/littlebrother/) shows this idea vividly: to form a trustworthy web under the nose of surveillance-maniac government, the protagonist throw a party and call friends he trust. Then in the party he present a key-pair-generator. Everyone one step in front of this machine, get his random key-pair, take a photo of his own private key, destroy this page, and show his public key to every one he/she is willing to trust. 

## II
I'd like to check briefly how it is used in [setting up and OpenVPN server](https://www.digitalocean.com/community/tutorials/how-to-set-up-an-openvpn-server-on-ubuntu-14-04). Here the server itself is treated as a CA, with its own details like name, mail, address, etc. Then a file `ca.crt` to indicate "Yes it's me". Then it generate certified public key `server.crt` and private key `server.key`. Then it can generate public key pairs for each client. It means the server itself is also a PKI, Seems plain enough.

We should note that a pair of Diffie-Hellman parameters are also required in setting up OpenVPN. This pair of parameters is public, and for some [dark math magic](https://www.wikiwand.com/en/Diffie%E2%80%93Hellman_key_exchange), they will let two people get the same key separately through open information exchange. It is the basis of [Perfect Forward Secrecy](https://security.stackexchange.com/questions/65802/ecdsa-ciphers-and-forward-secrecy-question-about-key-exchange/65808#65808). So: [DH](http://us.battle.net/wow/en/game/class/demon-hunter) is for encryption, RSA is for signature (RSA maybe too expensive for encrypt normal communication continuously).  

My questions are:
1. Where is CA's private key? Is the server's key always CA's key?
2. Is it always the case that CA is responsible for generating key pairs? That would be terrible.

## III

Cryptography is not the only way we can choose to hide information. One other choice is **Stegenography**: hide a tree in the forest. Another choice is **Authentication**: make a fortress around my secret, and only the people who I permit can enter. Password and PIN are some widely-used example of authentication. One interesting topic here is *Biometrics*. However, there is never a 100% perfect method. Again, the technology is not the key to privacy or security; human is.