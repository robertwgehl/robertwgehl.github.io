---
layout: post
author: RWG
title: ActivityPub, the Non-Standard Standard
tag:
    - ActivityPub
    - Goal 2
    - Move Slowly and Build Bridges
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 111240793574116926
---

In a couple days, I head to Philadelphia for the 2023 version of the Association of Internet Researchers conference. It's my favorite conference. And to give AOIR even more credit, they were one of the first professional academic organizations to set up [their own Mastodon instance](https://aoir.social) (I participate in that project by helping run the instance).

While there, I will present a paper about the creation of [ActivityPub](https://www.w3.org/TR/activitypub/), the protocol that allows the contemporary fediverse to run.

Titled "The Non-Standard Standard: A Critical Genealogy of ActivityPub," I will argue that ActivityPub is a very unusual standard. While it was created by a W3C working group, [the Social Web Working Group](https://www.w3.org/wiki/Socialwg) during [a W3C standard process](https://www.w3.org/2023/Process-20230612/), there were many non-standard aspects to its creation.

In this post, I'll sum up my findings, arguing that there are four ways in which ActivityPub is a non-standard standard. This work is informed by reading the Social Web Working Group (SocialWG) meeting minutes, interviews with SocialWG members, and a study of historical documents.

Comments are very welcome, since this is going to be a chapter in my forthcoming book about the fediverse, [_Move Slowly and Build Bridges_](/2023/08/17/OxfordUP.html).

<!-- more -->

## Four Non-Standard Aspects of the ActivityPub standard
### 1) Corporate social media was not involved
Corporate social media wasn’t involved in the production of ActivityPub. At best, corporations like Facebook or Twitter (as they were known at the time) treated the SocialWG with benign neglect. At worst, they saw the group as utterly irrelevant to the future of social media.

It wasn't as if the SocialWG didn't try to get corporate social media involved: they repeatedly reached out to Facebook, Twitter, Sina Weibo, and other major social media corporations. But none of these companies got involved.

This is very unusual in the world of internet standards. Companies such as IBM, Microsoft, Apple, Google, Meta, Oracle, or Samsung pay membership fees and regularly send employees to standards-setting bodies, such as the Internet Engineering Task Force and the World Wide Web Consortium, in order to shape the standards that govern their industries. In fact, as much as corporations like Apple, Microsoft, and Google appear to be competing with one another, in reality they often cooperate when building standards, because the general rule is that standardized technologies are good for business.

But when it came to the SocialWG, as ActivityPub co-author Amy Guy told me, “None of the big players... no one took us seriously. No one saw [the SocialWG] as a threat. No one expected it to go anywhere…. The feeling was, it was small beans, and it wasn’t worth their time.”

### 2) The Social Web Working Group Didn't Make a Standard -- They Made _Seven_
Instead of settling on one approach to standardizing social media – in other words, a single, standard approach – the group made [seven standards](https://www.w3.org/groups/wg/social/publications/). For a typical W3C working group, that is decidedly non-standard behavior – most groups make one or two.

Based on interviews, it's clear this happened because of a lack of corporate involvement. Say what we will about corporate social media, they at least have a clear goal in mind: more users. More people’s lives to datamine, more eyeballs on behavioral ads.

In contrast, the SocialWG members took a predominantly academic or theoretical approach, which initially resulted in multiple factions each championing their own approaches. The group easily could have produced zero standards.

But in a compromise, the SocialWG decided to produce many standards. In a sense, as SocialWG member Bengo told me, the group succeeded _too much_ -- it made many standards, instead of just one or two.

All this said, while lack of corporate involvement might have unmoored the group somewhat, the interviewees I spoke to said they were grateful to make standards that did not simply support the needs of corporate social media.

### 3) ActivityPub Almost Didn't Happen
This is the biggee. ActivityPub -- the most successful product of the SocialWG by far -- almost didn't get done.

One big reason was that a federation protocol was considered to be optional by the [SocialWG's charter](https://www.w3.org/2013/socialweb/social-wg-charter.html).

But an even bigger hurdle came in the face of resistance to ActivityPub from within the SocialWG itself. As an example of the pushback, consider this Mean Girls meme:


<figure>
  <img src="/assets/images/fetchfederation.jpg" alt="Mean Girls &quot;Stop Trying to Make Federation Happen&quot; meme" title="Stop Trying to Make Federation Happen" />
  <figcaption>A variation on the Mean Girls "stop trying to make fetch happen," adapted to refer to the federation protocol</figcaption>
</figure>

Fortunately for us, ActivityPub advocates such as eventual co-author [Christine Lemmer-Webber](https://dustycloud.org/) weren't taking no for an answer. Lemmer-Webber pushed back hard against the resistance to ActivityPub.

However, even with Lemmer-Webber championing it, time was running out: the SocialWG charter set the end of the group to be mid-2017.

It took Mastodon to save ActivityPub. [Mastodon implemented a draft version of ActivityPub](https://hackernoon.com/mastodon-and-the-w3c-f75f376f422), and because this was a big deal, the W3C gave the SocialWG _two_ deadline extensions, now known as the "Mastodon Extension."

Mastodon and ActivityPub connected because of their respective developers’ desire for safety for queer and trans people. Just as “the fediverse has historically been extremely queer,” [Christine Lemmer-Webber explains that ActivityPub was, as well](https://fossandcrafts.org/episodes/053-fediverse-reflections-while-the-bird-burns.html). Lemmer-Webber says ActivityPub “was largely developed by queer people – myself included – and including also implementation developers.” Four of the five ActivityPub authors self-identified as queer.

As for Mastodon, Lemmer-Webber recalls that a large number of its “key contributors, kind of set the tone by pushing for certain features and pushing for kind of certain cultural norms that were to support queer communities that did not feel well-supported by Twitter.”

So, ActivityPub solved many problems for Mastodon – it functioned as a privacy-respecting upgrade over [OStatus](https://en.wikipedia.org/wiki/OStatus) (the original protocol used by Mastodon), a means to break away from harassment coming from some [GNU social servers](https://medium.com/@Trevatos/gnu-social-pleroma-and-the-mastodon-culture-conflict-3b10872937c2), and a way to further differentiate itself from Twitter. And Mastodon helped ActivityPub by giving its authors a big implementation -- gold in the world of standards.

### 4) Mastodon Prompted Us to Ignore 1/2 of ActivityPub
However, while Mastodon saved ActivityPub from oblivion, it has also effectively erased half of the ActivityPub standard from the internet. This is because the [Mastodon API](https://docs.joinmastodon.org/api/) is dominant across the fediverse, with non-Mastodon projects adopting it. This is in spite of the fact that the ActivityPub protocol includes an API for clients, which would allow end clients to connect to any fediverse server regardless of what software the server is running.

This client-to-server portion of ActivityPub is cited by SocialWG members as their favorite part of the standard. But it is effectively ignored. So while ActivityPub’s creators are grateful to Mastodon for saving their work, Mastodon is also a cause for lament on the part of the ActivityPub authors.

## Implications for the Future?

Overall, I found the story of ActivityPub, the non-standard standard, to be fascinating. Obviously, it's also important to the history of Mastodon. As Evan Prodromou told me in an interview, the meeting of Mastodon and ActivityPub at just the right moment in both their development "has changed history. It could be a very different story now. A different story for Mastodon and a different story for the social web."

I also wonder how this story will affect the future, as well. People are currently reviving the SocialWG, with debates happening right now about what its scope should be. Given the history I've observed, I would argue that concentrating on the SocialWG's most successful product, ActivityPub, may be the wisest move.
