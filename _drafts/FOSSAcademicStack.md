---
layout: post
author: RWG
title: I Asked Mastodon About FOSS for Academics. Here's What They Said
tag:
comments: true
---

I [posted a question to Mastodon](https://scholar.social/@robertwgehl/105675026053096230) (specifically, scholar.social):

> Ok! If you had a good budget to build a cloud infrastructure to support small teams (2-5 people) collaborating on projects, with a special focus on academic writing projects, what would you recommend?
>
>I'm thinking Linux-based cloud stuff, so I have in mind:
>* Nextcloud
>* Jitsi
>* Natrix
>
>and...? Any recommendations?

I asked this question in all seriousness. I am lucky enough to have a small amount of research funding, I want to promote the world of software beyond Google and Microsoft, and so I'm really keen on building a FOSS Academic Laboratory in the cloud and using to for any collaborative projects I'm a part of.

The response I got to the questions was... *freakin' awesome!*

I thought it would be a good idea to catalog it here. I'll start with the least-recommended things and work my way up to the most-recommended. That's not to say this is a ranking -- things mentioned only once might be really valuable. I'm really just noting what was mentioned most. 

I'll also note which ones I am considering deploying -- again, this is not a commentary on the quality of any of these systems. It's more related to my own specific use cases forged in the past decade of academic collaborations.
<!-- more -->

Fidus Writer
------------
This is one I hadn't heard of. Per their website, [Fidus Writer](https://www.fiduswriter.org/how-it-works/) is

> an online collaborative editor especially made for academics who need to use citations and/or formulas. The editor focuses on the content rather than the layout, so that with the same text, you can later on publish it in multiple ways: On a website, as a printed book, or as an ebook. In each case, you can choose from a number of layouts that are adequate for the medium of choice.

Sounds intriguing!

However, it looks like its Zotero support is limited to drag-and-drop. I'd definitely want something closer to LibreOffice's level of Zotero integration (cite while you write, editing citations, etc). But Fidus looks like it's developing quickly, so it may be one to watch, especially since it puts collaboration first.


PubPub
------
[PubPub](https://www.pubpub.org/about) is a means to publish academic work online and to continue the iterative editing of it even after publication. It solves a problem -- after publication, I might find a mistake in my work, or want to update it, or to allow someone else to build on it. But I have no real way of doing that. PubPub solves that problem.

I've seen books published in this manner, and I always value the easy access to them. I don't have as much experience with giving or receiving feedback in this manner.

This may be a bit of FOSS to explore later on -- perhaps as a way to share my work outside of normal publishing channels.

Latex
-------------------------
Several in the thread made recommendations for LaTex collaborative systems, citing ShareLatex and Overleaf. Looks like [the two are one and the same now](https://www.sharelatex.com/), having joined forces.

I have a thing to confess: I've never used LaTex, and I haven't worked with anyone who has, either. So I'm going to note these for the record, but I can't say too much about them!

Homebase
--------
One person mentioned [HomeBase](https://joinhomebase.com/). At first glance, this may seem odd, since it's geared towards small businesses. But it's really a suite of team collaboration applications, like scheduling and time tracking, group chats, and tools for "onboarding."

I could actually see using something like this if I needed to hire student assistants, assuming my university's HR does not require me to use the university's HR system. In my experience I've seen both with student workers -- "do it yourself" contracts and hiring procedures and university-mandated HR systems. I prefer the latter for legal reasons, but if I had to do it on my own, HomeBase might solve that problem.

Jupyter
-------
For collaborative code writing and notetaking, there's [Jupyter](https://jupyter.org/). Per their website, "The Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more." 

This is not often a pressing need for the work I do, which is mainly interpretive, humanities work. However, my research area of interest is Internet cultures, broadly speaking, and I have had to come up with or modify web scraping scripts in Python. I could easily see collaborating with someone to build such scripts. Maybe Jupyter is too powerful for that, but if the need arises, I would take a look at it.

WriteFreely
-----------
[WriteFreely](https://writefreely.org/) is something I keep hearing about, which is not surprising since I spend so much time on Mastodon! It's a minimalistic blogging platform that integrates well with ActivityPub, allowing people in the fediverse to follow and share one's posts. It's meant to be so light it could run on a Raspberry Pi, which is a great feature. 

I could see integrating this into a project, since many of my projects have a public-facing, blogging component. I'm definitely considering this one.

BookStack
---------
[BookStack](https://www.bookstackapp.com/) is a self-hosted wiki system. Similar to what I said about WriteFreely, this could underpin the public-facing part of any given project. There are times when the presentation of information calls for blogs, and there are times when a wiki is a good way to go. I only ever thought of MediaWiki as a solution, but BookStack looks like it has a lighter server footprint.

Rocket.chat or Mattermost
------------------------
[Rocket.chat](https://rocket.chat/) and [Mattermost](https://mattermost.com/) were cited as alternatives to Slack.  Of the two, Mattermost is touting its security aspects, which is always a good emphasis. This is especially the case for academics dealing with sensitve data (interviews, HIPAA-protected data, etc).

However, I've not really used Slack, so I'm not sure what I'm missing in that regard. 

Arkisto
-------
[Arkisto](https://arkisto-platform.github.io/) is meant for data management, particularly at the end of research projects. As the website says, "The basis of Arkisto is that the long-term preservability of well-described data is *always* the first consideration." It looks to me as if they're thinking long-term about storing data for future use.

The sort of work I do may not fit what they have in mind. If I gather, for example, ethnographic data from participant observation (such as I did for my book *[Weaving the Dark Web](https://mitpress.mit.edu/books/weaving-dark-web)), I actually destroy the data after a period of time to protect people's privacy. 

For my other work, the data I rely on is bibliographic -- I collect sources and interpret them in a more humanistic/historical approach.

Still, I sometimes get invited to join teams working with data in the way Arkisto envisions. Thinking long-term about such data as a public good is a laudable goal.

Jitsi
-----
Several people agreed with my interest in [Jitsi](https://jitsi.org/), the self-hosted video conferencing system. I am strongly inclined to try it again. I tried it in mid-2020 and experienced glitches. I was very keen on getting it working, though, because I was (and remain) opposed to the sudden explosion of Zoom use. Jitsi struck me as a potentially easy alternative for students to talk to me. I had trouble running it, but a few months is a long time where well-maintained FOSS projects are concerned.

XMPP-Based Solutions
--------------------
[XMPP](https://xmpp.org/). I think I heard of that once upon a time! In all seriousness, I was once an avid [Pidgin](https://www.pidgin.im/) user (with OTR encryption, of course). I went away from it, for some reason. 

But XMPP is making a comeback, not just for me, but for many people. There's [Pleroma](https://pleroma.social/), a federated server that can connect to Mastodon, Pixelfed, and other projects. From what I could see, no one in the thread mentioned [Movim](https://movim.eu/), an XMPP-based federated social networking system getting a lot of attention these days, but I'm pretty sure someone will mention it. 

I'm starting to lean towards installing one of these, at the very least to experiment with them and see where they take me.

Matrix 
------
Matrix was mentioned a great deal, but people were less supportive of this option. Instead, they pointed to other ways to chat. I was surprised by this -- some of the Linux podcasts I listen to are all-in on [Matrix's Synapse](https://matrix.org/), so I figured it was a necessity. But, maybe not.

I'm happy to set that one aside to reduce my workload.

Nextcloud
---------
Nearly everyone agreed on [Nextcloud](https://nextcloud.com). It would end up being the beating heart of a collaborative academic cloud setup. It has file version control and file sharing. And I could easily add calendars and task lists. 

I tend to agree: I have a small Nextcloud server of my own, and I collaborated with a colleague on a book project using it. While the project went smoothly, there were a couple times the version control of Nextcloud saved us from losing work. 

We mainly used Signal for chatting, mostly via or text and on occassion via voice. Signal worked fine, but I would like something more persistent to keep track of ideas (for privacy, we set our Signals to delete after a set period.) This is why I mentioned something like Matrix or Jitsi in my initial post. One person noted that Jitsi or Matrix would not even be necessary, thanks to [Nextcloud's text and video chat support](https://nextcloud.com/talk/). Another disagreed, essentially, arguing that people are by now used to the capabilities of a Jitsi-like video conferencing application. In any case, Nextcloud is a possible chat channel.

Several pointed to [Collabora](https://www.collaboraoffice.com/), the system that allows for collaborative editing of Libreoffice docs (in a manner similar to Google Docs.) Assuming Collabora supports [Zotero](https://zotero.org) as well as client-side Libreoffice does, it seems like a no-brainer to add to the mix. The book project I just completed did not use Collabora, instead passing ODTs back and forth, so I'm curious to see how well Collabora could work in a future project.

Add it all up and Nextcloud is the single most important app in the stack, so I'm definitely going to fire it up. I may see if I can use it for all the things -- invest in a more powerful server with a good amount of storage, rather than multiple VMs. It may be easier to administer.

Final Thoughts 
---------------
Looks like Nextcloud is definitely in the future, and Jitsi *might* be. Something federated and XMPP-based might be, as well. The others are good to keep in mind for more specialized use cases.

Nextcloud gets the nod simply because it could cover all the bases, so administering would be easier -- that's a *huge* bonus.

A final thought, but an important one. I did not ask specifically about security. If anyone has recommendations there, I'm all ears. I know that I'd want to use SSH keys for server administration, two-factor authentication on both my hosting provider and Nextcloud, and insiste on 2FA for any collaborators. Beyond that, any tips out there?

Thanks to everyone who offered suggestions! 