---
layout: post
title:  "Final Sinatra Portfolio Project"
date:   2017-04-16 00:20:58 -0400
---


This final project has been mostly an enjoyable experience. Most of the issues I'd been having with Sinatra that I talked about in my last blog post (particularly understanding setting params hash via name= and mentally navigating routes) were ironed out almost immediately after posting that. 

That made things go quite a bit more smoothly for the lab that preceded this one, which instead of taking a day and a half was done in probably eight hours (still quite a long time, but I spent a *lot* more time tweaking parts of it and getting sidetracked on programming tangents than I had to). 

The vast majority of the work was done today; I laid some of the groundwork yesterday and the day before, but didn't actually have a lot of time (or ability to concentrate) until today. Once again, I will admit to allowing myself to be sidetracked probably more than I ought to have (I spent quite a bit of time reading about password security and algorithms, adding code and features I didn't need to, and testing the randomness of Ruby's RNG (rand) function in OS X's Terminal), but I figured it's all Ruby-related, so the only real harm done is that I'm currently exhausted and it turns out I'm not quite as done as I'd thought... I hadn't noticed the spec.md until the end, which upon reviewing, mentions error messages as a requirement-- something I'd decided against even while seeing it in the example project because, truthfully, they didn't seem to do much. (I'm not sure if the app is a little broken or not, but for me, at best I get a little error message in the URL, which doesn't seem especially useful.) 

My first reaction to the lab was actually that it didn't really seem to be very substantive. I went through the example site and there just didn't seem to be much there-- less, in fact, than on the lab prior. As a result, I probably made parts of it more complicated than I had to to compensate for what felt like a lack of a challenge, which in the long run made things more difficult in the end (and, as mentioned above, I let myself get sidetracked reading about other tangentially-related things).

I found tux very useful for this project. It let me see how some of my associations were working, and I was able to determine that deleting a book didn't automatically delete the characters that belonged to it, so while this didn't affect the web app itself, it did leave my database with a bunch of orphaned children from testing creation/deletion. I was then able to pretty easily figure out how to get rid of both. 

I will confess to not especially looking forward to having to tack on the error messages to my code (it's not really very apparent how it works, and I don't really feel like just copying and pasting, so it's going to be some time spent in pry and purposely generating all the same errors I've already tested), but I'm pretty confident it won't take too long once I'm not half-asleep and burned out from staring at the same project all day.

Still though, all in all, this was a pretty good experience. I'm looking forward to Rails.
