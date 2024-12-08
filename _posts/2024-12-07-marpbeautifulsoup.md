---
layout: post
author: RWG
title: 'Marp + BeautifulSoup'
tag:
    - Marp
    - beautifulsoup
    - goal 1
comments: 
  show: true
  fedihost: aoir.social
  fediusername: rwg
  fediid: 113615434906488351
---
The FOSS Academic Lifestyle Dream just got a bit dreamier.

Previously, [I wrote about Marp](/2024/12/01/marp.html), which is a [Markdown-based way to generate presentation slides](https://marp.app/). When I wrote about Marp last, I was speculating that it would be very useful:

> I’m going to do it: I’m going all-on on Marp for a while....  I suspect Marp is a future fixture of the FOSS Academic Lifestyle Dream.

Well, it's true. On Friday, I gave a presentation over Zoom using a Marp-based slide deck. You can [see the files here](https://robertwgehl.org/presentations/ITS_presentation.html). It worked wonderfully!

And I did something more. Marp produces responsive, semantic HTML. HTML can be parsed with [BeautifulSoup](https://www.crummy.com/software/BeautifulSoup/), a Python library.

<!-- more -->

Marp enables me to easily add slide notes with basic HTML comments, like this:

```
<!-- Slide notes go here -->
```

After Marp processes the Markdown file and converts it into HTML, I could see that those comments with a class, "bespoke-marp-note." Which means I could pull out all the notes directly from the HTML and create a new file, with the notes only, with BeautifulSoup.

I'm no programmer, but I can search for guides with the best of them. I wrote a python script to pull the comments and produce a second HTML with just my script. [Here's the result](https://robertwgehl.org/presentations/ITS_presentationText.html).

This gives me a great time-saver: instead of writing a script and creating the slides separately, I just do it all in one Markdown file, and the scripts generate everything I need from that single file. This will save hours of work!

Another nice thing about this is that I can share the text of my presentation easily over the web. Prior to this, I rewrote the presentation as a new Markdown file and posted it to the blog. That would add hours to the task. The new way will be automated!

Here's the Pyton script I wrote (if you see poor coding on my part, be gentle):

```
from bs4 import BeautifulSoup as BS
from bs4 import Comment


import requests
import getopt, sys

# This gets the system argument, which should be the Markdown file I'm exporting
filename = sys.argv[1]

# strips the final three characters, '.md', from the file name
filename = filename[:-3]

# changes file name for text
filenameText = filename + 'Text.html'

print(filenameText)

# adding local HTML file
with open(filename + '.html') as f:
    soup = BS(f, 'html.parser')

# parsing notes
# this will add a header, print to file

i = 0
presentation = (soup.find('h1'))
content = '''<html>
<body>'''
content += str(presentation)

# this will add slide headers and the notes

for note in soup.find_all(class_='bespoke-marp-note'):
  i += 1
  content += '<h2>Slide ' + str(i) + '</h2>'
  content += str(note)
content += '''
<!-- Some javascript here -->
</body>
</html>
'''

# Writing the content to an HTML file
with open(str(filenameText), 'w') as file:
    file.write(content)
```

You might notice a variable, "filename = sys.argv[1]". That is there because I wrote a bash script, exportPresentation.sh, to automate the whole export process:

```
#!/bin/bash
~/.local/share/marp/marp --theme ./CSS/custom.scss --html $1
python pullComments.py "$1"

```

That little script invokes marp-cli to convert the Markdown file, and then the python script recieves the file name (e.g., I'd type "sh exportPresentation.sh presentation.md" into the shell).

Again, much like using CSS to build a presentation, coming up with these scripts took a bit of time, but in the long run, I'm making presentation creation -- and sharing! -- that much easier.
