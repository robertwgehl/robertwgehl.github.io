---
layout: post
author: RWG
title: 'Threads and the Failure of Global Content Moderation'
tag:
    - Threads
    - ASM update
    - moderation
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid:
---
This week's [Alternative Social Media Update](/tags/asm update.html) turned out to be more of a critique of corporate social media, specifically Meta's Threads.

It all started when I saw the news that Meta had [donated $1 million to Trump's inauguration fund](https://apnews.com/article/trump-meta-zuckerberg-inauguration-donation-c540bf7c638def11b8428e633965c718). Look, I'm an American. I know how this works -- the wealthy buy influence by giving to politicians. It's not particularly shocking to see Meta doing this -- it's part of their longstanding practices of lobbying those in power so they can continue to operate with little to no regulations. 

But it simply reaffirms my desire to explore the world of communication outside the control of a handful of corporations.

Searching for coverage of Meta's donation led me to a bit of a rabbit hole of recent news about Meta's Threads. Much of it comes from [The Verge](https://www.theverge.com/), and most of it is about Threads's moderation failures. 

Since Threads is slowly rolling out ActivityPub capabilities, this ASM Update about Threads does have a lot of relevance to the fediverse. 

The TL;DR version is: after taking a second look, I continue to see Meta's Threads as a bad actor and [worthy of being blocked](https://fedipact.online/) by the rest of the fediverse.

<!-- more -->

## Californian Ideology at Scale
Writing in the aforementioned _Verge_, [Adam Heath reports](https://fedipact.online/) that Meta is now double-thinking their previous moderation practices. The story is nominally about how Meta was overactive in moderating during the COVID pandemic (though Meta blames Biden for that) as well as about how Meta's automated moderation systems are too "ham-fisted."

But the real problem is not explicitly stated. See if you can find it:

> Nick Clegg, Meta’s president of global affairs, told reporters on Monday that the company’s moderation “error rates are still too high” and pledged to “improve the precision and accuracy with which we act on our rules.”

You're probably thinking I'm going to critique the fact that Meta hired Nick Clegg, but as I said, I'm an American, so I know little of him other than he helped raise tuition fees in the UK and helped preside over Brexit.

No, my issue is with the title "president of global affairs." 

I find it inconceivable that any corporation can engage in content moderation on a global scale. This is particularly apparent to me after experiencing the fediverse, where content moderation is achieved at a local level on a small scale. Meta, X, TikTok: all attempt to impose their corporate standards on all the world. Perhaps we can come up with global standards and ethics -- but the vehicle for doing it won't be through top-down, for-profit corporate behemoths.

## Too Big to Comprehend
As a result of attempting the impossible task of moderating the globe, Meta has grown to be huge and complex. It's so big we need dedicated watchdogs. We need [investigative journalists](https://www.theverge.com/2024/10/9/24266096/instagram-threads-moderation-account-post-deleted-limited) to report on trends in corporate social media, including trends about poor moderation.

Indeed, Meta is so big that its own executives don't know what's going on. Consider this exchange on Threads:

> Social media consultant Matt Navarra — who was notified his Threads account is getting downranked after sharing a story about how Tom Brady fell for a Meta AI hoax — got a response to his public complaint from Mosseri. “Looking into it...” Mosseri said. Meta didn’t immediately respond to a request for comment on the issues. 

If the system is so opaque the head of Instagram/Threads, Adam Mosseri, can't figure it out... well.

Again, contrast this with the fediverse. On my previous instance, if I had a problem, I could contact the admin directly. I didn't need to post publicly and hope the admin saw it. (On my current instance, AoIR.social, I _am_ the admin, so people contact me for help.) The fediverse, at its best, is a far less abstracted, human system.

## Bots can't Moderate

Speaking of humans, Meta is [increasingly using bots to moderate](https://www.facebook.com/help/1584908458516247/). Unsurprisingly, this results in arbitrary decisions. 

That's the main complaint of posts tagged ["Threads Moderation Failures,"](https://www.threads.net/@mikethebearded/post/DA2D_C4yaya) which has been steadily documenting the weird and wild world of AI-based content moderation. For a corporation already incapable of understanding what its own moderation practices are ("I'll look into it!"), ceding more and more moderation decisions to AI seems like a bad choice.

We could ask Meta hire more humans to do the job, but then again... some of the last humans who did that work were summarily [fired after trying to unionize](https://jacobin.com/2024/02/kenya-courts-meta-content-moderation-union).

## Your Voice, Our Vote
But perhaps all of this will be made right once Thread users have their voices heard via a [survey on content moderation](https://www.threads.net/@oncescuradu/post/DDfgI0_o_3Y). Since Meta attempts to moderate a global scale, perhaps getting tons of input from its users might shed light on how to tackle that task. The survey appears to ask about users' attitudes towards sharing on Threads -- whether or not they feel inhibited from sharing because they fear being "penalized." 

Maybe Threads will learn from the survey and improve their moderation? 

I have my doubts. I've seen Facebook/Meta do this sort of faux popular polling throughout its history. As [I wrote back in the early 2010s](https://archive.org/details/UnlikeUs/page/n223/mode/2up), Facebook often held votes on changes to their Terms of Service agreements and, no matter the vote, they adopted the TOS they intended to the whole time. 

Might they do the same with their Threads content moderation survey? Who knows? Their content moderation decisions are so opaque that it would be impossible to tell, anyway. I believe the real goal is to keep their metaphorical shopping mall aesthetic intact, and to keep regulators at bay. And probably to justify their cost-cutting AI-based moderation practices.

## You Block Me? No way, man. No, way. I block you!
All of the above has renewed my belief that AoIR.social's decision to preemptively block Threads (and sign [the fedipact](https://fedipact.online/)) was the right decision. AoIR.social is a Mastodon instance I help run. We provide federated social media to members of the [Association of Internet Researchers](https://aoir.org/), a group of folks who have a pretty good idea about how Meta operates.

But I am a bit disappointed our block isn't mutual. Readers might recall I wrote about Threads's Fediverse Blocklist -- their own list of blocked servers. I first looked at it [six months ago](/2024/06/28/ThreadsBlocking.html). I checked it again today -- it has grown from 660 back in June to 843 today. 

As I wrote back in June, many of the blocks make total sense. But some don't. I mentioned Scholar.social as one that does not need to be blocked. Another one that's been blocked this whole time is Writeout.ink, which is a small server with a clear code of conduct.

Another one that doesn't -- and was added to the list between June and now -- is Darius Kazemi's Friend.camp, the flagship Hometown server. The reason Threads's blocklist offers is "no public timeline." I asked Darius about it, and he says that's true, but he thinks it's been true for some time now.

And surely there are many many more servers without public timelines than 800. So why is Friend.camp blocked? Maybe it's because Friend.camp blocks Threads. "We federated with threads for a long time but we defederated a few months ago based on user consensus," Darius told me. So maybe blocking Threads triggered a mutual block? 

But... AoIR.social blocks Threads! And we're not on the list! What do I have to do to get AoIR.social blocked by Threads? I kinda want that badge of honor.

In all seriousness, while I praised Threads for publicly posting its blocklist, noting this is a very transparent move, it's still pretty opaque how they're making these choices. Just as Threads is being criticized by its users for clumsy AI-based moderation decisions, I anticipate Threads will automatically and arbitrarily block a fediverse server that does not deserve it but whose members really do want to connect to folks on Threads. I don't see Threads putting a lot of effort into making informed blocking decisions. That's not what Meta does. And for those instances that want to federate with Meta, be prepared to behave how Meta says -- and even if you do, you may be arbitrarily blocked. And be prepared to [fill out a form and hope](https://help.instagram.com/contact/1574148669814359/) that someone, somewhere considers your case.

If people are going to use blocklists -- and [I think they should](/2023/09/20/blocklists.html) -- they need to be managed by people on behalf of coherent communities. Not by robots on behalf of a profit-seeking corporation. And they need to be documents that networks of communities gather around to discuss how to build out a federated network. Not dictated to the network by a powerful node.
