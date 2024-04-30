---
layout: post
author: RWG
title: Decentralization or Noncentralization, Bluesky or the Fediverse?
tag:
    - Bluesky
    - Fediverse
    - Goal 2
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 112361505840566144
---
I'm nearing wrapping up drafting _Move Slowly and Build Bridges_, [my book about the fediverse](/2024/02/11/Move-Slowy-Preview.html). I do several things in the book: provide some history, show the struggles of instance admins, talk about the politics of blocklists.

I also develop a concept in the book, "noncentralization." In this blog post, I want to talk about what this means and contrast the term with the more popular one, "decentralization." To do that, I want to contrast the fediverse with another system, Bluesky.

<!-- more -->

## Decentralization versus Noncentralization
As I argue, the very term "decentralized" implies that there was once a center, something that has been broken up, _de_-centered. This process could work in reverse -- something decentralized could be _re_-centralized at a later point. It might be hard to do, but it's implied by the idea.

In contrast, _non_-centralized means just that: designed to avoid a center emerging. It's a design goal from the outset. (Whether it is successful is another matter.)

I get this term from political philosophy, specifically federalism theory. As Glen Moots argues in _[The Ashgate Research Companion to Federalism](https://www.routledge.com/The-Ashgate-Research-Companion-to-Federalism/Ward/p/book/9780367603021)_, in federalist political structures,

> Power is diffused. Centralizing or concentrating power in a federalist system risks breaking the structure and spirit of the constitution. It negates the whole telos of federalism. Non-centralization applies to the United States, Canada, and Switzerland, for example. In each case, there is no central government that controls all the lines of political communication and decision-making. States, cantons, or provinces are not creatures of the federal government (Elazar 1984b 14).

We might argue whether or not the US or Canada is truly non-centralized. But the point Moots is making is that the ideal political structure envisioned by federalism doesn't involve breaking up an existing center. As Moots writes, "decentralization implies the existence of a central authority that can decentralize or recentralize as it pleases." Noncentralization by contrast involves designing political structures so that there are many, smaller locations where power is exercised. This allows for a high degree of local autonomy coupled with a larger-scale agreement about shared ethical values. (In the case of the fediverse, I call such a structure "the covenantal fediverse," but that's a topic for another post.)

Now, in my work on alternative social media, I'm not talking about states. I'm talking about social media. But given that social media must be governed (e.g., moderated, have policies), and given that we're now living in a time of federated social media, I think it's a good idea to look to federalist political theory to think about how things might work.

The two main projects seeking to federate social media today are the ActivityPub-based fediverse and Bluesky. Drawing on the noncentalized/decentralized distinction, I would argue that Bluesky is decentralized -- and as such will never truly be federated. The ActivityPub-based fediverse is closer to the noncentalized ideal. But it is vulnerable to centralization, too.

## Bluesky and decentralization
Bluesky has the ambition to be a decentralized Twitter. To that end, Bluesky has started out centralized and is slowly spinning out parts of itself from the center to the edges.

A simple example is support for GIFs. Bluesky has [proudly declared they now let people post GIFs](https://bsky.app/profile/bsky.app/post/3kqy4mjw5eo2t)... _powered by Tenor_. What's Tenor? It's a [Google-owned GIF repository and search engine](https://en.wikipedia.org/wiki/Tenor_(website)) with [an API](https://tenor.com/gifapi/documentation). So people can "post" GIFs to Bluesky insofar as that means they pull in a GIF from another, centralized database of them and have it embedded in the stream.

In keeping with decentralization, Bluesky says that "custom GIFs" will be implemented later. I take that to mean they will allow uploading a .gif file from a local machine. You can't do that now (I tried, and it just is a still image). So for now GIF posting is decentralized in that it involves two major services (Bluesky and Google's Tenor), and in the future these centers might get broken up further.

It's hard not to see this as symptomatic of Bluesky's approach as a whole. It started out as one central service, Bsky.app, with the promise that people could run their own Personal Data Servers (PDSes) in the future (a future that is, to their credit, slowly happening).

But Bluesky distinguishes between "speech" and "reach," meaning that while people can run their own PDSes and speak, their posts won't appear across the network unless they are indexed or relayed -- and Bluesky runs the only indexer. They promise that in the future that non-Bluesky employees can run indexers/relays, too, but that's a costly proposition -- much more so than running a PDS.

