---
layout: post
author: RWG
title: The Fediverse = Pleroma?
tag:
    - Pleroma

comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid:
---

Many people lament the conflation of "fediverse" with "Mastodon."

Because Mastodon is by far the most populated ActivityPub application, many people talk about it as if it is the entire fediverse.

This isnt' the end of the world. Christine and Morgan Lemmer-Webber observed it's a bit like the 2000s conflation of Ubuntu with Linux -- back then, Ubuntu *was* Linux to many casual Linux users. Think about it now -- I don't think that conflation still holds. But Ubuntu did a bit of a service by boosting Linux in popular arenas. Mastodon is arguably doing the same for the fediverse.

However, there is at least one domain where the fediverse is not conflated with Mastodon.

Instead, it's conflated with... Pleroma.

That domain is a growing corpus of computer science papers. And this literature's conflation of Pleroma with the fediverse is, in my view, much worse than the popular conflation of Mastodon with the fediverse.

<!-- more -->

## The Papers

In order to critique something, you've gotta read it. So here let me show the citations and offer short summaries, and then I will talk about why the conflation is happening in the papers and why it's so problematic. I'm adding them here in chronological order by publication date, since (as you will see), the articles share many of the same authors and all cite each other in a self-reinforcing tautology.

### Hassan, Anaobi Ishaku, Aravindh Raman, Ignacio Castro, and Gareth Tyson. “The Impact of Capitol Hill on Pleroma: The Case for Decentralised Moderation.” In Proceedings of the CoNEXT Student Workshop, 1–2. New York, NY, USA: Association for Computing Machinery, 2021. https://doi.org/10.1145/3488658.3493780.

As the authors write, "this paper explores the challenge of content moderation in" the fediverse. They start by noting a variety of fediverse systems -- Pleroma, Mastodon, PeerTube, Hubzilla. They go on to describe things like instances and federation.

So far, so good.

But there's a problem, they note. They cite Bevensee (who was writing about a wide range of peer to peer systems, from chat to Secure Scuttlebutt) to argue that white supremacists have turned to the fediverse. And of course, there are white supremacists all over the fediverse.

Then, they argue “administrators are often volunteers with limited resources, and federation means that content generated on one instance may be pulled to another instance (with different moderation policies).”

Add it all up, and we need better moderation tools.

Now, all of this ignores the moderation tools described in Bevensee, which discusses the ways in which Gab was isolated by the rest of Mastodon. Instead, Hassan et al are invested in a vision of the fediverse where moderators are totally overwhelmed by streams of hate content.

And the dataset they draw on to illustrate this? “Policy data” and “post content” from ~700 Pleroma instances. They then focus on 12 Pleroma instances that gained posts and users after the Capitol Riots in the USA in January of 2021. And their list of 12 includes exactly what you’d expect under these conditions:

- kiwifarms.cc
- freespeechextremist.com
- shitposter.club

And a few more notorious instances.

They then find that other Pleroma instances don’t seem to engage in much blocking of the 12 in their dataset. This leads to their big takeaway:

> “There are a number of reasons for this seemingly slow response. One could be the voluntary nature of content moderation while another could be that administrators wait and take these actions in batches. In either case, this motivates the need for new technologies to assist administrators in content moderation.”

They offer this instead of the obvious: Pleroma is dominated by free speech absolutists and thus trolls.

But this paper establishes their case: because we have some data with some hate speech in it, and because that data comes from a tiny slice (Pleroma) of the fediverse -- which is run by hapless volunteers and is subject to unfettered spread of content -- we need “new technologies.”

The table is set for the next paper...

### Bin Zia, Haris, Aravindh Raman, Ignacio Castro, Ishaku Hassan Anaobi, Emiliano De Cristofaro, Nishanth Sastry, and Gareth Tyson. “Toxicity in the Decentralized Web and the Potential for Model Sharing.” Proceedings of the ACM on Measurement and Analysis of Computing Systems 6, no. 2 (June 6, 2022): 35:1-35:25. https://doi.org/10.1145/3530901.

This paper will go on to offer some of the automated tools they claim the fediverse (or, as they say, "decentralized web") desperately needs.

This paper's central research questions are:

> (i) How much toxicity exists in the [Decentralized Web, their term for fediverse]? (ii) How does toxic material spread across DW instances via federation? (iii) Is it possible for DW instances to train their own automated classification models to reduce the manual load on administrators? And (iv) How can administrators cooperate to improve content moderation and reduce their workload?”

They again suggest that content spreads rapidly and out-of-control across the fediverse:

> A recent example of this occurred when the gab.social instance joined the Fediverse, rapidly spreading hate speech to other instances

