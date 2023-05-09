---
layout: post
author: RWG
title: Reading the Minutes of the Social Web Working Group, part 2
tag:
    - Goal 2
    - ActivityPub

comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 110339691525442849
---
_NB: This is the second in a series of posts where I will share my notes on my readings of the minutes of the Social Web Working Group. The [first one is here](/2023/01/20/ActivityPub1.html). Future posts to come._

As I mentioned several months ago, my book about Mastodon and the rest of the fediverse can't be complete without a deep understanding of ActivityPub, the protocol that powers the fediverse. ActivityPub itself is getting a bit of love in the press (see this [*Verge* article](https://www.theverge.com/2023/4/20/23689570/activitypub-protocol-standard-social-network) for an example).

And to understand ActivityPub, we have to look at the group that created it, the W3C's Social Web Working Group, or SocialWG for short. They posted their meeting minutes on the Web and I have read *all of them.*

In the previous post on the SocialWG minutes, I focused on the very early years, 2014 to 2015, finding that the period was dominated by organizational issues -- how to meet, how to make decisions, and so on. In this section, I will cover the development of [ActivityStreams 2.0](https://www.w3.org/TR/activitystreams-core/), the first goal of the SocialWG charter.

<!-- more -->

## Phase 2: A social syntax, corporate refusal, and user stories

### Social Syntax
One of the SocialWG's [chartered goals](https://www.w3.org/2013/socialweb/social-wg-charter.html) was the production of a "a common JSON-based syntax for social data." One potential source for this was "ActivityStreams," an already-existing format for labeling online activities. The [Wikipedia article](https://en.wikipedia.org/w/index.php?title=Activity_Streams_(format)&oldid=1153983815) on this gives an example:

> The standard provides a general way to represent activities. For instance, the sentence "Jack added Hawaii to his list of places to visit" would be represented in ActivityStreams as actor:jack, verb:add, object:Hawaii, target:placestovisit.

While ActivityStreams was already in wide use, unless I'm mistaken, it was not codified as an official W3C standard. The SocialWG was to draw on the work of the informal [ActivityStreams community](https://activitystrea.ms/specs/json/1.0/). Fortunately, James Snell, one of the key members of the ActivityStreams Community, got involved in the SocialWG and helped with this process. Spoiler alert: ActivityStreams 2.0 would be the ultimate result.

Regardless of how far along ActivityStreams was prior to the SocialWG, what's interesting about a "social syntax" is a fundamental question: how does one capture human sociality in a vocabulary? As SocialWG member wilkie [stated](https://www.w3.org/wiki/Socialwg/2015-01-06-minutes): "we should get philosophical :) we are trying to capture the entirity of human creativity. the challenge is not getting overwhelmed while also not being too limiting."

There were fascinating discussions in the minutes about terms. An example is a debate that happened in April 2014: should Activity Streams 2.0 use "person" or "profile"? Here's a [snippet of the discussion](https://www.w3.org/wiki/Socialwg/2015-04-14-minutes) between Evan Prodromou and Amy Guy:
> eprodrom: I feel like the Person is enough to justify a Profile, or if there are other kinds of profile, we could use other objects. such as Corporation etc having profiles for.

> ... the biggest issue that a Person having a Profile that people may have other aspects or personalities

> rhiaro: a person can have multiple profiles, but maybe persons and profiles don't need to be modelled separately in the vocab (unsure)

> eprodrom: for instance, my interest in baseball or poker may have different personalities facing different social areas
> ... I feel like it is a complicated and fine-tuned type of concept that can be mapped on multiple accounts
> ... my feeling is that requiring that all users have multiple profiles is unnecessarily complex for the general case

In this case, about a year later, they eventually resolved to use "Person," with the caveat that a ["person" need not be a "physical/real person"](https://www.w3.org/wiki/Socialwg/2015-05-04-minutes).

You can see how complex this can get: standardizing online sociality in a set of vocabulary terms is no simple matter.

(And I should note that the question of Person/Profile is still very much open, in spite of the SocialWG's resolution. Consider Christine Lemmer-Webber's current project [Spritely Goblins](https://spritely.institute/goblins/) and its emphasis on profiles.)

### Corporate Refusal
Ok, so to make a "social syntax," one needs a vocabulary, a set of terms that describes what people do when they're being social. Back in the mid-2010s, there was of course one key source for such knowledge: corporate social media sites, such as Facebook and Twitter.

They had APIs that no doubt did much of the work of describing the units of a social vocabulary, right? Indeed, back in 2009, Facebook even used the same ["activity streams" idea for its API](https://web.archive.org/web/20090430134956/http://www.computerworld.com/action/article.do?command=viewArticleBasic&articleId=9132182&intsrc=news_ts_head), so clearly Facebook would get involved?

And if the organization that *creates standards that power the World Wide Web* -- the W3C -- is involved, then perhaps Twitter and other corporations should get involved, too, and have a hand in shaping resulting standards?

Or, maybe not.

The SocialWG minutes are marked by many instances of the group reaching out to Twitter, Facebook, Google, and other major corporations to get involved. Here's [but one of many](https://www.w3.org/wiki/Socialwg/2015-09-29-minutes):

> eprodrom: one thing i wanted to quickly point out is in previous converstaions we've talked about having some participation by non-members, inviting outside participation
> ... it may be good to think about what we want to do and so we can put out invitations to the public or specific developers

> tantek: i agree. i think the participation that we wanted to focus on previously is around implementers in particular
> ... specifically, implementers of social websites, popular existing social web services
> ... i have a bunch of contacts at twitter if they'd want to swing by for a bit, even informally

They had [studied the APIs of Twitter](https://www.w3.org/wiki/Socialwg/2014-11-18-minutes) very early on, and so it makes sense they would want Twitter engineers involved in the SocialWG standard creation. Twitter never got involved, though. Later, after ActivityStreams 2.0 was finished, there was excitement that [Twitter might implement it](https://www.w3.org/wiki/Socialwg/2016-10-18-minutes). But Twitter never did this.

Reading the minutes as a whole, over time, you can see the hope simply die that any corporate social media would get involved. Instead, at a certain point, not having corporate involvement became something of a virtue. Consider [this statement from Tantek](https://www.w3.org/wiki/Socialwg/2016-06-06-minutes):

> tantek: we have seen with the examples of twitter and facebook there have been tons of business that have been built around either one of those, and ther ehas been a slow attrition of tightening apis, cutting off, etc

And this prescient statement from Sandro Hawke (in the same meeting):

> sandro: all the media companies that are built around twitter don't feel threatened or endangered by twitter
> ... if its started to be an unreliable or evil utility they would want some open replacement

All of this said, the corporate way of doing social was a constant touchpoint throughout the life of the SocialWG -- the members constantly ask "how does Facebook do this?" or "How does Twitter describe that?"

### User Stories
So, if corporate social media is not involved, then how could the SocialWG specify a social syntax? The answer came in one of the most fascinating aspects of the SocialWG minutes: user stories (otherwise called "use cases").

The idea here is that they would write short stories about users doing social things, and then break those stories down into the terms they sought for their vocabulary. Here's the first user story they adopted, the [Social Web Acid Test](https://www.w3.org/2005/Incubator/federatedsocialweb/wiki/SWAT0):

> 1. With his phone, Dave takes a photo of Tantek and uploads it using a service

> 2. Dave tags the photo with Tantek

> 3. Tantek gets a notification on another service that he's been tagged in a photo

> 4. Evan, who is subscribed to Dave, sees the photo on yet another service

> 5. Evan comments on the photo

> 6. David and Tantek receive notifications that Evan has commented on the photo

As I mentioned in my [previous post](/2023/01/20/ActivityPub1.html), creating User Stories would be the responsibility of a sibling group, the Social Web Interest Group. That group would go on to produce about [90 user stories like the one above](https://www.w3.org/wiki/Socialwg/Social_API/User_stories), but would [ultimately settle on seven](https://www.w3.org/wiki/Socialwg/2015-02-03-minutes).

To me, user stories exemplify what I call _[critical reverse engineering](https://www.amazon.com/Reverse-Engineering-Social-Media-Capitalism/dp/1439910359)_ – taking apart existing practices, deriving abstractions from those practices, and then re-implementing those abstractions in a new (and better) way. Since corporate social media companies weren't coming to the table to agree on a standard, the SocialWG simply told simple stories and developed their vocabulary (and Social API, the focus of a later post) from those stories.

### Success!
While they weren't able to attract representatives from corporate social media, the SocialWG did get their first win: ActivityStreams 2.0 drafts were [published in June of 2015](https://www.w3.org/wiki/Socialwg/2015-06-30-minutes) and the Candidate Recommendation appeared later that year. ActivityStreams 2.0 is now a key part of ActivityPub -- but that's a story for later.
