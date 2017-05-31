---
layout: post
title: The myth of ... getting it right the first time
---
I am reading it again: [Clean Code](https://www.amazon.com/Clean-Code-Handbook-Software-Craftsmanship/dp/0132350882).

This time I am reading it differently. The first time around (6 years ago), I was reading it and learned a lot (about how to write clean code) and was using it (a lot) to get other people on board and convinced that this is **the way** (the only way) to write code.

I still think that the book can serve that purpose.

But reading some of the recommendations again also got me worried, because I feel that sometimes and to some extend we are still fighting the same battles than 6 years ago (or maybe 20 years ago).

And the battles are the battles of expectations: The expectation that managers and engineers need and want to get it right the first time around.

So lets articulate a different expectation. And that expectation is based on experience. And my experience is that you have to write code three times. The initial version will allow you to understand and explore the problem space (e.g. understand all functional and non-fucntional requirements) and the solution space (e.g. start to learn the frameworks that you want to/need to use). You will (hopefully) produce a/the Minial Viable Product (MVP). [In general that code will be **bad**](https://arstechnica.com/information-technology/2014/11/how-to-manage-accidental-complexity-in-software-projects/).

After you understand more/better what the problem is and how to solve it and how the frameworks work, you need to rewrite/refactor your implementation. Note: During that refactoring no new functionality or net new features will be added. But your code will probably/hopefully shrink in size and complexity and will become much more readable (e.g. because you now know how to name things right). That code will be **good**.

Very soon afterwards it will be the first time that you have to change the code, because some of the requirements have changed and you realize that the code is hard to change. At that point you will start to understand, which parts of the implementation will be stable and will probably not change a lot and which parts are based on requirements that are less stable. That will allow you to introduce abstractions and indirections where they are needed and valuable. And then the code will be **clean**. And then the journey to keep it clean starts.

Now let me put a stake into the ground and let me say that it is going to take you 33% of the overall time/money to build bad code, another 33% to build good code and another 33% to build clean code.

And that is just the cost of building that code. If you want to own (and change and extend) that code for a period of time (let's say 3 years) you also need to keep it clean (Remember: There is a difference between [the cost of building something and the cost of owning something](https://www.intercom.com/books/product-management), let alone the cost of owning bad code).

And it is not hard to see, where it all can go wrong. After the first 33% you have something that works (100% functionality at 33% of the cost) and it will either take a very strong manager or a very strong engineer to spend the remaining 66% of the time/money to get to clean code (without a visible/significant increase in functionality). We all want to do the right thing (go to market as fast as possible with the smallest cost possible). We all want to be good. Good managers and good engineers. And iterating on something that works feels bad or not right. It feels like you have done something wrong the first time around. You might even feel guilty or not smart enough to not get it right the first time around.

Don't. Don't feel that way. It is totally normal to iterate on code that works. And the only bad thing that you can do is to have the expectation that you will be able to get it right the first time around. And the only thing that makes you a bad manager/engineer is not spending (and/or asking/fightig for) the 66% to make the code clean (after you have validated the MVP).

Last but not least, there is another big problem with this expectation or ambition to get it right the first time: It will slow you down. With that expectation, it might take you a lot longer than 33% to get the (MVP) functionality up and running (partially because the code will contain lots of premature optimizations) and you do not even know, if what you are building got the product-market-fit you are looking for.

Writing clean code it expensive. But premature optimisations and/or maintaining bad (not clean) code can [kill your company](https://www.forbes.com/forbes/welcome/?toURL=https://www.forbes.com/sites/falonfatemi/2016/05/30/technical-debt-the-silent-company-killer).

So let's feel good about writing code three times. Let's feel good about not getting it right the first time around.

And yes ... I know: I am breaching to the choir, but ... better safe, than sorry.
