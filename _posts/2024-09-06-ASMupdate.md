---
layout: post
author: RWG
title: 'ASM Update: Mastodon Research Ethics and the Ethical Quandaries of Tech Advocacy'
tag:
    - ASM update
    - research ethics

comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 113092548001487706
---

In this ASM update, I'll write at length about [a new research study on Mastodon](https://link.springer.com/article/10.1007/s11616-024-00855-6) that gets the ethics of research right -- even though they pulled data from my home Mastodon instance. I'll also discuss [a recent podcast episode](https://latenightlinux.com/late-night-linux-episode-297/) that talks about the ethics of using and promoting FOSS.

<!-- more -->

## AoIR.social data were included in an academic study -- and that's OK
I'm one of the admins of [AoIR.social](https://aoir.social), a Mastodon instance for members of the Association of Internet Researchers. In the AoIR.social Code of Conduct, we include the following bit about research:

> Researchers who wish to study AoIR.social or our users by collecting data using the API or through any other means that does not involve an "opt-in" from individual users are required to submit their protocol, analysis plan and all relevant ethics approval documentation from their institutional review board or departmental internal review documentation by email to the AoIR Fediverse admin account. You may also be required to submit code you plan to execute so that it can be tested to ensure it does not degrade the quality of service to other users.

I just found a study that most likely included data culled from AoIR.social via the Mastodon API, and... I'm not mad! I don't think they violated our Code. In fact, I think the authors did the fediverse a huge service.

The study in question is ["'Don’t research us' -- How Mastodon instance rules connect to research ethics,"](https://link.springer.com/article/10.1007/s11616-024-00855-6) by Marco Wähner et al. It appeared in _Publizistik_ a few weeks ago.

The authors are asking whether and how Mastodon instances signal their preferences for the collection and use of data for research purposes, as well as what ethical issues arise when researchers gather data from Mastodon's API.

Through the use of the Mastodon API, they pulled in codes of conduct from over 4000 active English-language Mastodon instances. They then quantitatively and qualitatively examine those codes. While they found that many COCs emphasize rules of behavior on the instance (e.g., no racism, no transphobia), only 31 English-language instances actually address research ethics and discuss data usage.

Undoubtedly, AoIR.social is in their dataset, since we address the topic explicitly. So, why am I not upset with Wähner et al's own paper, then?

It's because this research team did not study _individuals_, but rather focused on _instances_. This is exactly [the point I've made elsewhere](https://www.cell.com/patterns/fulltext/S2666-3899(23)00323-9) with fellow fediverse researcher Roel Roscam Abbing. I also [posted a bit more](/2024/03/14/Instances-and-Individuals.html) about the individual/instance distinction on this blog. We need these studies and data -- maps of the fediverse, population data, and trends in codes of conduct language are valuable insights.

And not only will the fediverse benefit from Wähner et al's work, I agree with their claim that pulling instance codes of conduct does no harm to fediverse members. I do not see it as a violation when people do instance-level studies of the fediverse without getting the consent of fediverse admins.

In light of the fact that only a small number of instances post explicit rules about research data use, the authors offer some recommendations to researchers. I'll get to them, but first, let's talk about implications for instance admins like me.

One implication of their study is that Mastodon and fediverse instances ought to include rules about research in their codes of conduct. This may be a wise thing for instance admins and community members to consider. However, I think we should not merely make this recommendation. It puts too much burden on instance admins and communities. If fediverse instances must write rules for every unethical case they might possibly encounter, their codes of conduct will shift from human-readable, community documents to legalese-drenched Terms of Service agreements found more often in corporate social media.

No, the answer here is that researchers, not instances, need more ethical training and thinking. One approach might be to consider codes of conduct in the aggregate and proceed from the assumption that a prohibition on a handful of instances indicates a much broader -- if unstated -- prohibition across the fediverse itself. Researchers might protest at this, arguing this would stifle their work, but I would argue that ethical approaches to fediverse research should meet an extremely high bar.

In fact, Wähner et al make this same point:

> The characteristics of the user community may lead to the expectation that users may hold a (more) critical stance towards user data collection on Mastodon. Of course, as stated before, the total number of 31 instance rules explicitly addressing data use for research purposes is quite low. Providing a detailed explanation for why there are not more instance rules reflecting on research data collection is beyond the scope of this paper. However, based on research on the general lack of awareness for the fact that researchers are using data collected from social media platforms (Breuer et al. 2023; Quinton and Reynolds 2017), we assume that this is also true for a substantial share (if not the majority) of Mastodon users (Wähner et al., 2024, p. 16).

For those who wish to examine individual-level data, Wähner et al go on to offer several suggestions for researchers of the fediverse, including paying attention to instance rules. They note that if an instance explicitly prohibits the use of member data, researchers ought to expunge it -- even in cases where the data will be anonymized. They also recommend reaching out to -- and collaborating with! -- instance admins in research design. Admins can be useful guides in getting informed consent among fediverse members.

I agree, and thus I recommend this study to future fediverse researchers. I'll definitely put this study in [the Bibliography](/bib.html).

## Late Night Linux tackles the ethics of advocating FOSS
Speaking of ethics, the crew at the Late Night Linux podcast just raised a bunch of ethical issues in FOSS, ones that I tackle in my [forthcoming book about Mastodon and the fediverse](/2024/02/11/Move-Slowy-Preview.html). In [their latest episode](https://latenightlinux.com/late-night-linux-episode-297/), the hosts talk about what to do when we deal with unethical Internet corporations. Cloudflare is one they highlight. X is another. Is it unethical to use their products? Or to give your custom to companies that do?

Both of these examples are quite germane to my book. In it, I definitely talk about how the actions of X have prompted a shift from that platform to the fediverse (among other alternatives). I also talk about a somewhat shameful secret of the noncentralized fediverse: that it often relies on [centralized cloud hosting services (such as Amazon) and technologies (such as Cloudflare) to function](https://doi.org/10.1145/3355369.3355572).

So, should we despair if we cannot escape unethical corporations? The LNL crew largely said, no. You try your best, and you do better over time.

But the real answer came in their next segment, which was about advocating that Windows Subsystem for Linux users make the switch to mainline Linux. The LNL crew [posted this question to Mastodon](https://mastodon.cloud/@LateNightLinux/113005956969609375), and the dominant answer was: no. Let people solve problems in the way that works. The best you can do is show them the benefits of the better stuff you use.

I think the same is true of the fediverse. We could berate people for using corporate social media. I've found over many years, however, that that doesn't work. Instead, show people what you use and talk about why it's better. If they switch, great! If not, that's ok. The fediverse isn't about infinite or rapid growth. It's about growing slowly and purposely.



