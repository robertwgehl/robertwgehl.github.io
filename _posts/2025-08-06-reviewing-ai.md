---
layout: post
author: RWG
title: 'The Plight of the Reviewer: Lessons from AI Generation and Software'
tag:
    - goal 1
    - peer review
    
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 114985436247329498
---

On the latest [_Late Night Linux_ podcast](https://latenightlinux.com/late-night-linux-episode-345/), the gang discussed a [recent blog post by Daniel Stenberg](https://daniel.haxx.se/blog/2025/07/14/death-by-a-thousand-slops/) about the plight of reviewers -- specifically, open source [bug bounty](https://en.wikipedia.org/wiki/Bug_bounty_program) program reviewers, who are facing a rising tide of AI slop. I think this has implications for my profession, particularly the task of conducting academic peer reviews.

<!-- more -->

As Stenberg reports, the bug bounty program had largely been a success over the years. He and his colleagues used it with [curl](https://curl.se/), a popular command-line utility to transfer data across the internet. As a widely used, open source program, checking for bugs -- especially security issues -- is a vital part of maintenance. And as open source development has taught us, this is a task far better done by the crowd than by one person or even a handful of people. A bounty system, where people are paid for successfully finding flaws in curl, rewards folks for doing this necessary work.

But things have recently changed, reports Stenberg:

> The general trend so far in 2025 has been way more AI slop than ever before (about 20% of all submissions) as we have averaged in about two security report submissions per week. In early July, about 5% of the submissions in 2025 had turned out to be genuine vulnerabilities. The valid-rate has decreased significantly compared to previous years.

With the advent of LLMs, people are now feeling empowered to prompt genAI with a bit of curl's code, asking genAI to identify bugs, and then they submit the results as a new bug report, either hoping to help or simply hoping to win some bounty money.

This results in much wasted time. As Stenberg wrote in an earlier post, ["The I in LLM Stands for Intelligence"](https://daniel.haxx.se/blog/2024/01/02/the-i-in-llm-stands-for-intelligence/), the problem of AI-generated bug reports is that they seem plausible, even if they're bullshit:

> The better the crap, the longer time and the more energy we have to spend on the report until we close it. A crap report does not help the project at all. It instead takes away developer time and energy from something productive. Partly because security work is consider one of the most important areas so it tends to trump almost everything else.

> A security report can take away a developer from fixing a really annoying bug. because a security issue is always more important than other bugs. If the report turned out to be crap, we did not improve security and we missed out time on fixing bugs or developing a new feature. Not to mention how it drains you on energy having to deal with rubbish.

And such wasted time is a major issue with a volunteer-driven, open source project like curl.

## Echoes of My Profession

I find all this eerily similar to issues I brought up in [a recent post about academic peer review](/2025/05/08/ai-review.html), a practice I regularly engage in. In that post, I predict that having to conduct academic peer reviews of AI-generated articles is going to increase in the coming years. 

Much like bug reports handled by open source projects, academic peer review is predominantly done by unpaid volunteers. Much like security reports, it's a necessary part of the publication process (although I would grant the stakes are a bit lower). A successful bug bounty offers a reward (some cash money). Successful publication in a journal does, as well (most often in the form of prestige and sometimes tenure).

If I'm right that AI-generated articles are going to be an increasing problem for peer reviewers, Stenberg's posts are sounding a clear warning: we academics will drown in AI slop, much as Stenberg and his colleagues are.

## Beyond Bug Bounties: Review and Software Development

Beyond bug bounties, software developers are also wrestling with having to review AI-generated code. On that episode of _Late Night Linux_, Félim Whiteley noted that 

> the problem of AI coding is the fact that there's too much for me to review. It's too easy to write software... I'm now overloaded with the amount of stuff I have to check and review and verify.

Similarly, Jake Trent's post ["Reviewing AI-Generated Code"](https://jaketrent.com/post/reviewing-ai-generated-code/) considers the plight of software reviewers. He notes that AI-generated software code reduces trust during code reviews. To mitigate it, the reviewer must do a great deal more work than merely review:

> It's as if I as the [reviewer] have to start from the problem statement and reason through to a solution myself. The solution has to make contact with a human's brain. I may have to reason about the problem, a design, an implementation, proper tests. This is because all that I can presume to have happened is the typing of a prompt into a chat box and the output of code from an LLM. I can't just push that to prod.

Essentially, Trent is arguing that code reviews are reverting to the actual writing of code -- conceptualizing a problem and implementing a solution. AI-generated code is making a vital stage in sofware development, the code review, much much harder -- even as it makes writing draft code much easier. That compounds the problem -- a glut of poorly-written code, generated by people who don't understand it, being pushed on people who have to review it.

## Lessons for Academics from the World of Software?
So, bug bounty review and software review are being swamped by slop. I'm worried academics will be, too. Can we academics learn from the field of software development to mitigate this problem?

Maybe.

One solution on offer is to treat AI-generated code (or, I would presume, bug reports) as made by metaphorically junior coders. That's [the suggestion of Rajat Gupta](https://medium.com/mr-dops/the-hidden-cost-of-genai-code-technical-debt-in-the-age-of-ai-assistance-d4b5be2d70de):

> Here’s my playbook: treat AI like a brilliant but reckless intern. Review its work, enforce standards, and monitor metrics (duplicate code ratio, bug rates). Invest in training and lean on automation — linters, scanners, even AI-driven refactoring tools — to catch the mess early.

Maybe that would work in the realm of software development. But that doesn't quite work for academic peer review. I can't treat every journal article as if it's written by a student. Academic peer review isn't a moment to train others -- rather, it's one of the first moments when academic research is tested outside of the bounds of where it was written. While peer reviewers do make suggestions for revision, our job is not to help authors completely rewrite their articles or re-do their research. We basically give the article a thumbs-up or thumbs-down, judging it on the quality of its methods and analysis.

There's another solution on offer. Of course -- of course!!! -- people are suggesting that we just need to [use AI to review AI code](https://www.forbes.com/sites/davidprosser/2025/05/07/worried-about-ai-generated-code-ask-ai-to-review-it/). And I am almost 100% certain many of my fellow peer reviewers will glom onto such a solution.

But I personally hate this idea. I hate the idea of offloading the intellectual task of reviewing to a machine, and I would hate to be on the receiving end of such a review. It strikes me as irresponsible and self-defeating.

Another solution to the problem of too much code/too many bug reports comes from Stenberg (he of the bug bounty posts), who suggests charging people money to submit bug reports, or removing the reward. 

But he doesn't really like those ideas. And I'm not sure they would translate to the academic realm. After all, journals are already charging money for the privilege of being published, and folks are paying. And there's no removing the reward of publication -- that's essential to the academy.

Ultimately, looking through the bug bounty/software dev posts on this issue, I find myself most in agreement with Trent's "Potential Helps":
> Write your own code.
> Understand your own code.
> If you use code from another source, give it a citation. For copy-pasted code, affix a URL to the source. Make notes on modifications. If you were assisted by a fellow developer, add them to the commit as a co-author or comment the fact. If you generated the code, comment it as generated.
> If there's a section that you're less confident in, state the fact in your review request.
> The citations of sources in the code help focus the reviewer to more granular portions for which more or less time and criticality might be warranted in order to mitigate the risk of the code, based on the source.

This is similar to my suggestions in my recent post. I really don't recommend any use of generative AI -- after all, like Trent's ideal coder, I would think my colleagues would write their own articles and understand their own articles instead of outsourcing any part of the process to [unaccountable and quite possibly fascist black boxes](https://blog.bgcarlisle.com/2025/05/16/a-plausible-scalable-and-slightly-wrong-black-box-why-large-language-models-are-a-fascist-technology-that-cannot-be-redeemed/).

But if folks are going to use generative AI in their academic research, I'd say the use of those systems needs to be cited. Clearly. Make notes on how you used genAI. Don't hide it, even if you think it simply helped with grammar. Be transparent. 

We peer reviewers deserve to know.
