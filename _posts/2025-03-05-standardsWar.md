---
layout: post
author: RWG
title: 'Standards War?'
tag:
    - ActivityPub
    - ATProto
    - IFTAS
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 114112053758622551
---
While I was not surprised by the announcement, it was still sad to read the news that [IFTAS is shutting down several of its services](https://about.iftas.org/2025/03/03/iftas-service-shutdowns/) for lack of funding. It is hard for me not to see this as another aspect of a potential "standards war" between ActivityPub and ATProto.

<figure>
  <img src="/assets/images/railroads.jpg" alt="a collection of railroads, each clearly with different gauges">
  <figcaption>Different standards.</figcaption>
</figure>

## What's IFTAS?

What is (or was) IFTAS? IFTAS is the Independent Federated Trust and Safety organization,* a non-profit that was inspired by the 2022/2023 influx of people into the fediverse after Elon Musk purchased Twitter. As they wrote in an [introductory blog post](https://web.archive.org/web/20230816114557/https://about.iftas.org/2023/08/09/iftas-federated-trust-and-safety/), "More and more people were joining [Mastodon and the fediverse], and more and more people were wondering 'if this keeps growing, how does moderation scale?'" 

IFTAS's founder, [Jaz-Michael King](https://jaz.co.uk/), successfully raised initial funds to bring the organization online. The organization ran fediverse moderator needs surveys and later developed a space for moderators to share knowledge (IFTAS Connect) as well as various blocklists that fediverse admins could import.

Full disclosure: [I gave money to IFTAS](https://about.iftas.org/first-50/). I also asked the Association of Internet Researchers (AoIR) to [give money to IFTAS](https://about.iftas.org/our-supporters/), since AoIR's [Mastodon server](https://aoir.social) has benefited from ITFAS's services. 

I know AoIR.social has benefited because I'm one of AoIR.social's admins, and thus I do a lot of content moderation on that server. While we did not really use IFTAS's blocklists specifically, we certainly have [benefited from the use of blocklists](/2023/09/20/blocklists.html) in general. We did directly benefit from IFTAS Connect -- I have an account there and read threads about moderation challenges, learning from the experiences of others.

While IFTAS was providing a valuable service to the fediverse, [they recently announced](https://about.iftas.org/2025/02/06/funding-challenges-and-the-future-of-our-work/) that they were struggling to get funding:
> Despite our best efforts to secure sustainable funding, IFTAS is now facing a critical financial shortfall. Without immediate support, we will be forced to severely curtail our activities in the next 60 days. With our current commitments we will be unable to pay our bills in April.

That was one month ago, and indeed IFTAS just announced [they are shutting down several services](https://about.iftas.org/2025/03/03/iftas-service-shutdowns/).

This is going to be a big loss. As Laurens Hof at [_The Fediverse Report_ notes](https://fediversereport.com/fediverse-report-106/), noncentralized social media needs some forums where folks can gather to discuss the the challenges they face:
>  IFTAS, as a grassroots fediverse organisation, is one of the best-placed organisations to have build trust and provide a nexus around which such infrastructure could be build. IFTAS got pretty far with their rollout of FediCheck, which was building such a place for collaboration between server admins. Now that IFTAS will not be the center around which shared moderation infrastructure can be build [sic], will there be another organisation in the future to do so? Especially when IFTAS found out that getting funding for such a project is so difficult?

But is getting funding so difficult? I wonder.

That brings me to the provocation I dropped in the first paragraph: there may be a standards war brewing. To see that, let's look at another organization that is spinning up as IFTAS is winding down.

## Free our Feeds
In January 13 of this year, a consortium of actors, bloggers, academics and tech luminaries [launched "Free Our Feeds"](https://web.archive.org/web/20250113141611/http://freeourfeeds.com/), a new foundation based on the idea that "we can no longer let billionaires control our digital public square." The announcement included a call for donations. As of March 5, Free our Feeds's GoFundMe [has raised $90K USD](https://www.gofundme.com/f/help-us-free-social-media-from-billionaires) -- not quite the four million they wanted, but certainly not nothing.

What would Free Our Feeds do? Well, for one thing, "re-grant [money] to the community of innovators," including folks doing content moderation. Another thing is to help develop an open protocol (namely ATProto, which is currently being developed by the Bluesky corporation). 

Right as this group made this announcement, a lot of folks asked a basic question: _doesn't this sort of thing already exist?_ They were referring, of course, to ActivityPub, which has existed since 2018 and is an open standard (governed by the W3C) with a thriving ecosystem of applications.

But there's another thing that existed at the time of the Free Our Feeds launch, an organization that was already innovating content moderation for the non-billionaire-controlled social web.

IFTAS.

Free Our Feeds does not mention the existence of IFTAS. (Initially, they didn't even mention ActivityPub, adding a note about that protocol in their FAQ later).

So, while Free Our Feeds seeks money for their  unclear goals (as [critics](https://tante.cc/2025/01/13/but-does-it-free-our-feeds/) [have argued](https://rubenerd.com/free-our-feeds/)), another organization that has actually achieved tangible things -- IFTAS -- is folding for lack of funding.

## Is This a Standards War?
Free Our Feeds eventually included a note about ActivityPub in their FAQ:
> ActivityPub is a W3C standard that enables interoperability between platforms like Mastodon, Flipboard, Ghost, Threads, and others. [ATProto] and ActivityPub should not be either/or options.

That answer also includes a link to [a blog post](https://socialwebfoundation.org/2025/01/13/free-our-feeds-and-algorithmic-pluralism/) by Mallory Knodel of the Social Web Foundation. That post explains, 
> [The Free Our Feeds] campaign is an opportunity to develop the capacity needed for the open social web protocols– ActivityPub along with Bluesky’s AT Protocol– to better interoperate, leveraging the entire open social ecosystem to create a working demonstration of algorithmic pluralism at scale.

The message is clear: It's not either/or. It's pluralism.

But is it?

The fact of the matter is that **there are now two standards** -- ATProto and ActivityPub -- making the **same fundamental claims to being _the_ open standard** that allows for decentralized social media. 

Another fact is that ATProto and ActivityPub are **architecturally very, very different.** The former is what [Christine Lemmer-Webber calls](https://dustycloud.org/blog/how-decentralized-is-bluesky/) a "shared heap" structure, where an installation requires access to all the posts in the network, while the latter is server software that sends and fetches messages as the necessity arises. ATProto allows for "Personal Data Servers" -- but these would rely on an infrastructure of indexes that likely will be prohibitively expensive. An ActivityPub server can run on a cheap server and still be a fully-fledged member of the fediverse.

Another fact is that **both are overseen by very different bodies** and **both have come from very different processes.** ActivityPub was developed at the W3C [largely independent of corporate interests](/2023/10/15/APnonStandard.html). The W3C remains the steward of ActivityPub. ATProto was born at Twitter and spun out into a separate, venture-capital funded corporation. While the Bluesky corporation [promised in 2023](https://docs.bsky.app/blog/protocol-roadmap) ATProto development will be shifted to the IETF, this still has not happened, and ATProto development is closely tied to a corporation that no doubt faces pressure to be profitable.

While there have been projects seeking to connect the two protocols -- such as Bridgy -- another fact is that this **bridging is incredibly clumsy.** To make a Mastodon account visible on Bluesky, one has to follow "@bsky.brid.gy@bsky.brid.gy", and then a _separate_ account is what is followed by Bluesky users. It works the same in reverse. Even when it works, posts are quite differently handled on either side. And none of this really addresses the fundamental architectural differences between ATProto and ActivityPub. Bridgy is a technical achievement, for sure, but I do not think it can be called "interoperability."

Thus, while Free Our Feeds has declared their interest in fostering interoperability and building resources that could benefit the decentralized social web, the facts are that **there are major organizational, cultural, and technical distinctions between these protocols** and **there are only so many resources to go around.**

In other words, it's possible we are watching a "standards war" happening in real time. It's not as apparent because the stakes are not the same as, for example, different railroad gauges or different ways to deliver electricity. 

But there are stakes. This is social media, where we have been taught that more is always better. Bluesky is attracting more people than the fediverse. This matters. Which standard would be recognized as the decentralized social media standard? Who will get the resources? Who will get developer energy, funding, academic research, and moderation support? Who will attract media coverage?

## IFTAS as Casualty in a Standards War
The case of IFTAS folding while Free Our Feeds emerges indicates that maybe AT Proto will win this potential standards war. If Free Our Feeds does raise the money for its (amorphous) goals, while IFTAS fails to get support for its actual services, that is pretty telling. 

If Free Our Feeds merely concentrates on what they believe is best for Bluesky -- as seems to be the case, given their interest in sorting algorithms, AI, and [blockchains](https://www.prnewswire.com/news-releases/who-owns-the-future-of-social-media-a-giant-leap-to-decentralize-core-components-of-blueskys-at-protocol-ecosystem-302387397.html) -- that is the most telling aspect of all.

Of course, it's possible IFTAS has failed to raise funds for good reasons. Non-profits can and do fail. (Free our Feeds also might!) 

But the failure of the broader tech, academic, and (frankly) celebrity sector to recognize and support an actually-existing trust and safety organization -- one tied closely to ActivityPub -- in favor of a relatively amorphous entity that is very tied to AT Proto is a troubling sign of how a potential standards war might turn out.

* Correction: I originally had this as the independent Fediverse Trust and Safety organization. The F stands for Federated, not fediverse.
