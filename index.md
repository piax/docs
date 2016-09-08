---
layout: default
title: PIAX distributed computing middleware
---
<div class="banner"><img width="100" src="piax-font.png"></div>
<div class="banner_bottom">[piǽks / piʌf]</div>

PIAX (P2P Interactive Agent eXtensions) is a framework for distributed
computing.

## News

* 2016/09/01 [PIAX GitHub](https://github.com/piax/piax) is now available
* 2015/06/08 PIAX 3.0.0 is released
* 2009/10/21 PIAX 2.1.0 release
* 2008/11/1 PIAX 2.0.0 release
* 2007/3/26 PIAX 1.0.0 release

## What is PIAX?

PIAX has two major features: One is a transport framework based on P2P
structured overlay. The other is a distributed computing framework
with mobile agents.

As a transport framework, PIAX provides Java class library called
'Generic Transport(GTrans)'. GTrans provides simple interfaces to
develop portable and sophisticated network applications that
integrate multiple different network features. By incorporating
composite pattern, GTrans enables programmers to use various kind of
network features by a unified interface.  GTrans allows applications to
specify communication destinations in flexible ways.  One can use IDs,
keys, locations, and conditions of attributes to specify remote nodes,
in addition to conventional locators (such as IP addresses and
Bluetooth MAC addresses). 

As P2P overlay networks, there are implementations of [Skip Graph](http://dl.acm.org/citation.cfm?id=1290674),
Suzaku, LLNet, DOLR and Flooding to support various kinds
of discoveries.  The structured overlays of PIAX are implemented as
a scalable and fault-tolerant system using [DDLL](http://ieeexplore.ieee.org/document/7328521/), which is a distributed
algorithm for constructing distributed doubly-linked lists. DDLL
maintains consistency with regard to lookups even in a churn situation
where multiple nodes are simultaneously inserted or deleted. DDLL also
provides a link repair mechanism.

As a low-level network transport interface, UDP, TCP and
emulation are supported in GTrans. Network features such as channels,
handover, fragmentation and RPC are provided in an abstracted
manner. These features enable programmers to implement their
applications or network feature in minimal efforts.

As a distributed computing framework, PIAX provides mobile agent
mechanism with simple APIs. The agents of PIAX support remote
procedure calls with discoveries, which we call 'discovery calls'. By
discovery calls, the agents can issue procedure calls to other agents
without knowing their existence. It enables applications to cooperate
each other in the asynchronous and on-demand way in the loosely-coupled
environment.  The agents integrates versatile P2P overlay networks
(e.g., LL-Net, DOLR) as a multi-overlay mechanism to
support discovery calls. The multi-overlay mechanism supports plug-in
independent P2P overlay networks.

PIAX is originally developed for ubiquitous computing, but the
characteristics of PIAX can be applied to various situations such as
cloud computing, smart cities, IoT applications, etc. Since PIAX
enables many computers to cooperate efficiently, a huge amount of
servers or devices can cooperate with each other and a scalable and
fault-tolerant system can be realized.