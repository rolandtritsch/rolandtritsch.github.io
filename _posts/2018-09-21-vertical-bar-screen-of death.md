---
layout: post
title: The vertical bar screen of death ... the story of an unexpected win-win
---
Last year I spend some time and money to "renovate" my old 17-inch Macbook Pro (remember the good old times ... when Apple was building good laptops with great keyboards and no touchbar :)).

For the last 6 month I was running [VirtualBox](https://www.virtualbox.org) on it hosting an Ubuntu image.

That kind of worked (a little bit slow at times and managing the ports was (sometimes) challenging, but otherwise ... ok).

But ... running Ubuntu through VirtualBox on MacOS, puts a lot of stress on the graphics sub system and ...

... 4 weeks ago the Discrete GPU collapsed and I was stuck with the **[Vertical Bar Screen of Death](https://discussions.apple.com/thread/6509358)**.

![VBSOD](https://forums.macrumors.com/attachments/img_1051-jpg.671258)

While I was researching what the hell is going on (and how to fix it (besides spending $$$ on a new main/mother board)) I stumbled over a [blog post](https://ubuntuforums.org/showthread.php?t=2157775) that explained how to install Ubuntu and disable the DGPU while booting and "just" use the Intel GPU/CPU for the graphics (which is fine as long as you do not play games (which I don't)).

Getting this done requires some careful typing (because while you boot and while you are using grub and while you are editing the boot parameters ... the sreen is still not working and kind of hard to read), but ...

... the result is **AWESOME**. Win-Win. I was able to get my laptop working again (without spending a lot of money on a new main/mother board) AND I am now running Ubuntu on the bare metal. Works like a charm.

![awesome](/images/2018-09-21-vertical-bar-screen-of-death/awesome.png)

Now I am in a position to channel the inner nerd in me again :) ...

* Writing [Scala](https://github.com/rolandtritsch/scala-aoc-2017) and [Haskell](https://github.com/rolandtritsch/haskell-aoc-2017) code
* Using [emacs](https://www.gnu.org/software/emacs) (with [ensime](http://ensime.github.io) and [intero](https://commercialhaskell.github.io/intero))
* On [Ubuntu](https://www.ubuntu.com/download/desktop) (running the [Awesome](https://awesomewm.org) WM)
* With a 17-inch Macbook Pro (early 2011)

Beat that :).
