---
layout: post
title: Make Google Chrome show the Wifi login screen (best trick ever :))
---
Not sure if this has ever happen to you, ...

... but once a month I am sitting in a hotel lobby or a coffee shop and I cannot (for the life of it) make Chrome show me the login screen to the Wifi portal and then you start to fiddle around with stop/start the Wifi and/or disconnect/connect to the Wifi and/or start a different browser (e.g. Firefox or Safari) and/or try a private browser window and/or clear the DNS cache and/or ... reboot!!!

By now I run Ubuntu on my Macbook Pro and figured that there must be a way to fix this and guess what: There is :).

First of all it always helps to (really) understand what the problem is. And in our case the problem is "just" that most Wifi portals cannot deal with https requests before you have gone through the login page. Note: Going to http://www.google.com (and/or other "big" sites like twitter, facebook, amazon, ...) does not help, because that gets rerouted to https://www.google.com.

Means the easy solution is to force the browser to go to a guranteed unsecure website/url.

I am using http://www.tritsch.org.

Have bookmarked it. And whenever the login page is not showing up I am "just" clicking on the bookmark ... and voila ... problem solved!
