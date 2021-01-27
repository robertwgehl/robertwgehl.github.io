---
layout: post
author: RWG
title: 
tags:
---
Word count: 444

this is aimed at The Reboot. It's about centralization of DNS and how to mitigate that problem.

Points I can make
* Berners-Lee's comment dates back a ways. Similarly, Ian Clarke in 1999. A lot of recognition that DNS is a problem for decades. Yet we're only now addressing one key problem: encryption
* Tor had the whole IETF .onion TLD issue -- and they worked to get .onion *out* of DNS for privacy purposes.


Ian Clarke's observation kicked off several projects that eschewed the DSN altogether: Freenet, I2P, and Tor in the early 2000s. Along with using IP addresses, the DNS was seen as too much of a liability for these darknet systems. 

There have been a host of projects seeking to decentralize DNS. In a sense, they lie like broken ships around a jagged rock. The edge of the rock is Zooko's Triangle. Named for computer scientist Zooko Wilcox-O'Hearn, Zooko's Triangle suggests there are three features of naming systems: security, human readability, and decentralization. However, when you build a naming system, you get to pick just two.

There are naming systems that opted for decentralization and security, and the have the URLs to prove it. Ian Clarke's Freenet relied on cryptographic hashes. The Tor Project's onion sites began as 16-character alphanumeric strings and are now 52??? characters. 

Their lack of human readability is an asset to some people: these are "dark web" systems which protect user identities (MORE). But it's a liability to most of us used to the public Internet. Cloners, scammers.

So the Dark Web systems chose two. In the case of the DNS, it was maybe 1 and a half. The wonder of the DNS is that you can type www.thereboot.com and not think about that site's IP address (192.0.66.136). Companies snapped up .com domains in the mid-to-late-1990s -- the human-readable URL became a marketing tool. Unlike cryptographically self-authenticating strings of alphanumeric characters, Pets.com became a household term.

It's only in the past few years that DNS has been moving towards encryption. DNS might have gotten half a point for being somewhat distributed, but as the likes of Clarke and Berners-Lee revealed, it was never topologically decentralized. 

And the turn to encrypting DNS and adding security from Zooko's Triangle is actually making the DNS more centralized.

Christian Grothoff has been attacking this problem for the past decade or more. 

What the hell to do? Can a blockchain approach scale? Must we always fasten down things with identity-handles? Twister claims to have solved the problem.