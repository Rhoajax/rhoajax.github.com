---
layout: post
title:  "'You Know Nothing'"
date:   2016-02-16
categories: privacy
---

##I

One article ["Time is an Illusion"](http://cacm.acm.org/magazines/2016/1/195723-time-is-an-illusion-lunchtime-doubly-so/fulltext) in 01/2016 Vol. Comm. ACM reveals an astonishing fact: the modern computers actually behave really poorly in keeping time: the quartz on motherboard that is used for timekeeping is prone to factors like temperature, leaving *a second* longer or shorter.  Since highly accurate & expensive crystals on each machine is not a likely picture, external sources for references is often necessary -- which makes *time* an oscillation rather than a fixed integer. This is the ideas of protocols like NTP and PTP. NTP applies hierarchies like DNS, with root servers having the most accurate time. When requirements for time precision is higher, such as in High Frequency Transactions, PTP is more suitable (in a controlled data centre/single network). Many details should be carefully consider, such as jitter. In the end, we will always be confined by the limited transmission speed of signals.  

> Any endeavor with a system that asks the question, “Who did what to whom and when?” and needs an an-swer that is correct to within less than a millisecond, will want to find a way to integrate PTP.

It reminds of a mystery novel by Yukito Ayatsuji: [The Clock Mansion Murders](http://www.amazon.co.uk/Murder-Clock-Lt-Valcour-Mystery/dp/1479408336): How do you feel if you suddenly find out that what you have been thought of as a most reliable locator in the universe is actually opaque, misty, and actually not (*Insert colourful and optionally offensive word*) reliable at all?

##II

> “Foes and false friends are all around me, Lord Davos. They infest my city like roaches, and at night I feel them crawling over me.” 

Do you know what your mobile phones are doing? Making phone calls, sending messages, surfing Internet? How about this: "A recent study shows that 65-75% of the energy consumed in Angry Bird on Android devices is spent by third party advertising modules"[^mobadv]? The thing is that, currently researchers are still trying hard to (make users) understand the behaviour of their very own creation more clearly. Think about it: these advertisements are crawling over our phones like maggots, and all we can do it pretend the phone is a loyal friend and well under control. (Alas, time to revisit the last minutes of *The Kingsmen*.) 

We can find loads of examples from different scientific fields. Not a news to any Computer Science 1st year student: the numbers in a computer is not unlimited. Here `1 - 65535 > 0` and `10 / 2 == 4.9999999987668` might both be true under some circumstances. That doesn't mean mathematics itself is totally bulletproof: two parallel lines can cross in some theories. The three crises in Mathematics had raised serious questions about its foundations. Some cases in Physics are surely more famous, such as Heisenberg's uncertainty principle and the cat of Schrödinger. 

##III

> "You know nothing, Jon Snow".

So here we are. On one hand, it kind of feels terrible to know that what we have been treating as common sense are actually illusions; on the other, however, in most cases it is totally OK to forget them. The clock on a computer works sufficiently good for me and Euclidean geometry is more that enough to use in my whole life time. But the lesson here is that we need to keep an open mind, and never take anything for granted when you dig deep enough in a field of research.

##IV

Maybe not about research but some facts about the harrassment women face in some part of our world still astonishes me:
> A survey by the UN in 2013 found that a startling 99% of Egyptian women are victims. [^slappingback]

We can argue it is because the conservative attitudes towards women for some religional norms. Then how about this documentary: [The Hunting Ground](http://www.thehuntinggroundfilm.com/)? Those stories happen in the top universities of USA and the world, presumeably the most civilized people of the most civilized socities.

One question is often thrown to face of victims: "If you do dress appropriately, how could they harass/assault you?" Same logic could be seen elsewhere: "If you do not show your money publicly, how could the robbers rob you?" One explanation for this kinds of comments is that the *foules* tend to deny the fact that he/she can be assaulted in normal life for no better reason than being randomly picked by the offenders. So it is a more comforting choice to close eyes and pretend all bad things happen because of the victim themselves do not behave properly. 

## Reference
[^mobadv]:  Vallina-Rodriguez, Narseo, et al. "Breaking for commercials: characterizing mobile advertising." Proceedings of the 2012 ACM conference on Internet measurement conference. ACM, 2012.

[^slappingback]: The Economist. "Slapping back." http://www.economist.com/news/middle-east-and-africa/21678788-women-still-face-constant-harassment-more-being-done-about-it-slapping