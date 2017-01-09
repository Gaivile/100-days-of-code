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

