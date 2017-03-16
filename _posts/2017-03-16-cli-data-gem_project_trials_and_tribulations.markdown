---
layout: post
title:  "CLI-Data-Gem Project: Trials and Tribulations"
date:   2017-03-16 20:10:17 +0000
---


I will admit that getting this particular project up and running has taken me longer than I would have liked, and that there were periods where I experienced a very great deal of frustration. 

That said, I'm genuinely *very* glad this project was mandatory, and I'm glad that I wasn't able to simply breeze through it in a day or two.

By far my biggest hurdle was the scraper itself. Not the act of getting the selectors right, or working with Nokogiri and Open-URI, but in figuring out how to encapsulate the functionality into a method that then properly iterated over each necessary piece and stored them all as objects.

Perhaps somewhat ironically, I had expected this to be the easy part. But what I found was that I really didn't know how to go about it. The previous, related labs (oo-student scraper, e.g.) were working with hashes, not proper objects, and I found myself not knowing how to start, and trying to both imagine and hold the entire program in my head at once while attempting to account for all the things I was uncertain about, which unsurprisingly, proved impossible.

I quickly became convinced that without a pre-written spec which someone else had made for me, I was incapable of programming, and that, as I had feared, when multiple classes were introduced across multiple files, and the interconnectedness and complexity of interactions between variables and methods and files reached a certain point, I simply lacked the requisite cognitive ability to program.

This was, perhaps predictably, very distressing. I have been worried (on and off) that my near-inability to visually retain information in my head would eventually prove an insurmountable problem when it came to coding, particularly with objects, and I became nearly certain that this was the case. 

I tried unsuccessfully for three or four (or five?) days to solve the problem, and I couldn't make it work. The selectors had come almost instantly, none took more than a few minutes, and most took a few seconds. But I was stuck without any way to manipulate or iterate over that scraped data in order to store it. 

Where before even on tough projects I had made steady and usually rapid progress, I now found myself stuck at square one after days of fruitless effort.

Finally, I decided to stop trying to build it all at once (where it properly looped over each selector, scraped it, made an object out of it, saved it to a class variable and continued until the page had been fully scraped).

I made my way back to the OS X terminal, and decided to build one object (using the first movie listed on the page) manually. 

After very little effort (three or four minutes), I had accomplished this. So, I knew— as I already had known— that my code was capable of accessing the page, and given I knew exactly how to make one fully-functioning object manually (creating variables myself, adding object properties one at a time and invoking Class.new), I reminded myself that all I needed to add (in addition to a couple of tweaks to go from terminal --> a program file) was the loop.

As a result, instead of my mind jumping to a different topic while right in the middle of trying to solve a related but separate problem, I was able to focus on one thing at a time. I knew assigning an instantiation of my scraper class to a variable would work (as I always did whenever I worked in the standalone terminal), and so I did that. Through some trial-and-error in the OS X Terminal, I also finally realized that I had the wrong selector for the loop (something I had long forgotten about). I quickly found and entered the right one. From there, now able to focus on one thing at a time, I finally realized that I wasn't properly assigning the selectors in the loop, and fixed that. 

The scraper, which for days had done absolutely nothing, was now working in a matter of about an hour or less. 

The second hurdle was really all the file setup and bin/console/gem items and file dependency. I had started out building everything manually, and I couldn't even get the bin file to run. Finally after a few more days I decided to just redo it and follow the bundler instructions, and very quickly it was working (although the CLI hadn't really been built yet as I'd had no way to run it before).

Within a day I'd built out the CLI, which is now functional, fixed a bunch of issues and errors I was having, added some functionality and cleaned everything up a bit. 

There still is more to be done— refactoring and the visual output of the CLI, but by far the hardest parts (as far as I can tell) are done. 

Again, I'm pleased that this project was mandatory and unassisted. It forced me to confront an accumulation of things I was weak on or didn't really understand well, and work through certain issues I was almost totally clueless about (such as how to work with bin files and get the CLI working-- my partner did that part on the ttt-with-ai project as I had done most of the previous portions). 

I feel I learned a lot from this assignment, and I think it's likely that if I had been forced to learn all of this better and more solidly before, I would have progressed a *lot* faster through some of the more challenging labs. 

I am disappointed that there was so much time wasted-- I'd estimate that 85-90% of the time this project has taken so far was trying to make the scraper and bin file work at all (as well as days I was either busy or too tired to work on it). I think there's a very decent chance that had I started this assignment on a different day, things would have gone a lot more smoothly and taken a third or a fourth the time. But I'm still glad I had to struggle and work for it. 

I also think that the website I chose— MovieInsider.com— was probably not a very good choice. It wasn't set up especially well for scraping and presented its own set of challenges that other sites probably don't have (missing MPAA ratings, MPAA ratings stored in "mpaa-3" format instead of "PG/R" etc., missing summaries, two different *kinds* of summaries-- one usually used, one only sometimes used), etc. But I'm sort of glad I chose it, for similar reasons... it made it more challenging and added some complexity to the design. 

All in all, I'm pretty happy with how things turned out. I just— as mentioned— wish I'd gotten to the actual process of coding a little sooner.
