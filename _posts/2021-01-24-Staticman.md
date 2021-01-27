---
layout: post
author: RWG
title: Staticman Comments Test Post
tag:
    - Staticman
comments: true
---

This post is to test [Staticman](https://staticman.net/) comments. I'll edit this post later to update my progress. For now, if anyone stumbles across this and wants to add a "test" comment or something helpful, feel free!

<figure>
    <img src="assets/images/staticman.png" alt="The Staticman Logo">
    <figcaption>The Staticman Logo</figcaption>
</figure>

I'm basing this process of this [helpful blog post](https://travisdowns.github.io/blog/2020/02/05/now-with-comments.html) from Travis Downs of Performance Matters. Thank you!

<!-- more -->

Update 1: There are clearly problems in my configuration, and so I must keep debugging. But it's time for a walk.

Update 2: Success in posting a comment after turning ReCaptcha off. However, not sure if I set things up to *display* the comment...

Update 3: Success in getting a comment posted! But the workflow is very convoluted. I know Staticman uses Github pull requests to work, so I have to merge each comment. That's fine. However, after I do so, I will have to move the data from my local version of my static site and then rebuild it via Jekyll. [There has to be a better way](https://www.youtube.com/watch?v=INX-KrjaNOo)! And I will figure it out.

And, I do know I will have to style the comments, as well. One thing at a time.

Update 4: I think it's done! Comment forms are styled for desktop and mobile, and the workflow is now improved. I initially set up my Github repository to be only the contents of the _site folder, but now the whole thing (warts and all) is in Github, which makes moderating comments much easier.

Once again, thanks go to Travis Downs for his exhaustive post on how to get Staticman going, as well as some of his code.

I do have a few more tweaks -- most notably, to de-Google-ify the whole thing, but the [system is not down](https://www.youtube.com/watch?v=JwZwkk7q25I).
