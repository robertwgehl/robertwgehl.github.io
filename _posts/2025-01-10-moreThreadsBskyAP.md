---
layout: post
author: RWG
title: 'Watching Threads, Bluesky and Decentralization, and ActivityPub Trust and Safety'
tag:
    - Threads
    - Bluesky
    - ActivityPub
    - ASM update
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 113805472773988685
---

This weekly [Alternative Social Media update](/tags/asm update.html) -- the first of 2025! -- is about getting caught back up with some things that have happened in the past month. First up, I'll relate the latest changes at Meta to a specific interest of mine, Threads's fediverse blocklist. Then, I'll point you to a very fascinating back-and-forth discussion about Bluesky's ATProto and ActivityPub (as well as OCapN). Finally, I'll let you know the latest in ActivityPub Trust and Safety.

<!-- more -->

## Monitoriing Threads's Blocklists
By now, you've likely heard the news that [Meta is changing many of its policies](https://www.404media.co/its-total-chaos-internally-at-meta-right-now-employees-protest-zuckerbergs-anti-lgbtq-changes/) (and board members) -- all likely due to the return of Donald Trump to the US Presidency. Aside from recruiting [a domestic abuser](https://www.espn.com/mma/ufc/story/_/id/35427773/ufc-dana-white-says-criticism-physical-altercation-wife-100-warranted) to the board and [ending fact-checking](https://www.aljazeera.com/economy/2025/1/10/metas-decision-to-end-fact-checking-captures-freewheeling-zeitgeist), I find the most egregious change to be specifically stating that [calling LGBTQ* folks "mentally ill" is now allowed](https://www.wired.com/story/meta-immigration-gender-policies-change/) (I'd say, encouraged, since it's specifically called for). 

I'll set aside re-declaring my decades-long loathing of Facebook/Meta to talk about a specific project I started a while back, one that is relevant to my interest in alternative social media and has taken on new importance in light of all this.

I've been tracking [Threads's fediverse blocklist](https://www.threads.net/moderated_servers). I first wrote about it [midway through last year](/2024/06/28/ThreadsBlocking.html) and [wrote an update last month](2024/12/13/threadsmoderation.html). Since then, I've been regularly collecting the Threads blocklist. 

My idea is to see how it evolves over time. I'm curious to see what changes in the future, since the community standards of Meta as a whole have shifted to appease the US right (and thus apparently foist US right-wing views on the rest of the world). Watch this blog for updates.

## Bluesky's Decentralized Heaps
I won't be able to do these posts justice, but I do want to flag an important blog-post-based conversation that has happened recently. One participant is Christine Lemmer-Webber, who not only was one of the co-authors of ActivityPub but is also [actively working on new decentralized web protocols](https://spritely.institute/). The other participant is Bryan Newbold, a Bluesky engineer.

This all started with Lemmer-Webber's incredible post, ["How Decentralized is Bluesky, Actually?"](https://dustycloud.org/blog/how-decentralized-is-bluesky/). Again, I can't do it justice -- go read it, but note it's long and gets technical. My takeaway from that post was that [I remain right in my basic claim](/2024/04/30/DecentralizedNoncentralized.html) that Bluesky is "decentralized" in the sense that it is a center is spinning off parts of itself. 

Reading Lemmer-Webber's post leads me to see Bluesky as decentralized in the same way Bitcoin is: sure, you can get the entire blockchain, but it's [630GB and steadily growing](https://ycharts.com/indicators/bitcoin_blockchain_size), so why would you? Likewise, if I read Lemmer-Webber correctly, Bluesky's "shared heap" architecture would mean anyone hoping to run a fully-fledge ATProto-based service would have to replicate all the messages in the network. As she writes,

> A world of full self-hosting is not possible with Bluesky. In fact, it is worse than the storage requirements, because the message delivery requirements become quadratic at the scale of full decentralization: to send a message to one user is to send a message to all. Rather than writing one letter, a copy of that letter must be made and delivered to every person on earth.

In response, [Bryan Newbold notes](https://whtwnd.com/bnewbold.net/3lbvbtqrg5t2t) that this is not incorrect: Bluesky is making a mass public messaging system, which is distinct from small community networking found among self-hosters. "Smaller more densely-connected communities are super important, and are where folks should probably spend the majority of their hours," he writes. But "Smaller communities are probably not well served by global public broadcast systems."

To be fair to him, no, small communities aren't well-served by massive global broadcast. (If only there was a way to build a global network out of many small communities who band together through an open protocol and shared values. Hmm.)

There's more to this back-and-forth -- a lot more. Including [Lemmer-Webber's reply to Newbold's reply](https://dustycloud.org/blog/re-re-bluesky-decentralization/), where she goes through the history of ideas of decentralization, all in support of her call for a new approach, [OCapN](https://ocapn.org/). It's worth a read -- go read it, too! -- but I will note that it appears both Lemmer-Webber and Newbold agree that Bluesky's architecture is, in fact, a "shared heap" -- which is not amenable for federation (and thus, in my view, it's not amenable for _[noncentralization](/2024/04/30/DecentralizedNoncentralized.html)_.)

## ActivityPub Trust and Safety

Earlier this week, I took part in my first [ActivityPub Trust and Safety Task Force](https://github.com/swicg/activitypub-trust-and-safety) meeting. This group, which is currently co-chaired by Emelia Smith and Darius Kazemi, has three foci. One is to [write a report](https://github.com/swicg/activitypub-trust-and-safety/issues/32) on the current state of moderation practices on the fediverse. Another is to [improve ActivityPub's moderation tooling](https://github.com/swicg/activitypub-trust-and-safety/issues/38). A third (which I will admit isn't clear to me just yet) is to work on [content warnings and labels](https://github.com/swicg/activitypub-trust-and-safety/issues/41). 

It's early stages for this task force, although the folks involved have been working on these issues for years. Much of the discussion during my first meeting was about scope -- a really important question, given the scale of "trust and safety"! For my part, I intend to contribute to the report. To do _that_, I will need to do a lot more work studying the various issues being raised in the task force's [Github](https://github.com/swicg/activitypub-trust-and-safety/issues/), as well as [Fediverse Enhancement Proposals](https://codeberg.org/fediverse/fep).
