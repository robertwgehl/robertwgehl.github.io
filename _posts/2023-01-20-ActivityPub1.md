---
layout: post
author: RWG
title: Reading the Minutes of the Social Web Working Group, part 1
tag:
    - Goal 2
    - ActivityPub

comments: 
  show: true
  fedihost: scholar.social
  fediusername: robertwgehl
  fediid: 109723434611493654
---

_NB: This is the first in a series of posts where I will share my notes on my readings of the minutes of the Social Web Working Group. Future posts to come._

As readers of the blog know by now, Goal 2 of the blog is [to document my writing of my next book](/2022/01/06/Goal2.html), which I'm tentatively titling _Move Slowly and Build Bridges: Mastodon and the Struggle for Ethical Alternative Social Media_.

To that end, I have been studying the workings of the [Social Web Working Group](https://www.w3.org/Social/WG) (SocialWG), a W3C standards group which ran from 2014 through 2017 and ultimately produced, among other things, [ActivityPub](https://www.w3.org/TR/activitypub/), the protocol that underpins much of the fediverse.

I figure I cannot tell any stories about Mastodon without understanding the production of ActivityPub. Looking through the SocialWG meetings, it's quite clear that Mastodon and ActivityPub's histories are deeply intertwined. Mastodon adopted ActivityPub it prior to AP being a Candidate Recommendation (the penultimate stage in the W3C recommendation process). Mastodon is also a key reason why the Social Web Working Group got a 6 month extension for their work in 2017 -- see [this meeting](https://www.w3.org/wiki/Socialwg/2017-06-27-minutes). They even set up a Mastodon instance (w3c.social) to show W3C members that software.

This post will discuss the early period of the SocialWG (circa 2014 through 2015). I'll follow up later with more posts and notes.

Importantly, I need to offer a couple caveats.

First, I didn't participate in the group. Instead, I'm basing much of this off the meeting minutes, as well as blog posts by SocialWG members, and to a lesser extent on informal discussions and formal interviews with some of the members. It's possible -- likely, even -- that I will get details wrong, not simply because I wasn't there, but also because this poor English major was not trained in computer science. The notes here are things that caught my eye. If you have corrections or critiques of my interpretation, please do share in the comments! And, as I talk to more people, I might change my interpretations, as well.

Second, my focus is predominantly going to be on ActivityPub. However, the SocialWG produced quite a few other standards. That said, in focusing on the group's history, I should cover a lot of ground, even with my emphasis on ActivityPub.

Third, the meeting minutes are not verbatim transcripts (which makes sense – meeting minutes almost never are). They were taken by volunteers from among the SocialWG, who were trying to transcribe phone conversations while an IRC chat was going. So, any quotes I include here should not be taken as verbatim statements. In addition, given the sheer number of times I read statements such as "who's speaking now?" and "I can hear weird noises" – these were largely telephone conferences, after all – I would take any attributions here with a major grain of salt, as well. Take, for example, the following exchange from [this meeting](https://www.w3.org/wiki/Socialwg/2015-02-17-minutes):
> harry: so a cheapo understanding of heirarchy

> ... am confused when I read the spec

> scribe: was that harry or dret ?

> sorry if I set the wrong one

> dret: me

Notice in this example statements are attributed to harry when they were actually said by dret. So, I will tend to cite statements and ideas with minimal attribution unless I am 99% certain the statement can be attributed to the person.

Let's dive in!

<!-- more -->

## Part 1: Getting Started, Getting Organized (2014 to end of 2015)

### The Charter

The first phase of a Working Group at the W3C is a Charter, and the Social Web Working Group is no exception. [Their charter](https://www.w3.org/2013/socialweb/social-wg-charter.html) stated

> “The Social Web Working Group will create **Recommendation Track** deliverables that standardize a common JSON-based syntax for social data, a client-side API, and a Web protocol for federating social information such as status updates.”

That is, there are three goals (although one was actually optional, more on that in a bit):

* A social syntax (what would ultimately become [Activity Streams 2.0](https://www.w3.org/TR/activitystreams-core/))
* A client API
* A federation protocol

In addition, the Charter connected the SocialWG to another group, the [Social Interest Group](https://www.w3.org/2013/socialweb/social-ig-charter.html). As we'll see in posts to come, the Social Interest Group played a key role by creating "user stories" that capture online social activities. Those stories would help structure the specifications the SocialWG would ultimately produce.

### Organizational Issues

After the Charter, the Group began meeting, and the early meetings are marked by seemingly mundane and yet important issues, such as how teleconferencing works, how to take and post minutes, and when and where to meet in person. Those early meetings were about setting workflows and meeting schedules, including how the Draft and Recommendation process works at the W3C.

These meetings also established/emphasized rules about who is allowed to participate in a Working Group.

### What Caught My Eye

Ok, so the first thing that I found fascinating was a desire for and fear of established social media corporations (specifically, Twitter, Google, Facebook). The SocialWG stated again and again that they wanted Facebook or Twitter to participate – here is but [one example](https://www.w3.org/wiki/Socialwg/2015-09-29-minutes) of such a discussion –  but there is also a strong fear of the work being appropriated or buried. Two things are often mentioned as cautionary tales: Schema.org and the Open Web Foundation. Obviously, the desire for and fear of corporate social media involvement relates to who can or should participate. And the lack of involvement from those corporations is really important for this history, I would think.

It's also interesting to note that federation was bracketed off at this point. This is consistent with the Charter, which contemplated that Federation would be an optional deliverable: "Note that the Working Group may not develop the Federation Protocol into a Recommendation and it may become a Working Group Note." Given that, from my perspective, the most important product of this group was the ActivityPub federation protocol, it's remarkable that it almost didn't get done because it was seen as optional. More on that in posts to follow.

Another thing that caught my eye is that implementation and real-world examples were emphasized right away. The W3C specification process requires at least two implementations of every feature:
> Arnaud: Would like to remind people that as a part of the W3C spec track, there will be a point at which we have a call for implementations, at which point we need 2 implementations of _every_ feature to move forward [(2014-09-30 meeting)](https://www.w3.org/wiki/Socialwg/2014-09-30-minutes)

This would be very important in terms of the eventual ActivityPub and Mastodon. The first time we see much emphasis on implementation would be [when ActivityStreams 2.0 is set to move to Candidate Recommendation](https://www.w3.org/wiki/Socialwg/2015-10-06-minutes) in late 2015.

Another fascinating aspect is that roughly a year into its existence, the SocialWG members would have a pretty heated debate about how to communicate. I tagged this in Zotero as "org comm," short for "organizational communication," or how an organization is constituted through its communicative practices. So, even though much time was spent early on in 2014 on how the group would get things done, communication conflicts emerged later on, with discussions about overloads in terms of channels and even flare-ups about who gets to speak when.

A final note, but an important one. There are three distinct "camps" in the SocialWG:
* An academic-focused group centered on SoLiD and semantic markup;
* People with previous federation experience, such as Pump.io folks,
* and IndieWeb, a group of folks who put the webpage at the center of everything.

I'll say more about these groups and their competing visions in future posts.
