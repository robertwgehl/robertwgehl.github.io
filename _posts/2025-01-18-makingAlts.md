---
layout: post
author: RWG
title: 'Making Alternative Social Media in a Corporate Social Media World'
tag:
    - ASM update
    - Loops
    - ActivityPub
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 113851053746091520
---
In this week's [Alternative Social Media Update](/tags/asm update.html), I want to share two things that happened this week and have a fundamental connection: they both indicate the challenges alternative social media developers face when they make ASM in a corporate social media world.

<!-- more -->
## Item One: Algorithmic Choice

Writing on the W3C [Social Web Incubator Community Group](https://www.w3.org/community/socialcg/) email list, [Bob Wyman asks](https://lists.w3.org/Archives/Public/public-swicg/2025Jan/0016.html), "How would algorithmic choice' laws/regulations impact ActivityPub?" Wyman points to the Missouri Attorney General Bailey's [new regulation about "algorithmic freedom" for users of social media](https://ago.mo.gov/attorney-general-bailey-promulgates-regulation-securing-algorithmic-freedom-for-social-media-users/). In that press release, the AG says,

>Big Tech oligarchs have manipulated consumers’ social media feeds for their own purposes and exercised monopoly control over content moderation. To that end, I am invoking my authority under consumer protection law to ensure Missourians get to control the content they consume on social media.

While he notes this regulation will face implementation and legal challenges, Wyman nonetheless suggests that ActivityPub developers think seriously about new regulations that may affect them:

> I think we should anticipate that the coming
to power of Trump and MAGA Republicans is likely to spawn many such
proposals in the coming years. Given this, I think it would be useful to at
least consider what impact such regulations would have on Social Media
systems that rely on ActivityPub and ActivityStreams.

Wyman's message resonates with me, because I've already written about how regulations [might affect the fediverse](/2024/04/10/Online-Harms-Act.html). 

In a world where the vast majority of people are only familiar with corporate social media, any new regulations are going to likely be written in ways that can have unintended consequences for alternative social media. The idea of "algorithmic choice" is likely applicable to corporate services such as Instagram or TikTok. It's less clear how this idea would apply as a regulation of federated social media, which tends to eschew content sorting algorithms in favor of reverse-chronological ordering and boosting. _Requiring_ small, federated instances to implement alternative ways to sort streams would place a major burden on them.

Moreover, if alternative social media continues to grow, corporate social media may lobby to have laws written in such a way that they _purposely_ undermine small alternatives. After all, they have loads of money and power and lobbyists -- as we're seeing now with Meta's attempts to ingratiate itself with Trump, as well as with Musk's outright buying of Trump.

Finally, this Missouri AG regulation is clearly coming out of the right-wing "media is full of liberals" view. Consider this closing passage from the press release:

>“This is the first prong of a comprehensive offensive to protect free speech in 2025,” said Attorney General Bailey. “Now that we have a presidential administration coming into office that will not silence disfavored speech, we’re turning our focus to corporate censorship. Missouri will continue to lead the way in defense of our most fundamental freedoms.”

If that AG thinks Meta is left-leaning (and thus "silencing disfavored speech"), keep him away from much of the fediverse! It certainly "silences" the "freedom" of trolls and bigots. This raises a third scenario: regulations that are written specifically by lawmakers to crush independent social media if their values don't align with right-wing values (perhaps under the guise of protecting children or fighting terrorism).

## Item Two: Terms of Servitude?
Mark Zuckerberg is tripping over himself to bow down to Trump. The changes at Meta includes the end of fact-checking and [explicitly allowing people to harass queer folks](https://www.404media.co/its-total-chaos-internally-at-meta-right-now-employees-protest-zuckerbergs-anti-lgbtq-changes/). 

As a result, once again, folks are looking around for alternatives to corporate social media and there it sits: [Pixelfed](https://loops.video/) and [Loops.Video](https://loops.video/). Both are made by [Dan Supernault](https://dansup.com/). Pixelfed is an image-centric, ActivityPub-enabled service. That means that it is geared toward photographers who can share their pictures, but it also means that people on other fediverse systems, like Mastodon, can follow those photographers, see the pictures, and comment on them.

Loops is newer and under development -- and it's the one that prompted a controversy. Loops is meant to be a TikTok-like short video system that will also enable ActivityPub. While it's in beta, it has been growing at a pretty rapid clip.

Such growth invites scrutiny. A blog post by Phil has taken a [critical look at Loops.Video's terms of service](https://bajsicki.com/blog/loops-video-terms/) and the analysis is troubling. Here's a key bit of what Phil found: Loops.Video's TOS includes the paragraph,

> By posting your Contributions to any part of the Services or making Contributions accessible to the Services by linking your account from the Services to any of your social networking accounts, you automatically grant, and you represent and warrant that you have the right to grant, to us an unrestricted, unlimited, irrevocable, perpetual, non-exclusive, transferable, royalty-free, fully-paid, worldwide right, and license to host, use, copy, reproduce, disclose, sell, resell, publish, broadcast, retitle, archive, store, cache, publicly perform, publicly display, reformat, translate, transmit, excerpt (in whole or in part), and distribute such Contributions (including, without limitation, your image and voice) for any purpose, commercial, advertising, or otherwise, and to prepare derivative works of, or incorporate into other works, such Contributions, and grant and authorize sublicenses of the foregoing. The use and distribution may occur in any media formats and through any media channels.

(Note that Phil's post is absolutely accurate as of this writing -- I checked [Loops's TOS myself and saw this language](https://loops.video/legal/terms-of-service).)

If you're like me and you regularly read terms of service agreements, I pity you, but also you and I have seen this language many, many times before: this is the language of surveillance capitalism. I [wrote about this exact issue back in 2014](https://search.worldcat.org/title/882779130). Like so many corporations before it, Loops.Video is claiming the right to use your content basically forever and for whatever purposes it sees fit -- including selling your data to advertisers or training generative AI.

Is this a secret plot by Dan Supernault to bring surveillance capitalism to the predominantly non-capitalist fediverse? Maybe not. To his credit, when this was brought to Supernault's attention, [he said he'd fix it right away](https://mastodon.social/@dansup/113848396412970536):

> There have been several concerns raised about [these terms of service], and I want you to know that we will be replacing them with a better, more clearer set of rules and policies.<sup><a href="#note1">1</a></sup>

It turns out he used [Termly](https://termly.io/), an online resource to write terms of service agreements. "Please don't assume the worst," Supernault wrote. "I'm trying my best but don't have a team to help me with stuff like this." Basically, Supernault is saying that, in the absence of a legal team, in the heat of trying to spin up a new service, he went with a boilerplate solution to legal agreements. 

I anticipate Supernault will fix this -- after all, take a look at [Pixelfed.social's terms](https://pixelfed.social/site/terms). They are nothing like the Loops terms.

## Making ASM in a CSM World
The clash between the values of alternative social media and corporate social media go beyond things like avoiding surveillance capitalism or providing community-based governance and moderation. Increasingly, they will also involve how to manage state-based regulations and legal regimes. 

In the case of state regulation, like that of the Missouri AG in the USA, alternative social media developers will have to think about how new regulations will affect them -- and they may need to preemptively address them. And I'm not saying they should address them in code, but by advocating for ASM in front of regulators. 

In the case of terms of service, it would be good if organizations who support ASM would offer boilerplate terms that are not based on corporate logics and instead reflect fediverse values.

In both cases, making alternative social media in a corporate social media world means more work from communities: not just coding, not just self-governance, but also engaging with regulators and working with lawyers across jurisdictions. This work is already happening, of course, but I imagine more will need to be done.

## Notes
<p id="note1">1) Note that in almost all cases, I reach out to people on the fediverse to get permission to quote them outside of the fedi. In some cases, I do not think the consent is necessary. An example case is when a project leader makes a public statement about that project. I think this post falls under that exception.</p>
