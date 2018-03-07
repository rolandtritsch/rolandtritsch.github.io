---
layout: post
title: Assembling a Gatling (gun) ... how hard can it be?
---
Back to the roots!!!

I am writing [Gatling](https://gatling.io/) tests (again :)). (Obviously) I used to do this (a lot :)), when I was with [Gilt](https://www.gilt.com) (for an obvious [reason](https://flic.kr/p/aSfJyx) :)).

To get going again, I had to make the basics work ... again.

The basics are: Make the [sbt-gatling](https://github.com/gatling/gatling-sbt) plugin work to build (end-to-end integration) tests/simulations and then create a "deployable" (fat) jar (using [sbt-assembly](https://github.com/sbt/sbt-assembly)).

This proved to be more difficult than I thought (because this used to work).

Everytime I was starting the jar with `java -jar load-test.jar -s computerdatabase.BasicItSimulation` I got the (in)famous `There is no simulation script. Please check that your scripts are in user-files/simulations` error message.

After some heavy debugging, I realized that the settings in `gatling.conf` override the command-line parameters (and in my case I had copied the gatling-default.conf into the resource directory and in that file `simulationClass` is set to `""`).

[Fixed it](https://github.com/rolandtritsch/gatling-load-testing). Working now. Something to be aware off.