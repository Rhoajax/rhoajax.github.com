---
layout: post
title: "A Research Survey"
description: ""
category: ""
tags: []
---
{% include JB/setup %}
## Group 1

### [The Microsoft Cloud Computing Research Centre](http://www.mccrc.eu)

Launched in April 2014. Computer Lab is one of its collaborator. Its research theme is a little bit "wired": it's about meeting challenges in cloud computing where technology and **regulation** intersect, which means that despite computer scientists, the lawyers play an important part. It addresses complex and difficult areas of vital importance to governments, businesses, and communities around the globe.
For example, the cloud computing services raise a numbers of legal ~~high~~ challenges, such as "Regional Clouds". 

### [CSaP](http://www.csap.cam.ac.uk/)

Centre for Science and Policy. It aims at providing the network and mechanisms for high-quality engagement between academics and policy professionals. 
Here quotes Jon:

>  Many of the things I work on -- both in research and education -- potentially entail important policy considerations. CSaP’s programmes, particularly the Policy Fellowships and the Policy Workshops, provide a fantastic opportunity to interact directly with the policy makers who are grappling with the relevant issues in government and industry.

So in my opinion this is a channel for researchers, policy makers and business makers to communicate.

### [Security and Privacy](http://www.cl.cam.ac.uk/research/security/posters/20131108-cam-security-research.pdf)

Cambridge has, for many years, been a centre for world-leading computer and communications security research, which spans many groups (basically *Every* group in Computer Lab).

- Operating System Security

   **Mirage** is a clean-slate OS written in *OCaml*. Implementing the OS in a type-safe, **functional language** offers security and reliability improvements through access to formal verification and immunity to many traditional vulnerabilities.
   MirageOS revisits the *library OS* concept and narrows the gap between safe high-level programming and low-level systems construction.

   The idea of the library OS is that the personality of the OS on which an application depends runs in the address space of the application. A small, fixed set of abstractions connects the library OS to the host OS kernel, offering the promise of better system security and more rapid independent evolution of OS components.

- Distributed-system Security

  - Federated secure sensor network laboratory
    Shared sensor networks; multiple application; each app can use any sensor available.
   
    For privacy: Different roles\owners\applications have different requirements. FRESNEL aims at offering a framework that supports merging of policies as specified by different roles in the system.

  - NaaS: Network-as-a-service

    An open challenge for Big Data: to balance the contention between nodes for network resources in data centers. The key idea is that tenants can customise the service that they receive from the network.

- Personal Data Privacy in the Cloud

  - User-Centric Networking

    We have uploaded too many personal data to online storage. The UCN projects aims at enhance mechanism to support privacy-preserving content recommendations and strike a balance between personal privacy and the need of the service industry.

    Specifically, the PIH software stack let the users in total control of their data. Users can decide whether or not, what kind of, and to what degree their data can be shared with specific providers.

## Group 2 -- Energy

### [INTERNET](http://www.internet-project.org.uk/)

A little bit difficult to understand. I'll come back later.

### [Energy@Cambridge](http://www.energy.cam.ac.uk/)

At least I can see that the Cambridge guys take the energy stuff seriously. Guess it is one of the cutting-edge research field. 

## Group 3

First let's meet three similar organizations: [Cambridge Networks Network](http://www.cnn.group.cam.ac.uk/about-us), [Network Excellence in Internet Science](http://www.internet-science.eu/), and [Community Organisation of Events in Communications, Mobile Computing and Networking](http://www.commnet.ac.uk/). In my opinion, they all try to provide an interdisciplinary environment to mitigate the "Research fragmentation" in specific areas: complex networks, Internet networks, and a grand vision across CS/EE/SIP. 
So we can accordingly see that productive dialogue and different perspectives are indeed taken seriously in technology development now.

So when these guys give a full discussion about the "future network", there must be something we should investigate in [the report](http://drops.dagstuhl.de/opus/volltexte/2013/4073/). Chances are that it will presents a broad vision that could not have been perceived by us IT guys alone. (Oh, it reminds me of this misleading movie name: *IP man* :)

- Social networks have to be considered, and can be combined with Communication networks
- Use cases of SDN
- Prescriptive Network Theories

## Group 4

### [Horizon Project](http://www.horizon.ac.uk)

Horizon features Ubiquitous Computing, a key engine of innovation for our future digital economy. It is specifically interested in people's *lifelone contextual digital footprint*. Horizon contains a great amount of sub-projects. I guess maybe it is (one of) the leading projects in the ubiquitous computing area. Again, interdisciplinary is a requisite part. Its ambitions also include policy influence, knowledge transfer. 

### [Public Access WiFi Service](http://publicaccesswifi.org)

The PAWS project seeks to develop technology that will enable *free* Internet connectivity to everyone whenever and wherever. Its core part is *sharing*. The user who agree to share a small fraction of his high speed bandwidth can put a PAWS box near the home router. It is shared as a VPN, which solves the security concern. Then any signed PAWS users can access the shared WiFi with their devices. Of course, they will be offered low quality services. By allowing the digitally excluded to access to public services, this project can save the government a bunch of money.

One obvious question I can perceive would be: how to incentive the bandwidth-rich users to share?

### [Global Access to the Internet for All research group](https://irtf.org/gaia)

## Group 5

### [OCaml Lab](http://www.cl.cam.ac.uk/projects/ocamllabs/index.html)

The goal of OCaml Lab is quite clear: push OCaml language, increase its applicability and popularity, create communities infrastructure, etc., just like any other language. 
The projects of this lab are more that just the language platform itself. Thy include an OS written in OCaml (MirageOS), a distributed platform application (Illuminate), a OCaml compiler (why it is not a part of the platform?), Trilogy 2 (described later), and a serious of propaganda plans.

Illuminate (not **Illuminati**) is one use case of a bundle of techniques to make distributed devices in IoT more secure, reliable and easier to program. The used technologies include: MirageOS, Signposts, and Irminsule (the later two will be described later).  

I was wondering, since this language is born in 1996, far ahead of Haskell, why the seven hell have I never heard of it before? 

### [Nymote](http://nymote.org/)
