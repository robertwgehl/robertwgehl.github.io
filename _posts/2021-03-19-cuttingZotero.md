---
layout: post
author: RWG
title: Cutting-Edge Zotero
comments: true
tag:
    - Zotero
    - FALD
    - Goal 1
---

There's exciting news on the Zotero front!

Zotero just announced a [preview of their new tab system, complete with a built-in PDF reader](https://www.zotero.org/support/pdf_reader_preview).

For anyone living the FOSS Academic Lifestyle Dream, this is huge news.

<figure>
    <img src="/assets/images/zotero.png" alt="The Zotero Logo" title="The Zotero Logo">
    <figcaption>The Zotero logo is in the public domain.</figcaption>
</figure>

They plan on releasing these features to the public in Version 6, but anyone itching to try it can use the development version of Zotero. This post will discuss how to install Zotero's beta in Ubuntu Mate 18.04, though the approach should be similar for other Linux distros.

<i>NB: Note, I would have found this sooner or later, but credit to Sean Lawson for alerting me!</i>

<!-- more -->

Step 1: Shut Zotero Down and Back It Up
---------------------------------------

First, make sure you're not running Zotero. You can still have your browser open, however -- the Zotero plugin will not affect this step.

After shutting down, navigate to your Zotero profile folder. You should see a zotero.sqlite file. Because switching to the Zotero Beta could cause irreversible changes to this database, it's best to back it up.

<figure>
    <img src="/assets/images/zoterosqlite.png" alt="A screenshot of the Zotero folder and zotero.sqlite file">
    <figcaption>The Zotero folder and zotero.sqlite file in Caja, Mate's file browser</figcaption>
</figure>

I also backed up my installation of Zotero's program files. Out of habit, I put them in a folder called "zoteroStandalone" in /.local/share. I simply created an archive of that folder and then deleted its contents. This is going to be my target for the Beta version.

Step 2: Get the Beta
--------------------

I then downloaded the [beta version of Zotero](https://www.zotero.org/support/dev_builds) from their Dev Builds page. It's in a compressed archive. I unpacked the archive in my now-empty /.local/share/zoteroStandalone folder. 

<figure>
    <img src="/assets/images/zoterostandalonebackup.png" alt="A screenshot of my .local/share folder with zoteroStandalone's directory in it">
    <figcaption>I store Zotero's executable files in /.local/share/zoteroStandalone</figcaption>
</figure>

At this point, since I've been using Zotero for a while, I could then just launch Zotero from Mate's Brisk menu and it was up and running. But, in case any of you want to know how to add Zotero to your menu, see the next step.

Optional Step: Add to the Brisk Menu
------------------------------------

To add Zotero to Mate's Brisk menu, right-click on your menu and choose "Edit Menus."

I like to add Zotero to the "Office" subcategory.

<figure>
    <img src="/assets/images/briskmenu.png" alt="A screenshot of Mate's Brisk menu editor">
    <figcaption>Brisk Menu editing starts with selecting where you want to add your menu items.</figcaption>
</figure>

Then, select "Add Item." You will see a menu like so:

<img src="/assets/images/addingmenuitem.png" alt="Adding an individual item to the Brisk menu">

Because I stored Zotero in my /.local/share folder, the command path is /home/robert/.local/share/zoteroStandalone/zotero. To add an icon, I click on that springy Mario Brothers-looking icon and navigate to /home/robert/.local/share/zoteroStandalone/chrome/icons/default/default256.png.

Now, I can launch Zotero from the menu.

If you've done all this and installed the Zotero beta, perhaps you're as curious as I am about the new tabbed interface and PDF reader. To get those features, you have to opt-in. 

<figure>
    <img src="/assets/images/betaoptin.png" alt="A screenshot of Zotero's general preferences menu">
    <figcaption>Here is where you turn on magic things.</figcaption>
</figure>

To do that, go to Edit -> Preferences and use the General Tab. There's an option about halfway down the menu to opt in. After a restart, Zotero will have the new features.

I just did this process minutes ago, so expect a follow-up post on using the new features soon!

In the meantime, if you're looking for Zotero tricks and tips, [check out this post](/2020/12/01/Zotero-Tips-and-Tricks.html).
