---
layout: default
---

## Command line tools for Linguists
### KIK-LG221 | Fall 2026
This course instructs users in the basics of Unix command line usage, with no prior required knowledge.
I had some passing experience with a variety of programming languages and some proficiency with rudimentary computer science to start with, so the course was not too taxing.

As a note, if a teaching assistant is reading this: it might have been nice to instruct the students to gather some reflection along the way! Attempting to reflect on a weekly or by-module basis a month or so later unfortunately feels equal parts difficult and pointless.
I've also quite completely lost track of which module was supposed to be which week; I hope you can forgive me segmenting this page by module rather than by week, as the final assignment spec requested.

#### Module 1: introduction
Beginning with installing and getting to know our way around a command line environment. I opted for the WSL Ubuntu environment, as I am already using Windows 10 and 11 computers in daily life, and I do not expect to use UNIX enough to warrant setting up a parallel-boot Linux. The module introduces the peculiarities of the UNIX file system and some basic, but essential commands; `cat, less, head, tail` for peeking into files would prove to be in nigh-constant use from now on.
Similarly, one couldn't survive without basic directory management tools such as `cp, rm, mkdir, cd, ls`. I stumbled upon the (to me) much more preferable `tree` package as well, which I tended to use much more frequently than `ls`.

#### Module 2: text processing
Regexps, csv:s, `sed`, piping. Coincidentally, while going through this material, I needed to do a bunch of simple text manipulations, such as extract, sort and format lists of names from an excel file. What a perfect practice opportunity! A quick .csv export, a quick `cp` from `/mnt/c/` and a (bit less) quick `sed 's/, /\n/g' file.txt | sort > file.sort.txt` later, a sheet of...
* Aapo K.. 
* Aapo P..
* Anki A..
* Astrid K..
* (and so on for some dozens of lines)

... had turned into a neat list of names ready for inserting into other text for further processing. I must admit, some command line magicks were supremely convenient for these kinds of simple tricks.

#### Module 3: scripts, config, sudo and python
Pre-acquired familiarity with Python made this module simpler on one hand, more complicated on the other (before getting used to venvs, when there were just too many conflicting installations of different pythons competing for attention!)
I did quite enjoy fiddling with stuff in my `.bash_aliases`, such as shortcuts to various coursework directories and a snappy little `alias KIK-venv="source $HOME/KIK-venv/bin/activate"` to get right into it with the python version for this course.

#### Module 4: remote connections and version control
Most of the time I spent on this module was spent working _around_ the deprecated course materials, such as the instructions on gaining access to CSC remote servers being written for `puhti` which was no longer available, and the process of gaining access into `roihu` being _quite a lot_ more involved than the course material presumed.  
It's kind of amazing that I've previously managed to graduate as a B.Sc. without ever touching git or github properly before this course! Better late than never, I suppose. Here, again, quite a lot of effort was spent on working to gain ssh access to my (pre-existing but not really used) github account, since github had deprecated username-password-authentication.

#### Final Assignment: building a page
It came as quite a surprise that the majority of effort required for the final assignment of a course ostensibly focusing on the basics of a UNIX command line would be spent on the basics of LaTeX and Overleaf to build a CV, which isn't going to be in a presentable state after this at any rate; seems like a wild swing off-topic.  