In the meantime, Bsky.app, the central Bluesky server, includes a connection to Twilio Segment, which is ["The leading customer data platform, powered by CustomerAI"](https://segment.com/).

<figure>
  <img src="/assets/images/bskySegment.png" alt="A screenshot of my Noscript Firefox extension on bsky.app, showing Segment.com as a source for a script">
  <figcaption>A screenshot of my Noscript Firefox extension on bsky.app, showing Segment.com as a source for a script</figcaption>
</figure>


Segment's presence on the site raises the specter of behavioral advertising -- a possibility the company has never denied. Consider this Q and A between [Bluesky CEO Jay Graber and _WIRED_](https://www.wired.com/story/bluesky-ceo-jay-graber-wont-enshittify-ads/):

> **Are you thinking about advertisements at all?**

> There will always be free options, and we can't enshittify the network with ads. This is where federation comes in. The fact that anyone can self-host and anyone can build on the software means that we'll never be able to degrade the user experience in a way where people want to leave.

That's not a "no." It's hard to understand exactly what it is.

It might be, "we won't do ads." But then what's the Segment integration for? Segment's presence might just mean Bluesky will sell data to marketers but not allow ads. (After all, brands are certainly welcome on Bluesky and may want insights into their audiences.)

Or, it might be, "if we do ads _wrong_ people will leave, so we better do them right." That seems likely given the Segment integration.

Or maybe Graber's answer means, "if we do allow ads, people can just move to another PDS and appview." That is, we can run ads on our PDS/appview, but others may decide not to.

In any case, if the costs of running Bluesky infrastructure can be partially subsidized by ads or other behavioral marketing techniques (without "enshittifying" everything), then most likely there will be one central mechanism by which anyone wishing to subsidize their part of the network (e.g., a distinct PDS) can do so. If Bluesky runs this monetization system, then de facto third-party PDSes that use it will be closely tied to the center.

Decentralization also holds when we consider the underlying protocol Bluesky is making, ATProto, That's being done by them alone. They promise it will be transferred to a standards body (e.g., the IETF) in the future so that it is more open. It could be that they do this, but it would replicate the pattern: they start with a center and then decentralize. The protocol will be made in-house, and even after being moved to something like the IETF, it can be dominated by Bluesky the company.

Overall, Bluesky is decentralized in the sense I'm using it here: there's a center that's being broken up. This might turn out for the best. [Steve Klabnik's explainer](https://steveklabnik.com/writing/how-does-bluesky-work) has a similar (if more sanguine) take:

> ...the BlueSky team has demonstrated, in my personal opinion, enough understanding and uncomfortableness with being in control here, and it’s designed in such a way that if other, better systems develop, you can move to them. They’ve also indicated that moving governance of did:plc to some sort of consensus model in the future is possible. There are options. Also, others could run a did:plc service and use that instead if they prefer, too.
> I personally see this as an example of pragmatically shipping something, others see it as a nefarious plot. You’ll have to decide for yourself.

So it's a pragmatic choice to do everything centrally, ship it now, and devolve it to the edges over time.

But it seems to me that, no matter what, much will continue to flow to the center, either on purpose or through inertia. And edge-parts that misbehave (by Bluesky's standards) might be recallable to the center. For example, if allowing just anyone to run an indexer causes problems down the road, Bluesky's control could be re-asserted later.

## Noncentralization and the fediverse
I would argue that the ActivityPub-based fediverse is much closer to the noncentalized ideal I would prefer. By "fediverse" I mean the ActivityPub-based fediverse.

How?

Well, for one thing, there's a whole host of different projects. From PeerTube to the Wordpress plugin, it's a network of heterogenous social media services. ActivityPub allows for a range of technologies. Moreover, ActivityPub is already an open standard -- it was that way from day 1. It supports a bewildering array of social media projects.

Now, you might argue "Mastodon is dominant." Yes, Mastodon is dominant, but it's not the only game in town. And even _if_ the fediverse was mostly Mastodon, what does that mean? There are forks of Mastodon (Glitch, Hometown) and heavily modified Mastodon installations (awoo.space). Mastodon isn't one thing -- it's many things.

You might say that there are points of centralization at the instance level: that an instance is a center. But they are not central to the network. There are tens of thousands of them, ranging from instances-of-one to large instances. And there's no guarantee they will connect -- they might have ethical disagreements. The smallest instance can block the biggest one. Indeed, that's why instance blocking exists.

Now, you might say, "What about Threads?" And _that_ is a concern of mine. The existing fediverse is so small that the appearance of a corporate-controlled network with 100 million+ accounts means that de facto there is now a center. That is indeed a problem.

There are solutions, though. One is #[fedipact-like agreements](https://fedipact.online/) to block Meta. I endorse this. In my view, the whole point of federated, alternative social media is to be a better alternative to corporate social media, not a means to connect to it.

Another approach to Threads is to hope other big companies get involved in the fediverse to balance things out with Meta. With Meta here, let's get Apple and Google and Microsoft to adopt ActivityPub. To cite Evan Prodromou, that's a ["Big Fedi" solution](https://evanp.me/2023/12/26/big-fedi-small-fedi/).

I don't like this solution, because I would rather see the fediverse be comprised of tens or even hundreds of thousands of small, self-governing communities. That would be closest to a noncentalized ideal: it remains a system where there was no center in the first place, where many small communities band together into a big network through mutual, shared ethical values, and any attempt to centralize will be resisted.

## Bluesky won't be federated
Reading the documents and discourses, it's clear to me Bluesky won't be federated -- it will be decentralized. It won't be federated because it won't be noncentralized. It is not being designed that way, and I do not believe it will ever be that way. Some of its centers are going to hold, which negates the idea of distributing power and control. And those things that are spun out to the edges could be recallable in particular ways.

The fediverse is closer to the ideal of noncentralization, but of course Threads indicates that such a thing is fragile. Designing a noncentralized system is hard work, and it can fail.
