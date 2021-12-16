---
layout: post
author: RWG
title: Test post for Mastodon Comments
tag:
    - Goal 1
comments: 
  show: true
  fedihost: scholar.social
  fediusername: robertwgehl
  fediid: 107457359549037273
---
I've been struggling with having comments on this Jekyll-based static site for a while. For a bit, I used Staticman, but that died for some reason.

Then, it hit me: so many sites use Facebook comments. Why can't I use Mastodon, the FOSS alternative social media system, to do something similar?

Fortunately, [this guide](https://blog.xmgz.eu/jekyll-mastodon-comment/) provided all the code I could need to do exactly that!

So this is a test run. Feel free to comment on it using your Mastodon account. (I think other federated accounts might work, but not sure -- if so, let me know in the comments!)

If you don't have a Mastodon account, don't worry! You can [sign up for an instance](https://joinmastodon.org) and join the federated fun. 

UPDATE #1
------

I've tested it a bit and have found a few things that give me pause:
* It does not respect the distinction between Unlisted and Public privacy settings. Both will show up here.
* It *does* respect DM -- that is, DMs do not show up as comments.
* It does not respect Content Warnings. CWs don't show up.

With all that in mind, I think I may keep it (pending further testing) and include a warning in the "Comments" section.

UPDATE #2
---------
Thanks to another Mastodoner, I found that if anyone who uses Mastodon to comment on a blog post deletes said comment, then it will also no longer appear on the blog. I think that's a cool feature, but I'm thinking that I have be *extremely clear* about what happens when people comment on my blog. It's going to be public -- very public -- not just in the federation, but also on my website.

However, I'm not 100% certain this is wise. I'd love to get more opinions from Mastodon users. Feel free to leave them in the comments -- or, to be certain that your opinion is expressed privately, DM me (@robertwgehl@scholar.social).
