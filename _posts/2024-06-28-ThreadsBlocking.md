---
layout: post
author: RWG
title: On Threads's Blocklist
tag:
    - Threads
    - Goal 2
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid:
---
Meta's Threads, which is slowly enabling ActivityPub capabilities, has just posted a [list of servers it is blocking](https://www.threads.net/moderated_servers). The list (as of this writng) has over 660 entries. Since I am finalizing a chapter on Threads for my [forthcoming book](/2024/02/11/Move-Slowy-Preview.html), I will definitely have to consider this list in detail. For now, I wanted to offer a few comments on this development, since it's a decidedly important moment in the ActivityPub-based fediverse.

<!-- more -->
## Meta is being transparent... sorta
I want to offer the most charitable take I can first: this public blocklist is one of the biggest moments of tranparency that Meta has ever engaged in. Maybe some of my academic colleagues who closely monitor Meta could correct me, but this strikes me as Meta offering quite a bit more insight into content moderation practices than they have in the past.

I think credit is due to the fediverse as a whole on this one, though. If Meta truly wishes to integrate with the fediverse, they have to follow the protocols, and I don't just mean ActivityPub -- they have to follow the [social protocols of transparent, open moderation](https://www.tandfonline.com/doi/full/10.1080/1369118X.2022.2147400). While typically this is in the form of simple, clear codes of conduct and open communication from moderators, posting a blocklist publicly a good step in the direction of transparency.

## This may be the first time millions see blocking in action
When I first started out on the ActivityPub-based fediverse back in early 2017, most Mastodon instances published their blocklists. Admins can still do this -- indeed, Mastodon.social, the largest server, [does (scroll down and click on "moderated servers")](https://mastodon.social/about).

However, over the past few years, many smaller servers stopped sharing this information publicly. Why? Well, it's obviously a vector for harassment. For example, if as an admin, I publicly say I block bad.instance, their friends could harass me with constant requests about why I did so, arguing that I need to change my mind. I have other stuff to do. Many admins just keep their blocklists to themselves.

So Threads is revealing something many of the millions of new fediverse members have not often seen: the fact that a healthy server _must_ block many others in order to moderate effectively. It's a fact of fediverse life.

This is a pretty radical change for Meta, to be honest: they now how to declare their relationship to the rest of the web, rather than just pretend that the web must flow through Meta properties.

## Blocking Nazis and nudity
Of course, transparency allows for scrutiny. We can take a look at the 660+ blocks and see what sort of values Meta adheres to.

First of all, there are a lot of instances on their list that I completely agree need to be blocked, including overtly white supremacist instances. I won't specify these, but if you look at the list, you'll see what I mean just from the URLs. There are also instances geared towards sharing sexualized cartoon images of children (a practice tolerated in Japan, but not by the rest of the fediverse). You can likely guess from those URLs, too.

However, multiple fediverse members have pointed out that Threads is blocking many queer and trans instances. While we'd have to dig in to figure out why, the most likely answer is that Meta has policies against nudity. Indeed, Meta's own Oversight Board found that [Meta is too aggressive in blocking nudity among LBTQ* users](https://gizmodo.com/instagram-meta-age-verification-system-ai-1849753822), including posts discussing top surgery.

In my interview with Mastodon founder Eugen Rochko, he saw such bans on consenting adult nudity as a very US-centric approach to global content moderation:

> [On the fediverse], there are thousands of other providers across the entire world, each giving a little bit of social space to the world, that is not controlled entirely from the US. And we know that US politics is not very stable – there’s a lot of turbulence. Trump was in charge, and that was not great for progressive laws.

> Some laws were passed, about 5 years ago, that affected a lot of sex workers – the SESTA and FOSTA bills – that basically erased sex work from social media because [so much] social media is based in the US. I think that’s not fair, because in Germany sex work is legal. Sex work _is_ work.

The Threads blocklist appears to be an extension of this logic: yet another attempt to moderate the globe from California.

Of course, if we think of Threads as another node on the fediverse, well... they can block whomever they wish for whatever reason. But the fact is, Meta is so large that if the rest of the fediverse tries to connect to it, we will defacto have US-based regulations on a highly localized, global network.

Indeed, Rochko's own Mastodon.social should probably be blocked by Threads, since it allows for pornography. In fact, several folks on the fediverse saw that Mastodon.social was blocked for 30 minutes, though it didn't seem to affect the connection.

Was that a mistake? Or a warning shot?

## You blocked what now?
Threads blocking white supremacists and loli comics strikes me as a fine choice. I don't agree at all with their blocking LGBTQ instances, but if they insist on blocking nudity, I suppose it makes some sense -- if only in a bland, shopping mall sort of way.

But some of their blocking choices make no sense to me.

For example, Threads blocks Scholar.social. An instance dedicated to acadmics, Scholar.social is one of the oldest Mastodon instances, and it has been a model of content moderation, safety for marginalized folks, and thoughtful federation practices. I know it very well because it was my home instance for several years. And when I shifted to being an admin of AoIR.social, we asked for permission to copy Scholar's code of conduct.

The only reason Threads offers for the block is Scholar "Violated our Community Guidelines or Terms of Use." I have no idea what this could mean. But the good news is, I know for a fact that Scholar would never federate with anything Meta, anyway, so I imagine their being blocked by Meta is a badge of honor!

Other confusing blocking choices that jump out to me are Kolektiva.social and Tabletop.social, two instances I also find to be well-moderated. Again, the justification is violated community guidelines. And, again, I don't think these servers care, since they are signatories to the [Anti-Threads Fedipact](https://fedipact.online/).

For the rest of us -- those of us who haven't been blocked by Meta -- take these arbitrary choices as a warning: if you attempt to federate with Threads, perhaps have a plan for when Threads blocks you and your members.

## Cross referencing ahoy!
Confusing decisions aside, it would be fascinating to cross-reference Threads's blocklist with shared blocklists, like the Bad Space, Oliphaunt's list, Sierdy's, and Garden Fence. I myself drew on these lists when we started AoIR.social. As I mentioned above, this is at least a bit of transparency from a Meta property -- we can learn a great deal about what they're thinking. But we can also learn what the broader fediverse values by comparing Meta's blocklist to those of other servers as well as shared lists.

As is clear from looking at the list, Meta continues to have a particular vision for global moderation. If you're looking to emulate Meta-style blocking, you can copy their list. If you reject Meta values, take a long hard look at their list and ask yourself if you should block the same servers.

If this were just any fediverse server, I don't think this blocklist would draw too much attention. But if it is an indication that this incredibly large, powerful social media corporation intends to reshape the fediverse in its image, and if they insist on blocking several well-moderated servers, it is a disturbing list -- not because of the choices they made that are right, but because of the arbitrary choices they make that simply get it wrong.
