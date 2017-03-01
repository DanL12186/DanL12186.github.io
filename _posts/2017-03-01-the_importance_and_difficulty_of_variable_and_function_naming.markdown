---
layout: post
title:  "The Importance (and Difficulty) of Variable and Function Naming"
date:   2017-03-01 21:48:50 +0000
---


Variables and methods (and constants!): They hold and manipulate our data, and form the bulk of our programs. We should, therefore, treat their naming as important, and go about the process thoughtfully.  For me, and I imagine for many others as well, I find the cognitive burden to be greatly lessened when variable names, rather than being called "a" or "b", or "var1" or "var2", describe precisely what they're holding. Similarly, when functions (and methods) are named for precisely what they do, things become much easier. 

But how to accomplish this? In theory, it sounds pretty straightforward. But I've found in practice it can be a bit trickier than anticipated. For my own personal tastes, I find it best when code reads as much like plain English as possible. So rather than, for example, a generic variable.method invocation like music.iterate_add, to iterate over an array of songs or song objects and add them to a collection, I find something like music_library.add_to_collection much clearer, although admittedly not perfect. 

But not everyone is going like this particular set of names, and when we program in the real world, we tend to be working with other people. As a result, this is no small issue. I've often found when looking at others' code (including some of the labs we've done) that I have a strong desire to rename variables or functions (and that when I do, things suddenly become much easier). For some, perhaps, the function or method's name is the most important; so "music.add_music" might be preferable to them ("add_music" clearly states what it does, while "add_to_collection" is less specific outside the context in which is it used). 

I find myself sometimes struggling with some of the same issues Wikipedia mentions on the subject of naming convention:

Some considerations:
-Shorter identifiers may be preferred as more expedient, because they are easier to type
-Extremely short identifiers (such as 'i' or 'j') are very difficult to uniquely distinguish using automated search and replace tools
-Longer identifiers may be preferred because short identifiers cannot encode enough information or appear too cryptic
-Longer identifiers may be disfavored because of visual clutter

It seems to be a question of balance between conciseness and descriptiveness. Too short and abstract, it becomes harder to remember what everything is doing. Too verbose, your code can quickly become cluttered and visually difficult to parse. 

The goal, at least as I imagine it, is to have things named such that anyone with more than a few minutes' familiarity with the code should be able to use your methods (almost) as if they were part of the language's standard class methods.

So what, then, is the best solution in terms of naming variables, methods, functions and constants that works for you and everyone else? 

...I'm still working that out..
