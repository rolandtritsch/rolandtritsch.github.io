---
layout: post
title: Can Micro-Services Systems be simple?
---
Architecting and designing large (distributed) systems makes you think about complexity. A lot!!!

The first question that you want to ask yourself is probably "What is complexity?".

For that I recommend to watch [Rich Hickey's talk](https://www.infoq.com/presentations/Simple-Made-Easy) on complexity (Simple Made Easy). In this talk he raises awareness for the difference between something being complex or complicated. And he also (rightfully) points out that **simple is actually very hard** (every idiot can build a complicated solution) and that simple is a relative term (something that is simple for you can look complex and/or complicated to others).

I want to define simple systems as systems that have **no unnecessary complexity** and are not more complicated than they need to be.

You can Google lots of different definitions of complex vs. complicated. Most of these definitions have their roots in [Systems Thinking](). For me the difference is that systems can be complex (have a lot of components and a lot of relationships between the components). A complex system becomes complicated, if it is not homogeneous or consistent. Complex systems are hard to learn. Complicated systems are hard to change. 123456789 is complex number. 738164952 is a complicated number.

Complex | Complicated
:-:|:-:
![](http://woodka.com/wp-content/uploads/2009/01/babel.jpg) | ![](http://www.basement.org/c/images/blog/night-cycle.gif)

Designing simple systems that are not unnecessarily complex or complicated requires tradeoffs. For instance you need to decide where to put the necessary complexity: In the components (making them bigger and harder to change/maintain) or between the components (making the system harder to understand/learn/change). There is [no simple answer](http://www.tritsch.org/2010/04/22/managing-complexity-with-osgi-in-and.html).

I was reminded of this the other day. We had a discussion about adding a capability to our system and had to decide, if we want implement that capability as a library or as a service. When I started to build micro-services systems, I was always pushing for the smallest possible *thing* (abstraction) and then turn it into a services. This gives you very good seperation of concern and also allows to deploy changes without running the risk that you need to touch a larger then necessary part of the system. On the other hand ... over time ... you will end up with a lot of services and the service management and the service discovery and the service orchestration becomes a problem on its own. Means you might regret to have (too) many services. It is a trade-off and not one to take lightly.

If I am stuck, then I tend to start with a service, because it is easier to turn a service into a library than the other way around.

Not a very sophisticated approach, but so far is has worked for me.

And to answer the question (*Can Micro-Services Architectures be simple?*) ... yes, they can be and should be, but ... necessary complexity is not bad and ... stay away from building complicated systems.