But! Let's look at their citation for this. It's [this paper, presented at a conference in 2018](https://experts.illinois.edu/en/publications/what-is-gab-a-bastion-of-free-speech-or-an-alt-right-echo-chamber). And if you know your fediverse history, you would know Gab hadn't adopted ActivityPub at that point -- it adopted [ActivityPub in 2019](https://blog.joinmastodon.org/2019/07/statement-on-gabs-fork-of-mastodon/).

But no matter. There's toxicity afoot! And since the previous paper helped establish that there are some toxic Pleroma instances out there, let's focus on them. They zero in on 30 Pleroma instances, pulling 9.9 million "toots" (their word, not mine) from them.

The instances they pulled posts from are pretty notable: shitposter.club, neckbeard.xyz, djsumdog.com, my.dirtyhobby.xyz (this last one being a porn-focused instance).

And they insist that Pleroma is a major part of the fediverse. Check out the subtleties here:

> Pleroma is a DW open source microblogging service that runs in the Fediverse and the largest decentralised social platform (next to Mastodon).

They support this by... [self-citing a paper their team wrote about Mastodon](https://doi.org/10.1145/3355369.3355572), which didn't really establish anything about Pleroma.

But again, no matter, we now have a major part of the fediverse (Pleroma) full of toxic content. Based on their analysis of 30 Pleroma instances:

> “We confirm that extensive toxic content is present in the [fediverse]. We identify 12.15% of all toots as toxic. Furthermore, we show that toxic content does spread across Pleroma: 26 out of the 30 instances receive an average of at least 105K remote toxic toots through federation.”

They find this by running the posts they gathered through Google's Jigsaw Perspective API:

> “For a given toot, Perspective returns a score (between 0 and 1) for its toxicity. This offers an estimate of the fraction of human moderators who would label the content as toxic. Following, we consider a toot to be toxic if its toxicity score is greater than 0.5 (and vice versa)”

They note, again, that there's *no way* to prevent the toxicity from blasting across the network:

> “Preventing the spread of toxic content with this dense and complex instance interconnectivity is challenging due to the ability for content to spread across the federated links.”

(They repeatedly ignore blocking as a key technique.)

Thus, we're off to the races to get to their conclusion, which is an automated tool for content moderation on the Pleromiverse -- I mean, fediverse. They introduce ModPair, a way for people to annotate toxic toots, thus training a model that can be shared across instances.


### Anaobi, Ishaku Hassan, Aravindh Raman, Ignacio Castro, Haris Bin Zia, Dami Ibosiola, and Gareth Tyson. “Will Admins Cope? Decentralized Moderation in the Fediverse.” In Proceedings of the ACM Web Conference 2023, 3109–20, 2023. https://doi.org/10.1145/3543507.3583487.

Note that the title is about “Moderation in the Fediverse,” so we’re cued to think about the entire fediverse as we read this. The paper cites the Musk takeover and notes that it has led to people shifting to “Pleroma or Mastodon.” They note that admins of these instances may face a growing burden due to the growth of the fediverse, which is a fine point.

“We observe a diversity of administrator strategies, with evidence that administrators on larger instances struggle to find sufficient resources. We then propose a tool, WatchGen, to semi-automate the process.”

And there's the red flag: the large instances have trouble precisely because they are large. But the implication here is that *everyone* wants their instance to be large (and thus will need tools, like WatchGenTM).

They do another self-citation, this time to Bin Zia et al 2022, to re-hash their claim that toxic content is just blasting all over the network.








### Nobre, Gabriel P., Carlos H. G. Ferreira, and Jussara M. Almeida. “More of the Same? A Study of Images Shared on Mastodon’s Federated Timeline.” In Social Informatics, 181–95. Springer, Cham, 2022. https://doi.org/10.1007/978-3-031-19097-1_11.


https://arxiv.org/pdf/2302.05915.pdf
https://doi.org/10.1145/3488658.3493780
https://doi.org/10.1145/3530901



Imagine going to a free speech absolutist instance and offering an automated tool to moderate based on hate speech terms from an academic database, or on "toxicity scores" from a Google algorithm. Yeah, they won't do it, or they'll hijack it to target marginalized people.

Imagine taking the same tool to a Code of Conduct-moderated instance -- all you have to do is run the tool, though for it to be effective, you will have to draw in a bunch of extra posts, likely from instances you've already blocked. Also an obvious no-go.

And none of this addresses the fact that automated moderation has no bearing on actual moderation practices.

I'm not sure why they conflate Pleroma with Mastodon. Does Pleroma use the Mastodon API?
