---
layout: post
author: RWG
title: FOSS Finds, On Demand Edition
tag:
    - Goal 2
comments: 
  show: true
  fedihost: scholar.social
  fediusername: robertwgehl
  fediid:
---
As I've written before, I'm working on a book about the fediverse. To do that properly, I need to have a good understanding of ActivityPub, a key underlying protocol that enables servers to talk to one another. A member of one ActivityPub-enabled server, such as Mastodon, can connect with another on a different server -- even if it runs different software, such as Pixelfed. It's quite a technical achievement and -- I believe -- it really needs to be part of the conversation when we discuss things like moderation, platform governance, and the political economy of the internet.

I like to study how such software develops over time, so I've been going through the [meeting minutes of the W3C Social Web Working Group](https://www.w3.org/wiki/Socialwg). It's been fascinating to see how they, for example, discuss [user stories](https://www.w3.org/wiki/Socialwg/Social_API/User_stories) and how they inform the protocol's functionality.

I posted a short note about doing this work on my home Mastodon instance, scholar.social, and people noticed! This is what I love about scholar.social -- when I talk about geeking out about something, people jump in. Another fediverse member suggested I take a look at [this week's FOSS Find](https://yewtu.be/watch?v=c17gjxEoyMQ). And now, I'm writing up notes about it -- at the request of the author of the Find. Read more after the jump.

<!-- more -->

## [Benjamin Goering on “ActivityPub W3C Recommendation.”](https://yewtu.be/watch?v=c17gjxEoyMQ) 2022.

This is a recording of a presentation by Goering at "Papers We Love" earlier this year. Goering has been “working on decentralized social networking” for 15 years, and here the "paper" he's lovin' on is ActivityPub, a W3C standard. In these notes, I'll include approximate minute markers, typically tied to the title of the slides. I'll include summaries, and some of my own personal notes. This also includes some notes on Christine Lemmer-Webber's comments during Q and A.

Goering's agenda is to talk about ActivityStreams, the W3C Activity Streams 2.0, and then ActivityPub, past and future.

### History of Activity Streams

2.47 - “History (1997 and before) - Activity Theory”: He notes the connection between this protocol and sociology. The screen shows the book _The Russian Theory of Activity_ by Bedny and Meister, 1997. It's about
human-computer interaction thinking from Russia. In the 1990s, Western researchers took these ideas up.

3.44 “I don’t know much about this,” he notes, but he likes the idea of sociology informing software.

3.47 - History (2005) - bengo blogging: He points to his blogging experience as a teen -- the web wasn’t centralized. It was blogrolls, links, the “whole web was a social network” with RSS helping make connections.

4.32 - History (2007) - Giant Global Graph aka ‘web 3.0’: Here we learn about Tim Berners-Lee's work on the semantic web with the MIT decentralized group lab. The semantic idea is links between data within web documents.

5.59 - History (2007) - https://diso-project.org: This is about the Distributed Social project.

6.25 - History (2007) - OpenSocial, OpenID 2.0: OpenSocial was a Google project. OpenID is still around. Goering implemented these on his blog.

8.12 - History (2008) - OpenSocial Foundation: This was a foundation started by Google, Yahoo! and MySpace.

8.46 - History (2008) - activity-streams mailing list: he uses the Internet Archive to find some of the original posts to this list.

8.50 - History (2009) - Facebook Activity Streams: “Facebook Open Stream API” - this would allow applications to read the Facebook Stream, and it would run on ActivityStreams 1.0. ActivityStreams 1.0 was a description of social activities in XML.

9.36 - ~2010 - GNU Social, status.net, pump.io. Here we're talking about projects like diaspora*, ActivityPump.

~11.23 - an open social web: In 2009, he notes, Google, Facebook, MySpace, Microsoft, Yahoo all tried implementing open social networking “using a common data model.” “That’s no longer the case. What happened? How can we get back? Should we even?” This is a very important observation. What about the business model precluded such a movement? He posts a Quora article that discusses how Google and Facebook fought over OpenSocial -- FB saw it as encroaching on its turf.

12.13 - Embrace, extend, extinguish: He notes that this was a real possibility at this point. Think about if Google were to really build out a decentralized social standard and then either abandon it or make parts of it proprietary. The idea here is that someone like a Microsoft takes up open standards, extends them with proprietary extensions and gains market share, then extinguishes the standard.

13.01 - OpenSocial Foundation PR: He posts the 2014 announcement that OpenSocial Foundation (the one started by Google, Yahoo, and MySpace) “moved” to the W3C Social Working group I saw “moved” because the IRC meetings show they didn’t know this was happening and that it put no obligations on them; it just dumped the money on the WG, from what I can tell. He notes that they were donating their documents and code.

### Part 2: W3C Social Web WG

14.24 - https://www.w3.org/2013/socialweb/social-wg-charter.html: He looks at the Charter for the Working Group. The Charter was meant to constrain and guide the group. He works through the Charter, talking about “user control of personal data,” federation, “embedded experiences”, and “enterprise social business.” The latter is about replacing email? Embedded experiences is about having social events trigger consumption “within the page itself." Federation is what it implies -- two or more organizations communicating.

Corporate actors were involved: IBM, Yammer, Salesfore was making Chatter.

~15.50 goals based on the charter: make a Social Syntax (in JSON-LD). Make a Social API (client applications). Make a federation protocol, so the servers could talk to one another.

16.52 - Activity Streams 2.0 Core: ActivityPub depends on AS 2.0, but AS 2.0 is also independent. AS is about “social data syntax” (in the charter). ActivityPub fulfills federation mandate.

2014 was a time when JSON was being used to describe things, Actor Verb Object. He talks through debate over JSON versus JSON-LD. The goal was to make it extensible, so JSON-LD is attractive.

19.43 - Activity Streams 2.0 Vocabulary: He walks us through Core types, Actor Types, Activity Types, and Object and Link Types.

21.42 - ActivityPub - https://www.w3.org/TR/activitypub/: ActivityPub makes use of ActivityStreams 2.0. HTTP helps send the AS data around (though he will go on to note that AP is not necessarily tied to HTTP). “Honestly, it works a lot like email,” he says: there are inbox, outbox terms. He wonders if they should have extended or modified SMTP [that's a really intriguing little thought experiment!]

Christine Lemmer-Webber, who is in attendance (and who also contributed a great deal to this project) confirms that it could be pushed past http, like IPFS, but that it relies heavily on the HTTP verbs GET and POST. Goering responds: ah, this is why there are so many verbs in the protocol -- to make it as independent of HTTP as possible.

25.25 - ActivityPub Actors - https://www.w3.org/TR/activitypub/: Here we discuss Actors. The Actor Model from computer science. This is taken up in blockchain stuff, too. “Really, ActivityPub is trying to find a way to describe all these actors.” A stream of inputs and a stream of outputs between actors. The Actor Model in computer science goes back to 1973. [As an aside, tt strikes me as very individualistic -- the actor speaks, a stream comes forth. Is there a way to model collective knowledge?]

26.34 - ActivityPub Interactions - https://www.w3.org/TR/activitypub/: Section 5, Collections: servers maintain these -- outbox, inbox, followers, liked, following. Section 6, Client-server interactions, how the client’s typing gets encoded in the syntax. Section 7, Server to server interactions: activities such as a follower activity means another server updates the follower collection.

28.58 - ActivityPub “Security” [note: these quote marks in the original]: Security, he notes, is an afterthought after making the protocol. They wanted to publish the protocol and left security for the future. There's a discussion of authentication schemes, signed keys. This was a bunch of suggestions, not “normative” (not required to abide by). He gets a question about authentication and identity, he notes that Oauth is the recommended approach but it’s an architecture, not a protocol.

32.19 - Social Web Protocols: This is another document that the WG produced. Amy Guy, University of Edinburgh edited it. This compares a bunch of protocols -- this helped the group keep track of competing protocols. He notes that this is a good doc to study, so I put it in Zotero.

33.11 - relationship to Tim BL’s Solid: Starts in MIT with decentralized web group. Solid tried to leverage AS, AP. Solid gets lots of coverage.

### Part 3: ActivityPub Today

34.25 - https://github.com/BasixKOR/awesome-activitypub: List of projects running on the protocol. Nextcloud social is one. Castling.club -- chess over activitypub, he cites this as an example of emergent, unexpected results of a protocol.

35.53 - Mastodon wikipedia page: Mastodon was around before AP; they were using status.net, they were very early adopters of AP. He says he’s seen estimates that 10 million people are using Mastodon; he notes it could be much more. [I should ask him where he's getting these numbers; everything I've seen estimates about 5mil users].

He points out Content Warnings as an innovation. Thus, he argues ActivityPub as a protocol helps set the base for these end-user features such as CWs.

37.58 - discussion of EU, Next Generation Internet: Billions of dollars to spread European values on the internet.

If a server implements ActivityPub well, end users get a “lot of choice in how they participate in the network.”

~40.00 - he talks about the term “fediverse.” He notes the fediverse may not necessarily all use the same protocol. The forum for activitypub is socialhub.activitypub.rocks -- this defacto replaces the Social Web WG as an organizing site.

41.24 - ActivityPub Conf: He cites a talk “Architecture of Robust Kindness.”

### Part 4: Future of ActivityPub (it’s up to you)

42.13 - OcaPup: Object Capabilities + ActivityPub. Christine Lemmer-Webber working on this project to pursue security for marginalized groups. “OcapPub: Towards networks of consent” [I need to learn more about this!]

43.40 - Extensions?: Discusses ways AP can be extended. This can be done via websites without permission from the WG; and if an extension catches on, it may be added to the AP itself. This is a benefit of JSON-LD; easily extended via RDF.

45.04 - Possible Futures: This includes non-http, e.g., Bluetooth, Data integrity, portable identity. Discussion of URNs versus URLs. Concerns about man-in-the-middle attacks that rewrite HTTP. Discussion of a protocol that would delegate the ability to post to others/other devices.

50.22 - Related Work/Current Events: Slide presents Bluesky (blueskyweb.xyz), Solid, Spritely. Discusses Elon Musk, EU regulations. Due to the EU regulation, interoperability is much more important

~52.00 - Start Using ActivityPub: Discussion of clients, Mastodon instances.

### Q and A

~56.00 - Christine Lemmer-Webber discusses the difference between the client-to-server part of AP and the server-to-server part. S2S is widely implemented; she notes that they were shocked that the C2S has not been well-implemented. Also notes they only barely got the federation part done. She explains C2S works like an email client: client to server, server to next server. She also notes that SMTP’s and ActivityPub’s “notions of trust” are “broken”.

1:00.00 -- Christine volunteers to clarify some things, noting Goering covered a lot of history she didn’t know. Christine was in Ostatus et al; Bengo was more familiar with Activity Streams. She notes Ostatus implementations often weren’t compatible.

1:02 - ActivityPub: originally was requiring C2S and S2S implementation. These were divided later on. She talks about MediaGoblin, which promised federation. She hired Jessica Tallon to pursue it. They got involved in the W3C standards, and they were passionate contributors (they didn’t start that way) who got more and more involved.

It was not obvious ActivityPub was going to succeed. There were many competing protocols, none of which were talking to each other -- and the common sense was that people weren’t going to get along.

