I ran into a problem in the FOSS Academic Lifestyle Dream today: for some reason, my spellchecker in Libreoffice Writer either stopped working or wasn't installed in the first place when I migrated to Manjaro.

Having used Libreoffice for years, I went into this problem with all the confidence in the world. And I came out on the other side a broken human, losing faith in the Libreoffice community. 

I first went into the Tools menu to set the language, thinking I must have not done that. But, no, the language was set (English (USA), in my case.)

I then wondered if it was a bug in Manjaro, or if it was otherwise a side-effect of my using Manjaro's Libreoffice-Fresh packages, which I assume keeps me on the bleeding edge of Libreoffice releases. So I started DuckDuckGoing combinations of "Manjaro" and "Libreoffice spellcheck" and found that, indeed, there are cases of people who are using Manjaro and have experienced this. "Well, there's your problem," I think to myself. But the solutions offered -- use pacman to install hunspell and hypen-en -- didn't solve the issue, either. 

I finally started poring through forum threads to figure out other issues. I'll spare you the details, but the ultimate solution was going to Tools -> Language -> More Dictionaries Online and installing the English dictionary. I've never had to do that before, and I'm not sure why I did here -- maybe it's due to the Libreoffice-Fresh aspect? But in any case, red squiggles are in their proper place again.

PRoblems, though:

arrogant dork: https://ask.libreoffice.org/t/automatic-spell-check-not-working/36781
(to be fair, another member asks them not to say that)

spell check is not a good idea: https://ask.libreoffice.org/t/can-not-set-text-language-for-spell-check-in-libre-office-version-5-1-4-2/20257/2
