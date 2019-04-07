---
layout: post
title: I love Haskell
---
Over the last 2 years I did a fair bit of Haskell (after doing a fairer bit of Scala for 8 years).

And I love Haskell.

Don't get me wrong: If you are tied to the JVM eco-system (and who is not these days), my opinion is that Scala is your best option to do functional programming in the JVM.

At the same time writting code in Haskell feels very natural to me. And sometimes it is not the big features/capabilities that make a difference. For instance in my case (in Haskell) I like ...

* ... the **where-clause**. There are obviously two way how you can compose/decompose a problem. Either you start with the pieces and then compose a/the solution from it or you start with what you want/need and decompose it into smaller and smaller pieces until you are done. The second approach feels more natural to me. Haskell supports both (with let-in and the where-clause), but most of my code starts with a function that is a single line and a where that explains how that line can be evaluated.

* ... the ability to have **primes**. As I said it is the simple stuff. One small thing that I love about Haskell is to be able to name variables as/with `name` and `name'` and `name''` and ... (not too much so; I normally stop at 2 primes), because it allows me to stay in the flow and do not think (too much about naming variables; not saying that finding good anmes for variables is not important :)).

* ... the **go** convention. I love recursions (and folds :)). The convention to have a function that pattern matches on the "start-the-recursion", "do-the-recursion" and "stop-the-recursion" (using a function in the where-clause that is called go) breaks down the problem into three very manageable sub-problems.

As I said ... these *features* (if you want to call them that) are not big, but sometimes the small things make a difference.
