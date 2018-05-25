---
layout: post
title: Advent of Code 2017 ... Reloaded!!!
---
OK ... it took me a while, but ... hopefully it was worth it!!!

![Matrix Reloaded](http://4.bp.blogspot.com/-_Ytk8mebsng/TvN56L3aHoI/AAAAAAAAHjc/lPKJfTklQAA/s1600/37.jpg)

Last year at christmas I did the [Advent of Code](https://adventofcode.com) and ... really liked it!!!

If you do not know it, it is a series (25 of them) of code puzzles that need to be solved to unlock a/the christmas tree (every day (between Dec. 1st and Dec. 25th) a new/the next puzzle becomes available).

![Christmas Tree](/images/2018-05-24-aoc-reloaded/tree.png)

The puzzles do a lot of different things and will test your ability to come up with good/clever datastructures/algorithms.

What's very interesting is, that every day has a Part1 and a Part2 and Part2 will only be unlocked after you have solved Part1. As a result you get good feedback, if you have been thinking about the problem right. If yes, implementing Part2 will be easy and straightforward. If not, then you will probably need to rewrite parts (or all) of the first step. One other thing that you will find out is, if you have [mechanical empathy](https://mechanical-sympathy.blogspot.ie) (means, do you think about how much memory your datastructures consume; do you think about how many CPU cycles you are spending). If you do: Happy Days :). If not, then sometimes Part2 will explode in your face, because the problem is not different than the problem in Part1, but just 10000000 bigger (if your solution takes 10 seconds to solve Part1, it will take much longer (probably too long :)) to solve Part2).

So ... there is a lot to learn.

Means at the end I figured it makes sense to invest in a little bit of refactoring to implement **good** solutions.

And while I was at it I also invested in ...

* making it a JVM/Native cross-project
* have ScalaTest, ScalaCheck and ScalaMeter tests for every day
* add documentation about every solution

[Check it out](https://github.com/rolandtritsch/scala-aoc-2017) ... and if you like it ... star it :).
