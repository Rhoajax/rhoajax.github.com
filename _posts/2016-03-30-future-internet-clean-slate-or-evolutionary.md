---
layout: post
title: "Future Internet: Clean slate or Evolutionary?"
description: "A summsary of a good article"
category: "Network"
tags: [Network]
---

For years the networking research community debates whether they should focus on designing new network architectures or keep improving the current ones. A paper [1] shows a point/counterpoint debate between two representatives of each side. In this short essay, I'd like to briefly summarize the opinions about the future development of Internet based mainly on this paper.

# Who? 

Clean-slate vs. Evolutionary

# Why? -- Main points

The main argument of Clean-slate approach is that current architecture faces many challenges: security, mobility, and network management, etc. [?] They are all deeply rooted in early design decisions of the Internet. Changes have to be made.

According to the Evolutionary approach, however, successful real-world implementation means everything. Current implementations are merely prepared for the test of economic and political constraints in the real world. As an example, ARPANET's success results from it being used as a production network.

There is no doubt that the Internet is a enormous success. However, it doesn't mean the current architecture is unarguably the "Right Thing". In fact, this paper [2] recalls some of the early reasoning that shaped the Internet protocols as it is. It turns out that some of them are merely a winner out of some possible choices. For example, the seemingly basic TCP/IP layer structure is not part of the original proposal, and "most services within the Internet would like a more sophisticated transport model than simple datagram -- e.g. a  "stream" is suggested as a possibly better building block. Besides, different network design is based on different priorities. As to ARPANET, its most important goal is its survivability, which then leading to a stateless connections. That is not necessarily the case in every network. Moreover, a lot of current research is deployed in production network, such as big companies like Google [3]. They are just not public yet. ARPANET itself is also one option out of many [?]. It is difficult to say that the success of ARPANET is totally without luck.

# What? -- Research Focus

A proponent for evolutionary approach may declare that the clean-slate approach means designing a significantly better architecture on nearly all aspects than the current one, and if it can't, it's a failure. This is a misunderstanding. The fact is, a clean-slate cares more about new methodologies for designing networks/protocols than its immediate deployment in real world. According to the clean-slate approach, the field of networking is far from mature: "We do not have anything approaching a discipline for creating, analyzing, and operating network protocols...no top-down treatment, laws, or even rules of thumbs." 

Regarding the research focus of network design theories, **prescriptive network theory** seems quite promising, against most of today's descriptive theory.

# How? -- Experiment & Implementation

The Clean-slate approach states that building and deploy real systems on experimental facilities, such as [GENI](https://www.geni.net/) and [Federica](http://www.fp7-federica.eu/), is an crucial part of a continuous cycle of research. Though the Evo declares that few clean-slate attempts succeed, such as per-flow QoSS guarantees CLNP and XCP, the fact is that IPv6 is already under a large-scale deployment. Times change, the clean-slate efforts is not necessary but also possible.

Concerning experiment and implementation in the development of Internet architectures, we should pay attention to **SDN** and **Virtulization**.

# When?

I tend to believe that "Punctuated Equilibrium" theory does apply in the evolution of the Internet, which means one species will remain stable before the next great evolutionary change. Currently the basic networking theories taught in school are still not quite different from what 20 years ago ( *is it?* ), and today may not be a perfect time for an total revolution of Internet architectures, but given cumulating enough research, *"His judgement cometh and that right soon"*.

# Reference

[1] Rexford, Jennifer, and Constantine Dovrolis. "Future Internet architecture: clean-slate versus evolutionary research." Communications of the ACM 53, no. 9 (2010): 36-40.

[2] Clark, David. "The design philosophy of the DARPA Internet protocols." ACM SIGCOMM Computer Communication Review 18, no. 4 (1988): 106-114. 

[3] Singh, A., Ong, J., Agarwal, A., Anderson, G., Armistead, A., Bannon, R., ... & Vahdat, A.. Jupiter Rising: A Decade of Clos Topologies and Centralized Control in Google's Datacenter Network. In Proc. 2015 ACM SIGCOMM (pp. 183-197).

This work is licensed under [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/).
