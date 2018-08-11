---
layout: post
title: Advent of Code 2017 ... Revolutions!!!
---
Let's talk about the Advent of Code ... [again](http://www.tritsch.org/2018/05/24/aoc-reloaded.html)!!!

Last time we talked about a/the [Scala](https://github.com/rolandtritsch/scala-aoc-2017) implementation.

This time around I figured that I need to understand what the hype about Kotlin is all about and decided to port my Scala solutions to [Kotlin](https://github.com/rolandtritsch/kotlin-aoc-2017).

There is a separate blog post on what I think about [Kotlin](http://www.tritsch.org/2018/08/11/kotlin-the-better-java.html), but overall it was a positive experience. I like Kotlin (but would not suggest/recommend it as a replacement for Scala).

The main result of the effort to port the code to Kotlin was a [benchmark](https://github.com/rolandtritsch/scala-aoc-2017#benchmark).

![Benchmark]([https://dl.dropboxusercontent.com/s/rdehnry29tdsnrr/benchmark.png](https://docs.google.com/spreadsheets/d/1kHugZ-8mJczlmQRcda23YGvAgeqlJLt1I7cYlDD3Tws/edit?usp=sharing))

A couple of notes about the benchmark ...

* the benchmark was run on a MacBook Pro (Early 2011) with 8MB of main mem
* nothing was optimized and/or tuned (not for Scala, not for Scala-Native and not for Kotlin; these are plain vanilla out-of-the-box numbers)
* means ... this is NOT scientific!
* would suggest that you run the benchmark(s) on your platform to get your own set of numbers
* I was not able to make Day18, Day21 and Day25 work for Scala-Native. This is why there are dummy implementation for them and this is why the time is 0
* (As you can see from the color coding) Scala-Native deliveres (in most cases) the slowest results. Kotlin is (in a lot of cases) the fastest. Scala is a fast follower/second :)

Otherwise ... enjoy!!!
