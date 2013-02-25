---
layout: post
category : features
tagline:
tags : [users, howtune, development]
---
{% include JB/setup %}

I just added in the user reputation system which allows you to like/dislike comment posts.

![New Reputation like/dislike Buttons]({{BASE_PATH}}/assets/img/reputation-comments-added.jpg)

The commenting and liking system is fairly db heavy in it's current implementation and will have to go through some optimization in the future.  I will either revert back to using Disqus or have to spend a great deal of development time tweaking the comment features.