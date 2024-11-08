---
layout: post
author: RWG
title: 'York Circle Lecture: Fleeing Facebook and Exiting X'
tag:
    - goal 2
    - presentations
    - journalism
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 113431216882331888
---

Yesterday, I gave a presentation at York University in Toronto as part of their York Circle program. The audience was comprised of York alumni.

My presentation was "Fleeing Facebook and Exiting X: How activists show the path away from corporate social media." Here's the abstract:

> The purchase of Twitter by Elon Musk in 2022, coupled with Meta's blocking of Canadian news sites, has prompted people in Canada to consider their social media options. Social media has now fragmented, with a small but growing population of people turning to non-corporate, alternative social media, such as Mastodon and the fediverse. This talk will discuss how non-corporate, alternative social media provide Canadians not just with a path away from Facebook or X, but also provide a new way to engage in online democracy.

If that sounds interesting, well... read on! This is a version of that presentation, edited into blog form. (Note: this is another long post.)

<!-- more -->

## Acknowledgements

Before I get too far, I want to acknowledge a couple things. First, this research has been supported thanks in part to funding from the Canada First Research Excellence Fund.

Second, some of what I'm going to talk about comes from a collaboration between myself and Alex Martin, who is a PhD student here at York in the Science and Technology Studies program.

## Introduction: News and Social Media in Canada

Let's start this conversation about social media in Regina, Saskatchewan. Specifically, let's talk about what could be the top news company in Regina. It is, arguably, a garbage company.

