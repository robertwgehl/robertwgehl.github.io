---
layout: post
author: RWG
title: Reading the Online Harms Act with my Fediverse Admin Hat On
tag:
    - Online Harms Act
    - Mastodon
    - Fediverse
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 112249058642915613
---
The [Online Harms Act](https://www.canada.ca/en/canadian-heritage/services/online-harms.html) is currently the talk of Canada. As the government’s website describes it,
> The internet is an exceptional tool for people of all ages to learn, play and connect with family, friends and those with similar interests. However, just like the outside world, the digital world can pose significant dangers. Social media can be used to sexually exploit children, promote self-harm to children, incite violence, put people’s safety at risk and foment hate. Online harms have real-world impacts with tragic, even fatal, consequences.

> The Government of Canada has introduced legislation to hold social media platforms accountable for addressing harmful content on their platforms and for creating a safer online space that protects all people in Canada, especially kids.

As something that addresses speech on the internet -- and includes some strong penalties for spreading hate speech -- the Act has led to massive debates. I won’t summarize them here, but you can read thoughtful critiques from [Professor Michael Geist](https://www.michaelgeist.ca/tag/online-harms-act/) and you can listen to a discussion on [Canadaland’s Backbench](https://www.canadaland.com/podcast/85-the-hate-u-post/) to get a sense of things.

My interest here is not to delve into the controversies, but instead read the Act while wearing my Mastodon admin hat. I am one of the two admins of AoIR.social, a [Mastodon](https://en.wikipedia.org/wiki/Mastodon_(social_network)) instance for members of the [Association of Internet Researchers](https://aoir.org/). AoIR.social gives our members access to [the fediverse](https://en.wikipedia.org/wiki/Fediverse) -- the global network of thousands of social media servers, with millions of users engaged in social media activities.

An initial question: does the Act apply to the tens of thousands of fediverse instances with their millions of users? Does it thus apply to AoIR.social? Considering that the Act defines “social media service” as “a website or application that is accessible in Canada, the primary purpose of which is to facilitate interprovincial or international online communication among users of the website or application by enabling them to access and share content” (page 5), then the answer is yes. AoIR.social operates internationally, including in Canada. So do many of the other tens of thousands of fediverse servers.

Since I’m one of the two admins of AoIR.social, am I affected? I believe so: I would be an “operator,” “a person that, through any means, operates a regulated service.” It could also be that the AoIR organization itself would be the operator, since in this Act “person” also applies to corporations.

The Act would create a Digital Safety Commission, an agency that would govern social media services. The Act notes this Commission should consider things like the size of the service and the operator's financial and technical abilities. This is good – many fediverse instances are small and are run by individuals or a handful of folks. They also often run on very small budgets as not-for-profit organizations. Regardless, however, I believe small fediverse servers would be affected (unless they find a way to not be available to Canadians).

So: will the Act radically affect fediverse instances, such as AoIR.social? The Act specifically says our service should not harm freedom of expression, and reading it leads me to believe that AoIR.social won’t be affected in that manner. While we welcome debate and discussion, we’re not in the business of platforming the sorts of harmful content the Act discusses.

But, the implementation of the Act could prove to be very burdensome to the administration of fediverse instances, such as AoIR.social. Much is going to hinge on how the Act understands the fediverse.

<!-- more -->

## Duties of Operators of Regulated Services
The Act is meant to regulate social media, and it lays out various duties social media service operators must follow.

The first is the duty to act responsibly: “The operator of a regulated service must implement measures that are adequate to mitigate the risk that users of the service will be exposed to harmful content on the service.”  Another is a duty to protect children, and related to both, there’s also the duty to make harmful content inaccessible to Canadians.

As a fediverse admin, I have two key questions about these duties. First, what is "harmful content"? This is defined on page 4 in the definitions section:
* "(a) intimate content communicated without consent;
* (b) content that sexually victimizes a child or revictimizes a survivor;
* (c) content that induces a child to harm themselves;
* (d) content used to bully a child;
* (e) content that foments hatred;
* (f) content that incites violence; and
* (g) content that incites violent extremism or terrorism."

So, things like revenge "porn", child sexual abuse material, hate speech, and terrorist speech are prohibited. There are definitions offered for each of these, so I won't define them here. Frankly, I have no problem blocking these things.

The other question I have is about the responsibility to "mitigate the risk that users of the service will be exposed to harmful content...." It seems to me that this is not just about removing content that’s posted. It’s about reducing the likelihood AoIR.social members will see such harmful content.

_This_ is where I have a lot of concerns. Some things seem easy to do, but there are other things that I’m not sure about.

Put simply, the TL;DR summary of the issue is: does the Act consider something like a fediverse server an independent social media site? Or would the Act see the fediverse as a singular network, with traffic being load-balanced across multiple servers?

Let’s get into the details.

## What's Easily Done
The Act calls for social media to publish "Guidelines." These "must be accessible and easy to use and must include (a) a standard of conduct that applies to users with respect to harmful content; and (b) a description of the measures that the operator implements with respect to harmful content on the service."

This is pretty easy to comply with, because like many other Mastodon instances, [AoIR.social has a code of conduct](https://aoir.social/about). I believe our code is “accessible and easy to use,” and it explicitly establishes a standard of conduct, which includes prohibitions on the sorts of content the Act describes.

The Act also calls for social media to provide users with “tools to block users” – done and done, because this was baked into Mastodon from its early days.

And the duty to protect children is quite easy for AoIR.social since our membership is limited to dues-paying members of the Association of Internet Researchers, and I don’t think that population includes anyone under 20, let alone minors.

## What's Less Clear
### Tools and processes to flag harmful content
One feature called for is to “enable a user to easily flag to the operator content that is accessible on the service as being a particular type of harmful content.” That’s baked into Mastodon, so easy enough.

But some of it is not as easy to do, such as “notify a user who flagged content as being a particular type of harmful content of the operator’s receipt of the flag as well as of any measures taken by the operator with respect to the content or of the fact that no measures were taken.” Mastodon does not automatically do this, so it would have to be something the admin/mod does on their own. On AoIR.social, if a user flags something and we block it, we don’t really bother to go back to the original flagger and say we did so. We just do it and move on. I suppose we can do the extra step, but it will add work.

But some of it seems misguided to me: “notify a user who communicated content that was flagged as being a particular type of harmful content of the fact that the content was flagged as well as of any measures taken by the operator with respect to the content or of the fact that no measures were taken.” Mastodon _definitely_ does not do this. I believe this is by design, because notifying people that they have had their content removed can invite more harassment. The approach on Mastodon is to block and not really let the blocked person know. I believe this is for safety purposes –- if we block someone’s content and tell them, they might harass us.

That’s not likely to happen if it’s an AoIR.social member. But the big issue is: **does the Act require me to do these actions with people who are not on my server?** If this is all meant to take place _within_ my server, it’s probably not a problem. Most such in-server moderation is going to involve a discussion with the “user who communicated content that was flagged.” In the case of a user who posts something abhorrent, they’re going to be booted. In the case of someone who posts something borderline, we’re going to chat about it. It’s not going to be a formal process, but more personal.

However, if this is meant to govern my interactions with a user on a server _outside_ my instance, I don’t think this is wise, and it could backfire. If, for example, some trolls are harassing people on AoIR.social, I might communicate with them to tell them to stop, but most likely I’m just going to block them (and hence remove their posts) and not explain myself. Explaining myself would probably lead to more harassment, both for the original victim and likely for me or other AoIR.social moderators.

How the Act handles this is going to matter. If the Act looks at the fediverse and sees a bunch of independent servers which can connect to one another and can sever those connections but have no power over each other, that’s fine. (This is how I think of the fediverse). I can moderate my own server easily enough, and even with the Act in force, the moderation burden might not change all that much (depending on how it is implemented -- see below).

If, however, the Act sees a large social media network that distributes the load across multiple resources, then it’s going to raise a great deal of problems for admins like myself. It’s going to create big burdens -- and could even lead to more harmful speech.

### Digital Safety Plan
The issue with how the Act would see the fediverse is really intense when it comes to the Digital Safety Plan section. “The operator of a regulated service must submit a digital safety plan to the [Digital Safety] Commission in respect of each regulated service that it operates,” the Act states.

The details are going to matter a great deal here. As someone attempting to immigrate to Canada, I have some familiarity with Canadian bureaucracy. Much of it is quite straightforward, but some of it is onerous and confusing. If AoIR.social will have to supply such a plan, what will it entail? How will it be submitted? Will it be like getting my social insurance number (which was super easy) or like going through the work permit process (which was pretty labor-intensive)?

Looking at the details, I have concerns. For example is point G of the Digital Safety Plan, which would ask me to report
> information respecting (i) the number of times that content that was accessible on the service was flagged to the operator by users of the service as being harmful content, including the number of flags relating to each type of harmful content, (ii) the manner in which the operator triaged and assessed the flags, (iii) measures taken by the operator with respect to content that was flagged as being harmful content, and (iv) the time within which the operator took measures with respect to content that was flagged as being harmful content.

This would be easy enough – again, _if it’s limited to my server._ AoIR.social members are a collegial, professional lot. I simply don’t expect any of them to post harmful content, and thus I don’t expect to have to often report that they flagged content on our own server. And maybe this would be the case. I can indeed interpret the Act’s “users of the service” to be limited to AoIR.social members.

But this does raise a separate potential problem. If the Act sees the fediverse as a bunch of independent servers, what happens when someone outside my server flags something on my server? For the sake of argument, let’s say AoIR.social is actually a bad actor on the fediverse, and our members share harmful content regularly, and that we don’t report each other (since we all agree with our harmful content-sharing project). Could we simply ignore the pleas of people outside our server to cut it out? Could our Digital Safety Plan simply say, “we didn’t get reports”? The Act has penalties for such things, but it would require someone outside our server to report us to the Commission who would then have to investigate. Meanwhile, we’re gleefully sharing harmful content (in this hypothetical example).

So, maybe the Act should require me (and other fedi instances) to document flags I get from outside my server -- that is, maybe the Act _should_ see the fediverse as one large network.

But if the Act requires me to document flags coming from outside my server, I could also imagine another problem: being burdened by reporting on malicious or coordinated flagging from outside one’s server. I would have to write up reports for those flags, even if they are done in bad faith. There is language about my being able to ignore “vexatious” or “frivolous” flags, but do I have document them, anyway, to prove that all the reports were, indeed, vexatious?

Taken as a whole, I think the Act should treat each instance as an independent entity.

### Duty to Make Certain Content Inaccessible
Subsection 67 of the Act says that if an operator finds material that exploits children or revictimizes an adult, or finds nonconsensual materials (e.g., revenge “porn”), the operator has to block it and tell the person that it’s blocked. This has to be done in 24 hours.

Obviously, I 100% support this. AoIR.social would act with the swiftness if a member posts such material.

But again, the details are going to matter, and the way the Act understands the fediverse is going to be important. If I block content from another server – not my own – do I have to inform the creator of the content, who did so on the other server? Because that sort of thing often leads to harassment of moderators. I or one of the AoIR.social moderators might get targeted by the sort of person who would maliciously share such content.

The next point, subsection 68, discusses “trivial, frivolous, vexatious” or “bad faith” flags, stating operators can ignore those.

That’s good.

But: “If the operator dismisses the flag, it must, within the period that applies under subsection (5), notify the user who flagged the content of the dismissal.” Again, this is pretty problematic if it’s someone outside my server. The sort of person who submits trivial or vexatious reports is not the sort of person who is going to simply walk away when an admin or mod says to stop.

### The Appeals Process

The question of whether I am responsible for reaching out to people on other servers or not is intensified by the “Representations” section (subsection 69), which describes a sort of appeals process:

> “If the operator of a regulated service makes content inaccessible under subsection 67(1) or 68(3), the operator must, within the period provided for by regulations, give the user who communicated the content on the service and the user who flagged the content, if applicable, an opportunity to make representations as to whether the content is content that sexually victimizes a child or revictimizes a survivor or intimate content communicated without consent.”

If I’m required to communicate with someone sharing CSAM on another server and ask them to justify their doing so (representing that it is actually OK to share), I will definitely be burdened. I simply want to block them. Or more likely block their server for engaging in poor moderation. I don’t want to negotiate the finer points of CSAM with people who share it.

This is compounded by the “Reconsideration Upon Request” (point 70): “At the request of the user who communicated the content on the service or the user who flagged the content, the operator of a regulated service must reconsider a decision that it made under subsection 69(2).” If I am asked to do this work with someone outside my server, then a full process could be:

* consider it and judge it
* communicate with the CSAM provider (“Hey, is this really CSAM?”)
* Hear them out
* Decide
* Reconsider upon request
* Decide
* Reconsider again (“Reconsideration” is mentioned twice)

This strikes me as pretty burdensome, as well as a vector for harassment.

And this is not just if the Act sees the fedi as one big network. It could lead to harassment if the Act sees fedi instances as independent, too.

Here’s how: the Act includes the appeals process, because if the Act requires a company like Meta to block stuff without any chance of appeal, that’s problematic, since Meta is going to use automated moderation and will make tons of mistakes.

But for small fediverse instances, I don’t really think a government-mandated appeals process is necessary, nor wanted. Most well-moderated fedi instances are just going to remove accounts of people who post harmful stuff. No appeals. No tolerance. They’re not courts of law. The approach many fedi admins take is: if you want to post X content, you’re free to do so on another server. Does the Act give a bad actor the right to appeal the decision of a fedi admin? I really, really hope not. It would be burdensome and actually cause more harm than good.

### Duty to Keep Records
Finally, let’s consider subsection 72: “The operator of a regulated service must keep all records, including information and data, that are necessary to determine whether the operator is complying with the operator’s duties under this Act.”

Depending on how the Act is implemented, this could be quite burdensome to operators of small servers. _Even if_ the Act sees fedi instances as independent, I don’t really see the benefits of my keeping records on all my decisions. Do I need to record the date and time every time I block an account or outside instance? Do I need to screenshot every time someone flags something?

## Conclusion

In my view, I completely understand the rationale behind the Online Harms Act: I believe corporate social media ought to be regulated. However, I am concerned that, in writing these regulations, the Act's authors may place some undue burdens on the emerging fediverse, which is comprised of tens of thousands of small servers around the world. If the Act's authors understand fediverse servers to be independent entities, then the Act _might_ not be so burdensome. If the Act sees the fediverse itself as a large social media network, problems compound. I'm not a lawyer but I believe that the Act is more likely to have the former interpretation.

But even if so, the Act could still burden small, self-funded social media sites by asking already overworked moderators and admins to do more work (or hire/recruit someone specifically to deal with these regulations). If so, the Act's burdens could happen at a bad time, because the fediverse is starting to emerge as a viable alternative to corporate social media -- the very thing the Act is no doubt attempting to address.
