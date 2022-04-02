---
layout: post
author: RWG
title: Review of Zotero's New PDF Annotation Features
tag:
  - Zotero
  - Goal 1
comments:
  show: true
  fedihost: scholar.social
  fediusername: robertwgehl
  fediid:
---

*UPDATE in 2022*: I've added the ability to comment via Mastodon on this post (see below) since this post is one of the more popular ones on the blog.

Zotero recently announced two major new features: an internal PDF reader and tab-based navigation. These are scheduled to be a part of the Zotero 6 release later this year, but when I heard about them, [I installed the Zotero 5 developer version](/2021/03/19/cuttingZotero.html) to give them a whirl.

<figure>
    <img src="/assets/images/zotero.png" alt="Zotero's Logo">
</figure>

My quick take on the new features? They are now a key part of the FOSS Academic Lifestyle Dream.

<!-- more -->

The Simple Pleasure of a Tab
----------------------------

First of all, opening a PDF in Zotero now opens its own native PDF reader with new annotation capabililties. I'll get to that. But first, I did not realize how happy one tab could make me.

The PDF now opens in a new tab, where I can read it and take notes. What's so cool about that is that I can easily go back to the main library and look at another source. I didn't realize how often I did that, but it makes sense: the PDF I'm reading might make reference to another source, so I might want to go back to my library to see if I have it and cross-reference ideas. Or maybe I don't have it -- I can pop into Firefox and get it easily enough. All the while, the PDF tab is waiting there, patiently, for me to return to it. 

I can even open a second PDF in another tab. 

<figure>
	<img src="/assets/images/zoterotab.png" alt="Zotero's new tab interface">
	<figcaption>Zotero's new tab interface</figcaption>
</figure>

This feature is great, and it makes me want more: could I eventually open search folders in a new tab? Group libraries? If so -- managing my library will get so much easier.

Taking Notes
------------

As for taking notes, the new PDF system offers a subtle, yet, invaluable capability: when I highlight text in the PDF, a button appears, allowing me to paste that highlighted section in a note. *And the pasted material doesn't have carriage returns.* 

So nice.

For years now, I would copy and paste PDF text into a Zotero note and have to go through and delete carriage returns. It could take so long that often I would just re-type the text rather than copy and paste it. This new setup will save me a great deal of time.

But there's more -- the pasted material has a citation at the end, allowing me an option to "Go To Page." Clicking on that citation does what it says -- it jumps to the page of the PDF. In addition, I tested this feature without a PDF open: clicking on it opens the PDF associated with the note in a new tab and jumps to the page. That's a fantastic feature.

<figure>
	<img src="/assets/images/zoteronote.png" alt="Automatically generated citation in a Zotero note">
	<figcaption>An automatically generated citation in a Zotero note. Clicking on the citation allows you to go to that page in the PDF.</figcaption>
</figure>

One thing that would really make this feature sing is this:
* I open a note and see a PDF citation, but the PDF in question is not open;
* I click on the citation and click on"Go To Page";
* The PDF *and* the corresponding note open in a new page.

In addition to the new note feature, the PDF annotation system has PDF highlighting and sticky note capabilities. Both the highlights and sticky notes can easily be added to a separate note, as well. The sticky notes can be tagged. There's a lot of new possibilities for library navigation now thanks to tagging sticky notes.

And, it looks like my location in a PDF was synced across devices. When I opened a PDF I was reading on a laptop at home on a second computer at work, I was dropped in exactly where I left off reading on the laptop.

In fact, these new features are so rich, I feel as though I'm barely scratching the surface. 

Bugs
----

Being beta software, I understand that there will be bugs. And there are.

First of all, the note window is pretty laggy. It often gets unresponsive while I'm typing. That can be frustrating -- it reminds me of the early days when Zotero broke out of being a Firefox-only add-on and went "Standalone." Zotero's "snappiness" improved over time, and I imagine the same will happen here.

Second, adding a chunk of text from the PDF to the note creates a new paragraph, rather than placing the text snippet on the current paragraph. 

Finally, the cursor seems to get lost when navigating the note with the keypad, especially when the cursor traverses the citation field. 

Features Lost
-------------

And there's unfortunately a feature lost in notes: the new note system does not allow for HTML editing, nor does it currently have the old highlighting. Looking at the [comments in the Zotero forum](https://forums.zotero.org/discussion/88064/available-in-preview-zotero-pdf-reader-and-new-note-editor), HTML editing is not coming back, since the notes won't use HTML. 

However, I put in a feature request, asking for a return of the highlighting option, and it sounds like the Zotero crew will implement that feature.

Overall Take
------------

 Due to the lagginess in note-taking, for anyone interested in these features but in the middle of important projects, I do recommend waiting until the Zotero 6 release. I'm in between projects, so lagginess in note-taking is not a big concern for me. 

But if history is any guide, the good people at Zotero will optimize these features for speed, and then this will be the biggest shift in how we interact with Zotero since it went "Standalone." I'm already using these changes and benefiting from them, and I'm quite certain other academics will, too.