According to [*Canadaland*](https://www.canadaland.com/podcast/1042-the-city-that-gets-its-news-from-a-dumpster-company/), the most trafficked news site for Regina
residents is a Facebook page run by Just Bins, a garbage can company. (I also should credit *Canadaland* another way -- I kind of stole this intro from them!)

In fact, the Just Bins Facebook page won a "best of" award for news in Regina.

This isn't to say there is no local paper. But the local paper, the *Regina Leader Post*, is seeing dramatic drops in circulation and no longer prints the paper locally.

That news reporting in Canada is in a crisis is not new, but it is certainly getting worse. Layoffs abound.

One major issue has been Meta. Because of the [Online News Act](https://www.canada.ca/en/canadian-heritage/services/online-news.html), Meta has now refused to let people link to Canadian news in Facebook and Instagram. This is in part what led to Just Bins Facebook page being able to become the top news site in Regina. As Jesse Brown of *Canadaland* said, "It appalls me that \[Just Bins\] can build a massive audience specifically because \[it's\] not news. I can't publish to Facebook, and \[they\] can *because* \[it's\] not news."

Regardless of how you feel about the Online News Act, it is coming from the recognition that a handful of media corporations have too much power over Canadian news. Let me put this a different way. Another, albeit different case in point: Elon Musk's X. Unlike Meta, news organizations are certainly welcome on X. But at what price? As [multiple](https://www.disinfo.eu/publications/disinformation-on-x/) [studies](https://www.isi.edu/news/55932/new-twitter-now-with-more-hate/) and [news reports](https://www.pbs.org/newshour/show/musk-lashes-out-at-advertisers-leaving-x-over-rise-in-hate-speech) are finding, disinformation, trolling, and harassment are on the rise on X. And often the disinformation and trolling comes from the top, such as when Musk labeled the CBC as ["69% government funded"](https://www.businessinsider.com/cbc-twitter-label-69-government-funded-media-elon-musk-2023-4).

## Where do we go?
Meta and X have me wondering: Where do we go if we want to leave Facebook or X?

What about TikTok? LinkedIn? Reddit? Maybe. But all of these share in the same basic problem: they are all social media that is controlled by for-profit companies that, at the end of the day, make their money by monitoring our lives. They can be bought and sold.

I've been researching this question -- where do we go? -- for my entire academic career, from my days as a PhD student in the 2000s to the writing of my first book, *[Reverse Engineering Social Media](https://tupress.temple.edu/books/reverse-engineering-social-media)* in 2014 to today, when I am finalizing my fourth book, *Move Slowly and Build Bridges*, for Oxford. (For more on my academic career, [see this post](/2024/10/18/GMUpresentation.html))

The answer to the "where do we go?" question has been given for many, many years by people I have been calling "critical reverse engineers." These are activists who take apart corporate social media -- Facebook, Instagram, Twitter/X, YouTube -- to make something better. I have interviewed dozens of these critical reverse engineers, studied the code and interfaces of the systems they've built, and have even operated some of the social media they've created.

It turns out that quite a few of these critical reverse engineers are right here in Canada.

Let me say a bit more about critical reverse engineering. And to do that, I should talk quickly about reverse engineering in general.

Basically, reverse engineering is forward engineering in reverse. Rather than starting with plans and them implementing them in material objects, reverse engineers start with the material object and seek to figure out how it works, often discovering clues about the creators' intentions.

Reverse engineers do this work for a range of purposes. It might be to make a competing project -- a famous example here is the reverse engineering of the IBM PC in the 1980s. Or it might be for military purposes, reverse engineering captured equipment -- a famous case is that of the Russian Tu-4 bomber, which was a reverse engineered US B-29.

Now, these aren't particularly critical. I'm using "critical" in the sense of critical theory -- the examination of power in society, with the goal of making a more just and ethical society.

And I think that social media admits to critical inquiry. Social media has had a major impact on how we live our lives. We can talk about the benefits of social media. It has been used by social justice movements (Idle No More, Me Too, Black Lives Matter). There's the simple pleasures of sharing and connection. And there's local and global news sharing. And we can also talk about its harms: Facebook’s emotional contagion experiments. The Cambridge Analytica scandal. Gamergate harassment on Twitter. And concerns over mental health, particularly of teens.

There's a lot at stake when we consider social media. So, let's consider reverse engineering social media, but not just to make competing products. I am interested in activists who are reverse engineering social media to create systems that are better than the corporate versions -- alternatives that are under our control, that push away some of the negative aspects of corporate social media away in favor of more beneficial aspects. I have been studying projects that produce new innovations in social media outside of the predominantly Silicon Valley model.

## The fediverse, innovations, and Canada

Specifically, I will highlight the fediverse -- social media that is comprised of thousands of small community-run social media sites linked together in a global network. As a project that critically reverse engineers corporate social media, the fediverse brings about many innovations.

I will talk about four such innovations:
- a new topology
- no surveillance capitalism
- ecological innovations
- online democracy

## A New Topology: Noncentralized

I argue the fediverse provides a new way of doing social media, one that's not centralized or concentrated.

I say new, but really what I'm going to say is quite similar to email. Email is federated. If I have an account on Protonmail, and a friend has an account on Gmail, and another runs their own server using Roundcube software, we can all still contact each other. We can do so in spite of the fact that all three are provided by different organizations in different locations.

This is because email runs on a shared, standardized protocol called Send Mail Transfer Protocol, or SMTP. SMTP dates back to the early 1980s.

Much more recently, critical reverse engineers have created a social media protocol that works much like email, but for social data. It works like this. Let's say I'm using a system called PeerTube, which is a video-sharing service. I can connect to someone using Pixelfed, which is an image-sharing service. And that person can connect to someone on a Mastodon server, which is a Twitter-like system. And so on.

This is possible because of a new standard called [ActivityPub](https://www.w3.org/TR/activitypub/), which, a bit like email, presents social data in the form of inboxes and outboxes. The ActivityPub protocol was authored by Christine Lemmer-Webber, Jessica Tallon, Erin Shepherd, Amy Guy, and Evan Prodromou. Here's a Canadian connection! Evan Prodromou, who has been actively working on social media alternative since the late 2000s, is a Canadian. Thanks to Prodromou, Lemmer-Webber, and the rest of the creators of this protocol, we now have a global network of interconnected social media servers.

And, as a testament to their engineering feat, consider the fact that the ActivityPub-based fediverse was able to absorb a [massive wave of new users happening in late 2022](https://www.theguardian.com/news/datablog/2023/jan/08/elon-musk-drove-more-than-a-million-people-to-mastodon-but-many-arent-sticking-around) -- that is, right when Musk finalized his purchase of Twitter.

The upsides of this noncentralized system are twofold. For one, it's less vulnerable to being simply taken over (e.g., as in the case of Twitter/X). Second, it is open to many groups participating in running their own social media.

## No Surveillance Capitalism

As for the refusal to engage in surveillance capitalism, consider [Mstdn.ca](https://mstdn.ca/explore), a Mastodon server that provides Twitter-like features
to Canadians.

If you're considering joining Mstdn.ca, you might notice that they ask for donations. Why? Well, they don't sell advertising space. Unlike corporate social media, which is in the business of selling our attention to advertisers, Mstdn.ca does not sell user data. This is typical of the rest of the fediverse.

In my study of Mastodon and the rest of the fediverse, I've found that the vast majority of instances use donations or other mutual aid-style approaches to funding. They use a variety of nonprofit organizational structures, from informal to formal. And Mastodon and fediverse software do not include the tools needed to do targeted, surveillance-based advertising.

There are some possible upsides here. Since people cannot buy advertising space, there's far less incentive to promote outrageous, attention-grabbing posts. Moreover, current disinformation practices rely in part on the ability to buy targeted advertisements -- you can do that on Facebook and Youtube, but you cannot do that on the fediverse.

I should note I say "possible" because I think it is early to tell if these advantages will play out. However, in my interviews with fediverse users, they do report that they have a calmer experience on the fediverse. In addition, I am part of a group of researchers monitoring the fediverse for disinformation -- a big concern as we head into a US presidential election -- and so far, so good on that front.

## Ecological innovations

On to ecological innovations. The brute fact is that, in spite of the promise that digital media will be light and airy, digital media is having a massive impact on the climate. Social media data centers -- and the turn to generative AI -- are [straining energy systems](https://direct.mit.edu/glep/article/24/2/9/120588/Generative-AI-and-Social-Media-May-Exacerbate-the). And data centers are [notorious for their demands for drinking water](https://www.washingtonpost.com/climate-environment/2023/04/25/data-centers-drought-water-use/). Speaking as someone who has lived in both the US and Canadian Rockies, this is a major concern of mine.

Let's say people leave behind X and Facebook for the fediverse. Will the fediverse replicate these issues? Not necessarily. Because the fediverse is community-run, it is possible for groups to experiment with it to reduce its energy and water demands.

Consider the work of [Anne Pasek of Trent University](https://www.trentu.ca/culturalstudies/faculty-research/undergraduate-faculty/anne-pasek). Anne and her colleagues are developing solar-powered fediverse social media.

This isn't far-fetched. A few years ago, an online publication called [Low Tech Magazine](https://solar.lowtechmagazine.com/) demonstrated that it is possible for a website to be powered by a small solar panel. Likewise, Pasek and her colleagues are working on powering a fediverse server with a small, consumer-grade solar panel.

This is experimental. Time will tell if it works. But if projects like Anne's are successful, we could see a reduction in the carbon footprint of social media.

In addition, I can say that there are some clear ecological benefits to the fediverse when we compare it to corporate social media. I mentioned previously that the fediverse avoids surveillance capitalism. This does mean that, right out of the box, the fediverse should have less ecological impact than corporate social media, since it does not require the infrastructure of behavioral advertising.

## Online Democracy

Finally, let's talk online democracy. Here I'd point to [Cosocial.ca](https://cosocial.ca/explore). This is a social media site run by Canadian cooperative organization. As a collective, Cosocial members have developed their own, [local moderation rules](https://cosocial.ca/about).

Here's a sampling of their code:

- "Treat all persons fairly and with respect, courtesy and dignity.
- Be sensitive to cultural and social differences and practices.
- Be careful in your use of language that may be disrespectful or demeaning."
- They also have prohibitions against racism, transphobia, and violence.

This can work because Cosocial is not large -- it has 100 active members. It's much easier to have such a code of conduct for a small number of folks.

So, you might think: 100 people? That's not a lot. That's nothing compared to corporate social media!

But Cosocial isn't alone. Cosocial can connect to another Canadian instance, [Ottawa.place](https://ottawa.place/about). Like Cosocial, Ottawa.place has a code of conduct with similar values. So those two can connect without clashing about their ethical values.

And Cosocial and Ottawa.place can connect to another instance, [Scholar.social](https://scholar.social/about). Scholar.social is a well-moderated, large instance run by a person in Montreal. Like the others, Scholar.social has a similar code of conduct. And all these servers can connect to others in Canada.

But this isn't just in Canada. These servers can connect others located around the world, forming a global network. And if they connect to other servers with similar codes of conduct, we see an emergent set of ethical values. This network of servers share a commitment to active moderation, not only against racism or transphobia, but also against disinformation. Studies are showing that there is a shared set of ethical values across much of the fediverse. I think this is most exciting aspect.

This is a structure a co-author and I call "[the covenantal fediverse](https://www.tandfonline.com/doi/full/10.1080/1369118X.2022.2147400)": a global network of ethically-aligned digital communities.

Here, we get the benefits of locally-run and moderated systems, but with the reach of a global network.

## But What About News in Canada?

But what about news? I started out with a note about the sorry state     of news in Canada -- including a discussion about social media's role in news sharing. Can Canadians share and receive news on federated, non-corporate social media?

This is an area Alex Martin, a PhD student, is working on. The short answer is: yes, Canadians can share and are sharing news on the fediverse.

Alex has taken the lead in a research project where we interview Canadians who are running or using federated social media. A big question Alex is asking: are Canadians sharing news on the fediverse? And what sorts of news are they sharing?

We're hearing Canadians across the country note that the fediverse has become a viable source of breaking news. This includes local happenings as well as global events. And we're also discovering people and groups who recognize this and want to make local federated social media so that people can share news.

What about news organizations? This is emerging, too, albeit a bit slower. [The Tyee](https://mstdn.ca/@thetyee), [Conversation Canada](https://flipboard.com/@ConversationCA), [The Narwhal](https://mstdn.ca/@thenarwhal), [Livewire Calgary](https://mastodon.social/@livewirecalgary), and [a host of journalists](https://medium.com/@marilync/canadian-journalism-on-mastodon-15eeb4f5b9df) are posting to the fediverse.

I think there really ought to be more. In addition, both [Fen McKelvey of Concordia University and I](https://theconversation.com/canadas-public-broadcaster-should-use-mastodon-to-provide-a-social-media-service-194116) have argued the CBC should set up their own presence on the fediverse. They could establish a server and provide their journalists with accounts. Those journalists could post to the network and have global reach while at the same time being on a server run under CBC standards -- not under the standards of Elon Musk.

Were the CBC to start their own fediverse server, they wouldn't be alone. Globally, there are public news organizations starting to operate their own fediverse servers -- most notably, the BBC has experimented with [its own Mastodon server](https://theconversation.com/canadas-public-broadcaster-should-use-mastodon-to-provide-a-social-media-service-194116).

## Conclusion
The fediverse has a great deal of potential for Canadian social media:

-   Canadians are, right now, running their own social media
            outside of the dominant Silicon Valley systems.
-   They can moderate and govern themselves locally, and yet
            have access not only to the rest of Canada but the rest of
            the world
-   They can experiment with solutions to the climate crisis
-   They can stave off the privacy violations of surveillance
            capitalism
-   And they can share both local and global news

In other words, Canadians are doing the work of critically reverse engineering social media, and are showing folks a            possible path away from X or Facebook.

This isn't to say that the fediverse is a flawless system. I present plenty of criticisms of it in my book. But given the growing set of problems posed not just in Canada, but globally, but corporate social media, I believe serious scholarship that highlights the fediverse and critical reverse engineering is needed.

Incidentally, if you're Canadian and want to try the fediverse, here are a couple options to look at. [Mstdn.ca is open for registrations](https://mstdn.ca/auth/sign_up). Or, if you want a more regional/localized instance, the [Mastodon Server
site](https://mastodonserver.ca/) has a list.
