---
layout: post
author: RWG
title: How Universities Lost the Internet
tag:
    - Goal 1
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 111387781311156195
---
My first full-time academic job was at the University of Utah. Utah is, of course, very famous. No, not because of [cold fusion](https://en.wikipedia.org/wiki/Stanley_Pons) or teaching Ted Bundy about the law.

It is famous because it was the [fourth node on the ARPAnet](https://it.utah.edu/node4/posts/2017/august/node4-history.php), the forerunner to the modern internet. The other three nodes were in California; connecting to Utah was a major test of the network's ability to work across long distances.

Although it was a US Defense Department-funded project, the ARPAnet was a [playground for academics](https://ieeexplore.ieee.org/document/5432117) who took its mission (command-and-control even in spite of a nuclear attack) and turned it into research into networking and collaboration. The pattern continued: academic exploration of computer technologies has produced a bewildering array of experiments, and no doubt students at institutions have benefited greatly from being able to play with local, experimental computer tools while they study.

Fast forward to the early 2010s. I'm working at Utah, hired in part to teach a Web design class to Communication majors. Simple enough: each and every person affiliated with Utah had their own domain (something like domain.utah.edu/~username) on a local server, complete with FTP access via their email credentials. I taught students the basics of HTML and CSS. I got to see students who were openly scared of coding make things that appeared on their screens -- and on the internet. It was fun!

Until it was not. I was at Utah from 2010 to 2020. Over that time, it became harder and harder to get students into their web space. It turns out that Utah was winding down web hosting for everyone, centralizing its web presence and no longer providing web space to anyone. To support our class, the IT folks helpfully carved out some space on a server, specifically for our Comm Intro to the Web Design students, but we knew this was an exception.

At the end of my time there, even the machines in the computer lab were outsourced. Instead of fully-functional desktops, students were accessing their servers over a convoluted "thin client" computer lab setup. I had to spend the first 2 weeks just showing them how to find their files -- since they were no longer local -- and then FTP into a server to move those files over a client-to-cloud-to-FTP setup. This was for students who had no networking or web design experience -- it was _rough_. (And if we needed software -- such as basic text editor -- good luck getting it when all the software was on a cloud somewhere).

I'm sorry to say I spent a great deal of that time in an increasingly adversarial relationship with the IT folks.

As this happened, my colleague [Sean Lawson](https://seanlawson.net) and I would vent our frustration by jokingly saying, "Welcome to Node 4!" The irony being that Utah was once _25% of the freakin' Internet_ but we could not get easy access to basic Web hosting. It was an ordeal just to get students to the point where they could move a text file they were working on to a server.

Fast forward to today. Now, I am happily employed by York University in Toronto. But just the other day, my colleagues met for a faculty meeting, and we discussed recruiting students. Someone suggested we post information about our faculty to our department website and social media. "No," the chair said. "All of that would have to go through the central administration" -- the implication being either it wouldn't be allowed, or that it would take months to achieve.

## Someone's Gotta Write This Book

I would propose, were I to have time, to write a book called "How Universities Lost the Internet." How did we get from many nodes to everything being dumped into California or Redmond, WA? How did we get from a system of experimentation to seeing digital media as a controlled environment to market a brand? How did we get to the point where university core functions were run by for-profit firms?

It would be a fascinating book. (Someone else can write it, though; I'm too busy with [my current project](/2023/08/17/OxfordUP.html)!)

<!-- more -->

I think there's quite a readership for this book, judging from a recent thread on the fediverse. I posted this [proposed book idea on Mastodon](https://aoir.social/@rwg/111308895829845440) a few days back:

> Does this book exist? "How Universities Lost the Internet"?
> Or has someone done research on this topic? That is, the fact that many North American universities have ceded all technical capacity to Microsoft, Google, etc?
> It used to be students could get web hosting, email, and even some cool experimental online stuff through their schools. Now every online communication channel is locked down.

The response to my fediverse post was pretty intense. I'm not going to directly quote any of it here because I did not ask permission of the respondents (and of course you can see public comments if you follow the above link), but I will sum things up:

* University IT is being outsourced across the board. Instead of local email, storage, or HR systems, these services are subdomains of a corporate site, e.g., https://yorku.zoom.us/, or even just simply note affiliated with the university at all (e.g., when I login to York webmail, the domain is office.com and there is no York branding).
* This is a global phenomenon. I originally mentioned North America because that's the context I know, but folks from universities the world around have observed the same thing.
* For universities outside the USA, the outsourcing is doubled: they're not only outsourcing things from the university to outside third parties, they're outsourcing to companies outside the country.
* The reasons given for this shift vary. In some places, faculty and students are told this is done for security purposes. In others, they are told it's done for cost-cutting reasons. And in others, they're told it's done to protect the university's brand.
* Timelines also vary. The pandemic sped things up, but such outsourcing has been going on for a while. Some note it began at their institutions as early as the 1990s.
* There are some bright spots: university-hosted Git repositories and local file storage are mentioned.

While I didn't hear that the book on this shift exists, people helpfully pointed out [this article on the "Zoomification" of higher education](https://arxiv.org/abs/2104.09462). Poking around, I also found a [book review essay](https://www.insidehighered.com/opinion/blogs/learning-innovation/2023/09/01/recoding-america-and-perils-outsourcing-it) lamenting this process, a report in the [Washington Post](https://www.washingtonpost.com/local/education/colleges-outsourcing-services/2021/01/07/c3f2ac6a-5135-11eb-bda4-615aaefd0555_story.html), and a [Guardian Australia investigation into outsourcing](https://www.theguardian.com/australia-news/2023/mar/07/australian-university-outsourcing-how-can-i-tell-if-my-online-course-is-being-run-by-a-third-party).

The topic is definitely getting attention. Someone outta write a book.

## Why I Care About This
Readers of this blog know I care about communication infrastructure pretty deeply. Goal 1 of my blog is to [document the life of the "FOSS Academic"](/2020/11/27/introduction.html) -- my attempt to do most or all of my professorial work using FOSS tools and self-hosting. I use Nextcloud for document sharing, collaboration, and conferencing, Zotero for managing bibliographies, Thunderbird for managing emails and calendars, Libreoffice for writing. I use Syncthing, Wireguard, and Nextcloud on a local network to move data from home to office. Of course, all of this is running on Linux machines (Manjaro KDE, if you're curious).

For the most part, this has worked, but I am sorry to say it's increasingly hard. Zoom is a big culprit, of course, but I've accepted that. (I use [Nextcloud Appointments and Talk pretty often](http://localhost:4000/2021/09/25/Appointments.html), however).

What I didn't bargain for was how powerful Microsoft has become. Outlook, Teams, Sharepoint, Office. The assumption among my colleagues is that I use all of these regularly. I get why they think that -- it's what's provided. But I'm starting to get pressure to put my calendar on Outlook, since people assume that if my Outlook calendar is open, I can meet. Whenever my colleagues want to work on documents, it's in Office online, not a draft passed back and forth. And all of my department's governance runs through Teams (a program so awfully designed it wastes time -- I can hardly find anything in it).

I'm trying to hold onto my FOSS, self-hosted network as a living experiment -- maybe if I can hold the line, chip away at things, convert a colleague or two to the "FOSS Academic Lifestyle Dream" -- maybe we can find an alternative to this mess.

But given that university IT outsourcing is a global phenomenon, I'm starting to lose hope.

## Lost Creativity

Perhaps the biggest reason I'm concerned, however, is not just about my day-to-day work, but because of the loss of skills and experiments such outsourcing causes. This is the point of the [book review essay I cited above](https://www.insidehighered.com/opinion/blogs/learning-innovation/2023/09/01/recoding-america-and-perils-outsourcing-it), in which Joshua Kim uses a book about US government IT outsourcing to lament the loss of IT skills in universities, as well as the reduction of University IT to mere "support services."

What I would like to see is universities providing infrastructure for students and faculty to do interesting, creative things. I'd like to see this done for _all_ students and faculty, not just sequestered in computer science or engineering departments. I'd like to see folks be able to do everything from making websites to local document collaboration to running their own social media. On this latter point, there are efforts, notably in [Holland](https://www.surf.nl/en/mastodon-pilot-for-research-and-education) and at [MIT](https://mastodon.mit.edu/about). But I worry that these are exceptions, not the rule.

More than that, I would like to see universities run their own IT again, seeing it as central to the pedagogical mission, not just another budget line to cut.

## Did you write this book?

Finally, to repeat my question above: did someone write this book and I just missed it? Hey, let me know: I'm buying!
