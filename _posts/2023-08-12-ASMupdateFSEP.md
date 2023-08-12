---
layout: post
author: RWG
title: ASM update, August 12 2023
tag:
    - Goal 2
    - Moderation
    - alternative social media

comments:
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 110878304823659934
---

It's been a while, thanks to drama with rent and apartments (welcome to Toronto, Robert), but I'm back with another Alternative Social Media update!

<!-- more -->

## New challenges in moderation and new responses

*Content warning: abuse mention*

I imagine most readers of this blog saw news about the [Stanford Internet Observatory report](https://cyber.fsi.stanford.edu/io/news/addressing-child-exploitation-federated-social-media) on child sexual abuse material (CSAM) on the fediverse. I know I did. I'm currently the admin of [AoIR.social](https://aoir.social/), and the report came out while I was in the middle of moving apartments -- and in the middle of relying on dodgy mobile hotspot internet. Regardless of the bad connection and stress of unpacking, the report's publication prompted me to immediately do an audit of AoIR.social's instance blocklist to see if we were facing any risk of having CSAM hit our server.

I am quite confident AoIR.social is in good shape. Why? Because on day one of AoIR.social (months before the Stanford report), I imported blocklists. First, I grabbed [Oliphant's Tier 0 Blocklist](https://codeberg.org/oliphant/blocklists), and later [Ro's The Bad Space](https://thebad.space/) list. Both of those are based on community consensus about who are the bad actors on the fediverse, and by importing the lists into AoIR.social's moderation panel, bad actors -- including the ones implicitly identified in Stanford report -- were already blocked.

So, while the Stanford report was scary as hell, the community has been aware of bad instances for a while now. The community is sharing knowledge about the bad servers and is blocking them. As one admin put it to me, any fedi admin with any consciousness about moderation has been blocking the bad instances for a while now.

In the time since the report came out, I've interviewed Oliphant, Ro, and other respected fediverse admins and they are advocating for easier use of blocklists to prevent the fediverse from being swamped with bad servers.

In fact, a great response to moderation challenges is coming in the form of Ro's [Fediverse Safety Enhancement Project](https://nivenly.org/docs/papers/fsep/). This project is about automated, consensus-based subscription blocklists. The proposed interface looks a lot like one of my favorite tools, The [Pi-Hole ad-blocking system](https://pi-hole.net/).

This is *huge.* There are so many interesting things to figure out, from the technical to social. Special attention should be paid to how such lists will be governed. The good news is there are folks working on that exact issue, including Ro and Oliphant.

Hint, hint, fellow ASM academics: this is a good topic to study! I know Ro and people like him would welcome academic knowledge about how to improve this new form of moderation.

In addition, if you're interested in supporting Ro's project, I recommend giving (you gotta give!) [to his GoFundMe](https://www.gofundme.com/f/a-new-way-to-social-media).

## AOIR Workshop is a Go
In other news, Jessa Lingel, Ashwin Nagappa, and I are hosting an [Association of Internet Researchers Preconference focusing on alternative social media](https://aoir.org/aoir2023/preconfworkshops/). This will take place in Philadelphia on October 18. From what we've seen, we're just short of full capacity. If you're going to AOIR, there may be still time to sign up if you haven't.

We're still planning details but our focus will be on research project creation and ethics.
