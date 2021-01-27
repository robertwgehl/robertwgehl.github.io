---
layout: post
author: RWG
title: My Workflow
tags:
---




My workflow



devilspie
----------
Devil's Pie. It's not just [a documentary about the R&B singer D'Angelo](https://www.youtube.com/watch?v=EgvE6c7-2ag). Devilspie is a [small application](https://help.ubuntu.com/community/Devilspie) that gives me total control over how applications load into various workspaces.

On my typical MATE setup, I have 6 workspaces. I'm old-school, so I set them up horizontally in a top panel. I also set my keyboard shortcut to CTRL+Left or Right to switch between them. 

One of the first things I do is install devilspie and set it to run on startup. 

Devilspie works with scripts stored in ~/USER/.devilspie. Each application requires its own script (saved in .ds files). For example, my Firefox script is:

<pre>
(if (is (application_name) "Firefox") (set_workspace 3))
</pre>

That line is in a file called firefox.ds, and as you might have guessed, opens Firefox in Workspace 3. Now, no matter where I open Firefox, it gets pinned to workspace 3, and is at most a couple CTRL+direction keystrokes away.

Using similar techniques, I route my applications to the same places -- Zotero, the citation manager, goes in Workspace 1. My "comms" workspace is 5, with Evolution email and chat applications routed there. Entertainment (music players, video players) goes to 6. Terminals and my IDE (currently Brackets) goes to 4.

With the exception of Brackets going to 4, most of my writing goes into Workspace 2. I route Libreoffice there, as well as my PDF reader. I also use some rules to move Zotero notes to Workspace 2. Devilspie allows me to control window geometry, so I set my PDF reader to 2/3s of the screen and a Zotero note to the remaining 1/3. Devilspie even supports ["always on top"](https://itsfoss.com/always-on-top/), though I don't use that much.

I'm a bit concerned, however. The original devilspie is [apparently no longer being maintained](https://wiki.gnome.org/Projects/DevilsPie), and neither is its successor, [Devilspie2](http://www.nongnu.org/devilspie2/). I hope these handy applications stick around!

But for now, with devilspie and the corresponding rules in place, when I launch an application (in my case, using [Synapse](https://www.fossmint.com/synapse-application-launcher-and-file-search-tool/), which appears with CTRL+Space), I know exactly which workspace it's routed to. I can flip between a browser and a writing application with a keystroke -- cutting, pasting, and so on. 

Pomodoro
--------
In fact, switching from my writing space (Workspace 2) to email is now *too* easy. I find myself flipping over to email too often, and for no good reason. Because of this, I close Evolution, but to really help me focus, I also use the [Pomodoro Timer for Gnome](https://gnomepomodoro.org/). 

I find the [Pomodoro Technique](https://en.wikipedia.org/wiki/Pomodoro_Technique) to be a simple and effective way to stay on task. It starts with a conscious decision to say "I am working on this task." Then, I start the timer (set to the default 25 minutes) and do it. After 25 minutes, the Pomodoro Timer takes over my screen and says, "Take a break!" I take the 5 minute break to stretch, do some pushups, move my limbs. And then: back at it for another 25. If I do four Pomodoros, I take a longer, 15 minute break, usually by walking around campus.

The nice thing about this approach is that it is open-ended. If I have a stack of emails: that's the task. Once that's done, I can switch to grading, or writing. 25 minutes seems like a good amount to knock out a lot of things.

But how to decide which tasks need be done?

Cal Newport's Weekly To-do List
------------------------------

I don't think Cal Newport came up with the [weekly work plan](https://www.calnewport.com/blog/2014/08/08/deep-habits-plan-your-week-in-advance/), but I give him credit because I first learned it from his blog. As he writes,

<blockquote>
    On Monday mornings I plan the upcoming work week. I capture this plan in an e-mail and send it to myself so that I will be sure to see it and have access to it daily. (See the snapshot above of some recent plans in my inbox.)
</blockquote>

I used to do it via email, but now I put a task in Evolution. Every Monday morning, I spend about an hour assessing what I need to get done in the week, and then I develop a weekly schedule with time blocks allotted to the various tasks. I set the task to be "due" on Sunday. I don't actually look at it then; I instead look back on last week's plan on the subsequent Monday morning, reflecting on what I got done in the previous week. I also use the Sunday deadline to see if any tasks in Evolution are due *sooner* than my weekly schedule -- that means those tasks are high priority for the week.

At the top of my weekly plan I list out projects I'm working on. Usually, these are long-term projects which require daily work to maintain progress towards deadlines. 

I think break the week down by day and assign blocks of time (typically an hour or two) as time to drive towards completing those long-term goals.

A week then looks like this:

<pre>
2020 December 13

//Research
* WP met Tor
* Mastodon
* JOC
* DNS

//Teaching
* Comm 431:
        - Build at least one more week
        - grading
* Comm 101
        - find podcast episode
        - grading

//Service
* NMS review

-------------------------
Monday 13 Dec

2 hours DNS research and writing
1 hour Comm 431
1 hour Comm 101

-------------------------
Tuesday 14 Dec

2 hours DNS research and writing
1 hour Comm 431 grading
1 hour NMS review

-------------------------
Wednesday 14 Dec

...etc, etc
</pre>






