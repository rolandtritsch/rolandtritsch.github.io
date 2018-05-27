---
layout: post
title: The cost of building a skateboard ... and a lot of PSs
---
The other day I was explaining again how to build an MVP and I was using the [skateboard picture](https://blog.crisp.se/2016/01/25/henrikkniberg/making-sense-of-mvp) (again :)).

![Skateboard](https://blog.crisp.se/wp-content/uploads/2016/01/mvp.png)

In the middle of the discussion I realized that we only had half of the discussion, because we only talked about the direct benefits of the approach: Fast feedback, less risk to build the wrong thing, ...

We did not really talk about the *cost* of getting these benefits. The meeting got interesting when I started to point out that this is not about building the solution the fastest way or the cheapest way. When you look at the picture you can actually see that it will be very expensive to build the car this way, because on the way to the car you build a fully functional skateboard, a bicycle and a motorbike (before you *start* to build a/the car). And even worse the overlap between these incarnations of your solution is probably minimal, means you probably have to (and want to) (more or less) start from scratch (maybe even using a new programming language and a new architecture/design (monolith to microservices ... [anybody](https://martinfowler.com/bliki/MonolithFirst.html) :))).

The cost of this (in terms of time and money/people) is obvious and significant.

Compare this to the cost of building the car right away. You are always working on the car. No waste in time and money. You are building one thing and you are building it once.

Why can't we just do it that way (besides that it takes 12-24 month before the users see something)?

The main reason is (as we all know) that you do not know. You actually do not know what you are building and we do not *really* know what the customer wants and/or needs and/or values (until after we get feedback on the motorbike). Means at the end there is a 90% chance that we are building the wrong thing (it is unuseable; it is not solving the problem that the customer/user has) and we are building it wrong (the system is hard to maintain and hard to change). And building the wrong thing is obviously the most expensive outcome to produce/deliver (and let's not assume that you will be able to build something that is *80% right/valuable*, because in reality (in the best case) (with the car-first approach) you will probably build something that is *20% right/valuable* (and *that* thing (believe me!!!) will never get used!!!).

**Main take-away**: Building systems with a/the skateboard approach is dramatically reducing the risk that you will build the wrong thing, but it is also slow and expensive (compared to the naive/mythical "let's build a car right away" approach) and I think it is important to get everybody on board with that reality (e.g when we are done with the skateboard, we have to throw it away and start from scratch again) and then ... build the skateboard.

**PS**: I think the myth/urge to build it once (and get it right) exists on multiple levels: In the large (systems, architectures, MVPs, ...) and in the [small](http://www.tritsch.org/2017/06/06/getting-it-right.html) (designs, code, tools/frameworks/technologies, ...).

**PPS**: Very early in my career I was spoiled (and probably ruined for life). For 2 years I worked on a massive project/product to replace an existing bill-of-material system (in the automotive industry) with a new one (C++, HP-UX, Ingres; absolute state-of-art at the time (1990); my thesis is on doing (recursive) parts-decompositions with a relational database in a single SQL statement and all the query optimizations that you need to do to make that work (you might want to think about that for a while)). And for 2 years we build the car ... and it worked. It took me a while to realize that this was one of the 10% cases. Mainly because the guy who was running it was a genius (Product Manager, Project Manager, Chief Architect, People Manager **and** Business Domain Expert ... in one person (total [unicorn](https://www.linkedin.com/in/hermannsauer)))) and he had build the previous system (for 5 years) and the customer trusted him (even when we showed them the first wheel with nothing else)). It was an amazing experience. For a while, I thought that all projects should be like this ... and will be like this. And then ... I woke up.

**PPPS**: But then ... on the other hand ... maybe he had build the skateboard, the bicyle and the motorbike before I joined the project back then.

**PPPPS**: There is a question to ask here about macro-MVPs and micro-MVPs. A macro-MVP can be structured like this ...

* build the skateboard (3 month)
* rebuild the skateboard ... better (e.g. more maintainable; build the frame of the bicycle) (2 month)
* build the bicycle (4 month)
* rebuild the bicycle ... better (build the frame of the motorbike) (3 month)
* build the motorbike (6 month)
* rebuild the motorbike ... better (build the frame of the car) (6 month)
* build the car (12 month)

... for a total of 36 month/3 years (Note: As part of that journey you will also build up the team to maintain the car long-term and to build the plane that comes after the car and that means more and more people will work on it and that means the cost of this is probably more in the region of 100 person/month (not 36 person/month :))).

Now ... depending on your situation (e.g. seniority/experience of people, amount of business domain expertise, ...) you probably want to implement some of these "phases" as/with a micro-MVP approach (which will slow down the development even further (while reducing risk)).

Remember ... with a/the MVP approach you are compensating for a *lack* of business domain expertise/a lack of understanding what the *real* problem is and what the customers/users *really* want and need (and with that comes the risk of building the wrong thing; and not only now, but building the wrong thing for what the customer wants/needs in 2 years from now). If you have that *insight*, then nothing prevents you from moving faster. **Otherwise ... slower *is* faster!**

**PPPPPS**: BTW ... as you have figured out by now, all of this is about learning and building up business domain expertise. One way this can go very wrong is, if you do not plan for attrition, means you need to realize that over the course of the solution development life-cycle (from skateboard to car) you will loose people. You probably want to minimize the turn-over, but it will never be 0 (and probably should not be 0). Retaining the people you have invested in is key. Loosing more than 30% of the know-how between the incarnations can kill the entire MVP approach. Clarification: 80% of the know-how will probably be with 20% of the people in the project. It is the turn-over on that group that you need to be worried about.
