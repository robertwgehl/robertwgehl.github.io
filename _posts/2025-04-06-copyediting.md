---
layout: post
author: RWG
title: 'Copyediting: The Bane of the FOSS Academic Lifestyle Dream'
tag:
    - Goal 1
    - Goal 2
    - workflow
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid:
---
I'm starting this post with a specific passage from my upcoming book. It's important for context.

I conducted interviews as part of the research for [_Move Slowly and Build Bridges_](https://global.oup.com/academic/product/move-slowly-and-build-bridges-9780197776681). In my "Research Note," I write:

> I stored the interview data and notes on a self-hosted Nextcloud server, and I transcribed interviews myself. I did this to avoid storing data or passing interview audio through third-party cloud services, because I am quite certain few if any fediverse members consent to have their ideas supplied to train large language models, as is now happening to data stored in Google or Microsoft services. I realize that this book will be digitally scanned, and thus AI companies may be tempted to use it in their training data. For what it’s worth: I do not consent to have any portion of this book be used to train a large language model (LLM) or similar system. I do not believe any of my interviewees would consent to have their ideas used to train LLMs, either.

I worked very hard to maintain this position throughout the writing process. My notes were stored on self-hosted infrastructure (or, in the case of Zotero, in a non-public library). I drafted much of the document in Zettlr and LibreOffice on local files. I never ran anything through corporate cloud services. I was going to once again write a book without relying on corporate infrastructure.

But then I faced copyediting.

## The Copyediting Phase
Copyediting a book is a major part of the process of writing one. After _years_ of note-taking, drafting, writing, refining, responding to peer reviews, refining further, copyediting is the moment when someone other than the author -- the copyeditor -- goes through the manuscript line-by-line and corrects small errors, revises ackward sentences, and clarifies. 

For _Move Slowly_, Oxford hired [Leslie Anglin](https://reedsy.com/leslie-anglin). Leslie did a superlative job. I'm really, really happy with the results -- it's my writing but improved and with far less errors. (Thank you, Leslie!)

Copyeditors of course need tools to do this work. Over the course of my four books, the tool I've seen copyeditors use again and again is, unsurprisingly, Microsoft Word. I get it -- it's ubiquitous.

Normally, if someone I'm working with uses Word, I have little trouble editing .DOCX files with LibreOffice. It's not always perfect but it's very, very workable. 

But in the case of copyediting, copyeditors do some stuff with Word that I do not comprehend. Paragraphs, phrases, and even individual words get coded (with corresponding colors). Endnotes are handled in a specific manner. Author Queries, where the copyeditor asks the author about something to be fixed, are handled in special ways (even if they are based on standard document comments). There are track changes to consider. As savvy as I might be, copyeditors clearly have a whole other level of fluency with a word processor than me.

LibreOffice simply doesn't handle the special formatting practices of copyeditors well. In the case of _Move Slowly,_ I tried to review and respond to copyedits with LibreOffice Writer and it got mangled quickly. (At one point Writer was deleting words seemingly at random -- not good!) As a result, as with all my prior books, I've had to find a way to deal Microsoft Word to complete the copyediting phase.

Over the years, this hasn't been too big an issue. After all, Microsoft Word has been ubiquitous for years -- I would just find a computer running it. I vividly remember sitting in a University of Utah lab during a 2014 weekend to engage with copyedits for my first book. I've repeated the process in computer labs at a variety of universities for the next few books.

## This Time Was Different
But copyediting with Microsoft Word in 2025 is a very different matter than in 2014. Back then, Microsoft Word was installed on the computer. Now Word is a _service_. You basically need an account to use it. It's in the cloud. And since 2023, [Microsoft began adding generative AI to Word](https://www.cbc.ca/news/business/microsoft-ai-copilot-office-suit-1.6780630).

And that's a problem. I pledged to avoid running my work through cloud services or through anything associated with an LLM. Finding a machine with a "local" Word installation is not a thing these days. Uploading my book to Word 365 would have broken my heart. I've made it _so far_ without having done this sort of thing. Would I be forced to now?

## What about Softmaker Office?
Then it hit me: Softmaker Office.

I had used Softmaker Office in the past on occasions when I simply couldn't work with Microsoft Office files in LibreOffice. Particularly in the case of Powerpoint files, which invariably get utterly mangled in LibreOffice Impress. I had purchased a copy of Softmaker in the past -- maybe it would be the solution here. It isn't FOSS - it is proprietary. But (at least in the past) it was local to my machine.

So I looked at [Softmaker's site](https://www.softmaker.com/en/softmaker-office) and _almost_ paid for a new license. And then I saw it: [Softmaker now includes ChatGPT](https://www.pcmag.com/reviews/softmaker-office).

Maaaaaybe the use of ChatGPT is optional and I could avoid it? But I wasn't willing to risk it. 

It seems like we can't escape from the AI mania.

## This One Weird Trick
I was full on despair mode at this point.

Look, I know for a fact my book will be fed into generative AI. I have no illusions that the passage I quoted above will help. Here's what we've already seen:
* In the time since I signed the contract with Oxfor UP and now, they have [entered into agreements](https://www.thebookseller.com/news/wiley-cambridge-university-press-and-oxford-university-press-confirm-ai-partnerships) with generative AI companies. (I have not heard from the press about this, so I cannot say if my book will be included).
* Regardless, my book will likely be pirated, which means it will be out there with little in the way of restrictions. [Meta has simply gone to pirate libraries to train LLaMA](https://www.theatlantic.com/technology/archive/2025/03/libgen-meta-openai/682093/). My previous work is included.
* And of course, during this copyediting process, surely someone at the press, or my copyeditor, moved my manuscript into a cloud service -- it seems unlikely my book escaped being turned into an LLM input.

But despite these facts I _do not want to simply give in._ I do not want to be forced to contribute directly to the generative AI machine. 

It seemed that the copyediting phase would be my downfall -- whether using Word or Softmaker Office, there would be a chance that my materials would feed some LLM.

Then, I remembered: I still have an old copy of Softmaker Office, one I bought in 2018. It's stored on my machine as a .DEB package. Could I use that?

Turns out, I could. Thank you, Linux! I installed and ran that seven-year-old binary on a modern machine and it worked flawlessly. Softmaker's compatibility with Word held up. I was able to do the copyediting queries successfully -- the proof is in the proofs I just received from the press.

I suppose in the future I could even run this old version of Softmaker in a virtual machine and replicate this trick.

## Copyediting and the FALD
Copyediting continues to be a major hurdle to the FOSS Academic Lifestyle Dream. While I've written many papers with collaborators over the years, when it comes to the peculiarities of copyediting, I have been repeatedly compelled to throw my workflow out the window and adapt. In the past, this was a minor inconvenience -- just use Word for a weekend! 

But now? Now it means agreeing to have my work be the property of Microsoft's cloud services. Companies like Microsoft are simply claiming more and more power over the things we make. And given everything going on -- particularly in the USA -- I don't see that changing before I finish up my next book. 

