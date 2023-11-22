---
layout: post
author: RWG
title: Ethics and Codes of Conduct on Mastodon
tag:
    - Goal 2
    - Mastodon
    - Codes of Conduct
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid:
---
Yesterday, I taught one of the final meetings of my undergrad "Ethics and the Media" course at York. We're using [Charle Ess's _Digital Media Ethics_ (3rd edition)](https://bookshop.org/p/books/digital-media-ethics-charles-ess/7513541?ean=9781509533428) as our textbook, and so we've had a good guide to ethical theories, such as virtue ethics, deontology, utilitarianism, and feminist ethics of care. (I also supplement Ess with readings and ideas from Shannon Vallor, Kwame Gyekye, Carissa Veliz, Michael Zimmer, and others).

Much of the course has been about learning the ethical theories and then discussing [case studies](https://mediaengagement.org/vertical/media-ethics/). It's been quite an enjoyable course to teach, particularly because I've seen the students go from the vague and intellectually unsatisfying statement "Ethics is a subjective, personal thing" to the more robust "Let me lay out how a virtue ethicist would think about this."

But I wanted to have at least one day of the course dedicated to applied ethics. Instead of looking at a case that happened in the past, I wanted the students to apply the ethical theories to a concrete situation.

And these days, we have a great situation in digital media ethics to consider: what to do when we start up a Mastodon server?

In this post, I'll write up what we did in the class, in case anyone out there wants to try something similar.
<!-- more -->

## Mastodon in the classroom

I spun up a relatively inexpensive Digital Ocean server and installed the latest version of Mastodon. I also imported a [server blocklist](https://thebad.space), because I did not want to have the students -- all of whom were new to Mastodon -- experience some nasty trolling in their first foray. At the same time, I still wanted students to be able to follow accounts outside of our server, so blocking known bad instances made the most sense. I recommend anyone using Mastodon in the classroom do something similar.

I then invited students to join and mess around with our server -- post, share, make profiles, etc. I realized that they would see essentially an empty stream and few others -- this is all part of the process. I wanted to stress to them that everything on the server is under our control, so we -- not some big company -- have to decide how active our server would be.

## What about a Code of Conduct?

One step I skipped in setting up was setting server rules and a code of conduct. I did this on purpose: it was the point of the in-class discussion. After providing some background details about Mastodon and the fediverse and answering student questions, we then discussed codes of conduct. For background, I gave them a draft chapter of my [current book](/2023/08/17/OxfordUP.html), which focuses on the history of codes of conduct (and thus draws heavily on an interview with [Coraline Ada Ehmke](https://where.coraline.codes/)).

After we talked codes of conduct, I talked about how running Mastodon requires us to be active in making choices about content moderation. Running a Mastodon server is a moment of applied ethics.

I then asked them to break into four groups:

* One group focusing on **feminist ethics of care,**
* Another focusing on **deontology,**
* Another on **virtue ethics,**
* And the last on **utilitarianism.**

I asked the group to first summarize the ethical theory (not an easy task, I know).

Next, I asked them to apply the ideas from their ethical theory to our potential Mastodon code of conduct.

I really, really liked the results!

Here are summaries of each:

### Feminist ethics of care
Feminist ethics of care (FEOC) rejects the idea (most associated with deontology) that ethical decisions are the sole purview of individual, autonomous rational actors. Instead, FEOC argues we make ethical choices based upon, and informed by, relationships we have with one another. Moreover, an ethical choice is not purely a rational matter, but also involves emotions. Finally, FEOC elevates care of others to the center (but it rejects the idea that only one segment of our society is responsible for care work).

Based on this theory, the students argued that our Mastodon server code of conduct should
* Describe how we can network with other servers who share our values.
* Take inspiration from the first clause of Canadian charter: your rights end where someone else's begin. You can post so long as you don't violate others' rights.
* Emphasize contextual judgement (considering potential violations in context).
* Emphasize communication during moderation, using empathy for would-be violators.

My take: this is a great set of insights. It echoes what I've learned over the past few years doing interviews with fediverse admins. Many told me that their approach to moderation is to talk to people and find out what's going on. They also talk about how they choose to federate/block other instances.

### Deontology
Deontology emphasizes individual rights and autonomy, as well as duties to do what is right. Intentions often matter more than consequences. Often deontology is expressed as rules (although that's a bit reductive.)

Students in this group did offer rules, likely inspired by reading sample Mastodon codes of conduct:
* Post nothing illegal!
* No discrimination based on age, race, gender, sexuality
* No harassment
* No trolling
* No defamation or coercion
* Show some respect in the community

My take: if there's one ethical theory that Mastodon seems designed for, it's deontology. Mastodon's software prompts the admin to put in "Server Rules," short statements about expectations would-be members should live up to. Many, many Mastodon codes of conduct have rules similar to the above.

### Virtue Ethics
Virtue ethics is less about intentions or consequences than it is about character. Virtues in a digital environment might include honesty, humility, courage, and compassion, and these are balanced against vicious extremes. Virtue ethics is also relational in that we teach children about virtues and provide advice to them when they have to make ethical choices.

The students in this group suggested that our code of conduct should
* Call for displays of virtous traits, such as wisdom, courage, loyalty,
* Emphasize being polite and respectful, and
* Have high standards for moderation.

My take: I was really curious what the students would say in this group, and they delivered some good stuff. What's useful, I think, is contrasting the negative rules of deontology with these positive virtues and character traits. I could imagine a code of conduct that integrates virtue ethics to emphasize positive behaviors.

### Utilitarianism
Alongside another consequentialist theory, libertarianism, utilitarianism is probably the most familiar theory to me, since I grew up in the USA. (I'm not saying I endorse either; just that I think I soaked in them). Utilitarianism judges acts based on their consequences: if an act creates the greatest happiness for the greatest number of people, it's an ethical one.

Students in this group emphasized the greatest happiness principle in their code of conduct ideas:
* Let's promote inclusivity to make people safe, welcome, and heard.
* We need to listen to user feedback.
* We need to consider well-being of the community.
* Server members should report stuff to the moderators.
* We should promote free speech but exclude hate speech.

My take: Students really leaned into thinking about the would-be Mastodon server as a community, and so this approach emphasized group happiness. I think this was a good addition to the other ideas, because social media can be fun and happy -- why not build a code of conduct that emphasizes these aspects?

## Summing it all up

We concluded the class by considering how these different approaches to a code of conduct could be synthesized. We kinda ran out of time for that, but I think we may have been able to write a pretty sweet code if we had more time.

I did spend some time talking about enforcement, since no code of conduct is worth anything if you're not willing to live up to it. I ran various scenarios past them -- what if someone outside our server violates our code? What if someone outside our server reports one of our members?

Their answers reflected the ideas I've heard from seasoned admins, including how admins discuss things with one another and how admins talk to members.

All in all, I think this experiment was really exciting. Unlike corporate social media -- Facebook, TikTok, X, etc -- _we_ get to make decisions about moderation when we run our own instance. It's a big responsibility, but these students showed they're up for it.
