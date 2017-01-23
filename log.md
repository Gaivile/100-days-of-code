# 100 Days Of Code - Log

### Day 1: January 3, Tuesday

**Today's Progress**: Got back to an old project! Re-implementing data strucure in more Clojure-appropriate way.

**Thoughts** Looking back at how I've done the same things previously, it's interesting to see how more practice and experience can improve the way of thinking. Also, an hour a day seems doable so far. 

**Link(s) to work**
[0b1d1c3](https://github.com/Gaivile/breakout/commit/0b1d1c337f54769f640b6ed437e90a459d6ba6a6)


### Day 2: January 4, Wednesday

**Today's Progress**: Apparently, one hour is not enough when you get so much into a project! Today I'm continuing with data structures - got an idea how to represent a brick in Quil for collision detection. 

**Thoughts** I kinda desperately need to move to another editor... Bit of a shame - I'm still using LightTable - which is awesome at the very beginning stage as you can see the output of all the functions straight away and inside the editor. However, when you have a bit more dependencies - it refuses to work. Noticed this some time ago to be honest, and it's a "known issue". Where do I go...? What do I do...?
Emacs? Vim? IntelliJ? Sublime? Atom?

**Link(s) to work**
[ed663e7](https://github.com/Gaivile/breakout/commit/ed663e76a21eecd57e58b7d4708fc6cf90dc163d)


### Day 3: January 5, Thursday

**Today's Progress**: Built data structure (a map) to represent each brick as an integer (key) and nested lists of (x y) coordinates (values). Not sure if that's a good approach, as the whole structure becomes huge. At least, it only get's smaller.

**Thoughts** Still can't manage the time and hour/hour-and-a-half is definitely not enough. However, this brings happiness! It's like Clojure-zen-time. I forgot how much fun it can be to work on personal projects! 
And still thinking of editors. Tried IntelliJ at work, so far looks nice. Will try Emacs next Tuesday, can't wait!

Another thought - I'm embarrassed about all the mess I'm leaving in the code. I'd normally wouldn't push until I've cleaned it and would have another hour (therefore - another day) for cleaning up when done. But those are rules of #100DaysOfCode - so let's pretend it looks fine. =^_^=

**Link(s) to work**
[7786006](https://github.com/Gaivile/breakout/commit/7786006041040120a3ffc3ab9a9784197f40a6d7)
[e65039d](https://github.com/Gaivile/breakout/commit/e65039d269b307ae3bc9fe4440ace4a3bf26cbda)


### Day 4: January 6, Friday

**Today's Progress**: Didn't do much today - improved data structure so it's map keys are the coordinates of upper left corner of the brick. Should be easier to make collisions later. Started writing collision function.

**Thoughts** Code drunk - refactor sober. \m/

**Link(s) to work**
[5971c87](https://github.com/Gaivile/breakout/commit/5971c875af5b0787b3c9eea9d184c4fcbe2f7fac)


### Day 5: January 7, Saturday

**Today's Progress**: Cleaned up the majority of the mess so it's easier to understand what's going on. Done a bit of refactoring towards data structures (again - Clojure is all about data!), was reminded that nested anonymous functions are not allowed :) Left a few notes for myself what needs to be done next so it's easier to finish it later.

**Thoughts** Was a bit frustrating to work at first as the code was kinda messy. Note to self - clean up your mess! It's a lazy Saturday, so it's nice to work in a slower and relaxing pace - and still having something done. Also, I need to somehow learn/have a reminder to not overcomplicate things. Writing small and short functions and then connecting them together is way more easier and understandable than creating long and complicated ones. 

**Link(s) to work**
[84eb564](https://github.com/Gaivile/breakout/commit/84eb56415398b4c2cb1fa6c3363f5d799361f46d)


### Day 6: January 8, Sunday

**Today's Progress**: Today I've tried to put everything together how it's supposed to look like and run the game, and obviously - ran into new bugs. At first I've got a few exceptions, then got error in functions, but eventually, fixed those things. Game is running, however - bricks are not removed. And they can't be because I've stumbled upon a bug at (setup). Things to do next time: 
1) Fix data structure for the grid, possibly at (generate); 
2) Use new structure at (draw-bricks);
3) Work on collision detection.

**Thoughts** What works on small data structures - not necessarily works on bigger ones. Previously constructed map data structure doesn't work as expected on huge data sets. In (setup) function - functions are not called as expected as well (maybe, try (let) - and add the output as a structure...?). Will try to refactor (generate) - so it constructs the map straight away.

**Link(s) to work**
[45b8e5e](https://github.com/Gaivile/breakout/commit/45b8e5ed0d95f9929cb24c3702473d2957ac28e5)


### Day 7: January 9, Monday

**Today's Progress**: Today I was working on a different project - breakfast app which was started by my colleagues at work, but it's not really work-related. I was working with re-frame framework. I still am not really used to it or can use it comfortably, but it was a nice way to practice the framework. 

**Thoughts** It's obviously easier to work on projects you know by heart or have written yourself, but it's an invaluable experiance to work on a project, started by someone else! You can see the different way of thinking and can use different approach on the future projects. It can be hard or even frustrating sometimes, but totally worth it - and really rewarding too. And I've just noticed - it's already a week of #100DaysOfCode! 

**Link(s) to work**
[92c4ef5](https://github.com/Gaivile/breakfast/commit/92c4ef56a3c6660e769e0edb2103d06b75b5db2c)


### Day 8: January 10, Tuesday

**Today's Progress**: Got back to Breakout game. Fixed data structure (repeat "again and"), ran into a weird bug - runtime exception when having an anonymous function at (setup) to set up an atom of grid. However, I also made a quite hacky fix, when trying to understand the problem: it started working when I added (println) for the named function. It's quite a mystery for me - going to ask fellow Clojurians about this and do some research. 

**Thoughts** I'm half dead today - like, deadly tired. I had quite the same bug two days ago in (setup) and though that it's because of badly constructed data. Well, data was indeed badly constructed, but today bug persisted too, even after fix. Really curious about this issue and would be glad to understand it. Stack trace showed TypeError and undefined value - that's also strange. Even more strange was to find out that it works with added (println) - I'd assume that it's something with asynchronous functions as I had something quite similar before in JavaScript - but it just doesn't feel like it's the case here. 

**Link(s) to work**
[22507ab](https://github.com/Gaivile/breakout/commit/22507abf2a4a9b57506df7588474d365b16b047d)
[abe0e30](https://github.com/Gaivile/breakout/commit/abe0e30d7bd71c63365ba8c489b3299ca0a73e27)


### Day 9: January 11, Wednesday

**Today's Progress**: What a nice and productive day - I'm getting so close! Today, as always, I improved data structure on grid atom. Then, using the new structure, changed draw funtion to represent all the bricks. Started working on collision function and, surprisingly, finished it so now if a ball touches a brick, the brick disappears (is removed from the grid and not drawn anymore). It's not perfect yet - the game slows down on collision, so need to improve that.

**Thoughts** Having a clear plan and knowing what exactly needs to be done really helps. So, I think I'll be writing some notes here too (maybe not always... Will see). Stuff that needs to be done: 1) improve collision function so it's faster; 2) implement (bounce) function so the ball bounces off the bricks on collision; 3) work on some math for the movement of the ball itself; 4) work on some colours.

**Link(s) to work**
[68449a5](https://github.com/Gaivile/breakout/commit/68449a5ce3b320b7f712c34142392c306b573e05)
[a1614b8](https://github.com/Gaivile/breakout/commit/a1614b8dae41175b80eb09eb2fcab6c3f6af0da6)


### Day 10: January 12, Thursday

**Today's Progress**: Today I reassured that collision function works properly and made a ball bounce off some of the bricks. It still doesn't work as it should, as I'm getting null pointer exception in draw function (another mystary/magic thingie...) - have to debug that and work a bit on the math for bouncing. 

**Thoughts** Oh god, I thought it's already Friday... Wasn't as productive today, not sure if I can be productive tomorrow too. Need more sleep, I guess..?

**Link(s) to work**
[4b6c019](https://github.com/Gaivile/breakout/commit/4b6c01939ecdbc44700e9371a64739a1f886460f)


### Day 11: January 14, Saturday

**Today's Progress**: Eeks! I've missed a day yesterday :( So, getting back on track today - already past 12, so done a late commit, but it's totally worth it as I have a working version of the game! So excited! Null pointer exception was because I forgot to put (do) function in (if) statement when I had more than one function there. I also changed the math for ball direction which solved another issue with not every brick being removed and some bouncing troubles. 

**Thoughts** So, I just realized that I missed Friday the 13th - guess it's for the better as I was quite tired after writing insane SQL queries at work. I literally was dreaming databases the night after. However, today I was able to do my own things with fresh mind and well-rested which lead to improving the game as much as it's working and really play-able. There are still a couple of things left to do: 1) Fix an issue with a ball being able to go up when it's missed by the player to save - it shouldn't go back up (easy fix); 2) do something about the colours - maybe change each line to a rancom colour when collision occurs; 3) maybe add you won/you lost thing? 

**Link(s) to work**
[056b728](https://github.com/Gaivile/breakout/commit/056b728eca687e68681f857bdbe316c72c38bd6f)


### Day 12: January 15, Sunday

**Today's Progress**: Continuing on improving the game =^_^= Fixed a small issue with the bottom so that the game is lost if a player didn't catch the ball with a paddle. Also changed colour theme - the row of bricks get randomly generated colour on each collision. 

**Thoughts** The more I work on this game, the more I enjoy the process! I think I'm kinda done with the major part - data structure for pixels around each brick (quite unbelievable though). However, now I've got an idea of won/lost part of the game. I think I'll <i>really</i> be working on this, just because. Need some ideas for what to put there, but I'll come up with something.

**Link(s) to work**
[9ab0cf9](https://github.com/Gaivile/breakout/commit/9ab0cf9ec19908d7fad7486fb98be0739edcb316)
[44c531c](https://github.com/Gaivile/breakout/commit/44c531cfcae27940a8e935bfbafa1a74f5b6e02b)


### Day 13: January 16, Monday

**Today's Progress**: Today I added win, lose and play again features to the game. Nothing much to explain - if a game is lost, "you lost" appears and if it's won - "you won", also a mouse click restarts the game after winning/losing. Quil is pretty coll library for these kind of functions. It was hard to work with collision detection, but it also was a good experience. Other things were just really cool and fun, and enjoyable =^_^=

**Thoughts** I guess, this game is pretty much done. I might add some additional featueres in the future or make it look somehow different, but for now I'm happy with the result. What I've learned so far is that the most important thing in Clojure is data. It's stressed in every Clojure-related blogpost or tweet or anywhere - but that's simply because it's true. Once you've got the right structure, using Clojure for data processing is incredibly pleasant. Started to think about the next project. Hmm... Maybe another game?

**Link(s) to work**
[9f51670](https://github.com/Gaivile/breakout/commit/9f51670f790359bbca8c28a8ad1e39e803306d58)


### Day 14: January 17, Tuesday

**Today's Progress**: A bit hard to measure the progress as I've finally found some courage to change the editor - learning Emacs! I know that it's not concidered as "personal coding project" per say, but it's quite big for me. I'm feeling like a 5 y/o for the first time at the computer, using MS Paint :D But I kinda like Emacs. I was convinced how powerful it is, so it seems like nice journey of learning.

**Thoughts** I think I'll do something small and simple this time - just to get more familiar with Emacs. Maybe some tiny exercise with a single namespace, then next time something slightly bigger... I don't know yet. I was told about a steep learning curve with Emacs, but I don't want it to be too steep anyway.  

**Link(s) to work**
[Attended this workshop](https://www.meetup.com/London-Clojurians/events/230231615/)


### Day 15: January 18, Wednesday

**Today's Progress**: Introduced myself to a new project (a website for a friend) with Php (brrr...). So much for today's progress...

**Thoughts** Quite a hard day - I think I've fallen ill, so left from work earlier :/ Was feeling like death. Then my friend asked to check her website and make some changes. I just though to myself <i>Oh, what could possibly go wrond so I couldn't fix it?...</i> - and opened the source code. Oh how wrong I was! To make things worse, I've found some pretty much horribly written Php code, using Joomla! templates. Like, yeah... The nightmare upon a nightmare. Basically, an unmaintainable clusterf*ck. 

**Link(s) to work**
It's a TRAP!!!!!


### Day 16: January 19, Thursday

**Today's Progress**: Was trying to maintain unmaintainable, got frustrated, decided to start a new (proper) project.

**Thoughts** I was told to try not to do any programming today - well, I failed that. Still feeling quite miserable and staying home without any energy is really not nice. I think I'll still help a friend with her website when I feel better, but I also want to do some personal project for the sake of this challenge and because I want to learn using Emacs for Clojure, and also because I couldn't find any time. I'll be making a Game of Fifteen - a puzzle game where a player has to rearrange squares in the right order. Well, picture will help:

![15-puzzle-loyd svg](https://cloud.githubusercontent.com/assets/11088666/22128899/e29ad1b8-de9a-11e6-8174-408ba7e654a3.png)

I'll make it in ClojureScript using Reagent and Re-frame, it's going to be interesting. 


**Link(s) to work**
[The repo of the (soon to be) game](https://github.com/Gaivile/game-of-fifteen)


### Day 17: January 20, Friday

**Today's Progress**: Opened an already finished Breakout game in Emacs just to find that it doesn't work (and therefore - not that finished) :D The problem was that I've written functions for win/lose in the wrong order and LightTable didn't show that because it works slightly differently. Also, decided to play the game itself a little longer just to find another bug: after losing, the bricks didn't reset, but rather got one on another as duplicates, like layers, so they had to be hit multiple times to disappear. There is no such issue with winning as all the bricks are removed by the player, but I still decided to fix the issue with losing in (play-again), and it looks like a good decision. 

**Thoughts** Was nice to go to work after being off yesterday. Feeling better today. Also, it's a real struggle to learn Emacs, possibly because for me personally it's always a bit more iteresting to actually work on some project than learn to use a new tool. Well, I've got a feeling, when I get a bit better with Emacs, I'll really enjoy the process of learning and expanding the knowledge, but I'm not there yet.

**Link(s) to work**
[248b8d8](https://github.com/Gaivile/breakout/commit/248b8d8642bb7bbf6384198e67713e083e06abae)


### Day 18: January 21, Saturday

**Today's Progress**: Hack the Tower event and some ClojureScript along with Reagent making Kanban kind of board for to-do lists. It's by [Lambda Island](https://lambdaisland.com/episodes/reagent) videos and learning material, they're so useful and easy to follow. Also, I somehow managed to break my Spacemacs, but during the event, I got help to fix it, so was able to get used to Spacemacs a bit more.

**Thoughts** I barely made it this Saturday - I've got even more ill :( 

**Link(s) to work**
[260de6f](https://github.com/Gaivile/kanban-lambda-island/commit/260de6fc5821a87dbf80dcec51019348ecb03e30)


### Day 19: January 23, Monday

**Today's Progress**: Continuing on [Lambda Island](https://lambdaisland.com/episodes/reagent-2-cursors) and Kanban project. I'm really glad we started this on Hack the Tower on Saturday as I probably wouldn't be doing any project at all right now because my brain is melting. Learning a lot with ease - I think the understanding of how Reagent works will give me a stronger foundation for later work witg Re-Frame when building the next game.

**Thoughts** Being ill sucks. I skipped the day yesterday as I could hardly get out of the bed. I think I had fever. Today again, I really struggled to do anything at work, colleagues even suggested me to go home, but I <b>really</b> wanted to have my stuff finished and I knew that at home I just couldn't. So taking it easy today, going slowly through a tutorial and learning the sorcery of Reagent.

**Link(s) to work**
[3a2747d](https://github.com/Gaivile/kanban-lambda-island/commit/3a2747d21522f32ab782fe197c21ec9e85afe2f4)

