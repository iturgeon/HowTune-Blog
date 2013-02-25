---
layout: post
category : features
tagline:
tags : [editor, howtune, development]
---
{% include JB/setup %}

Today I finished the first version of the control bar for the article editor. Sometimes it's amazing how tedious the little things can be.

![New Article Edit Bar]({{BASE_PATH}}/assets/img/new-article-edit-bar.jpg)

It all started with the need for a Publish button on the article edit page. I added at the end of the article, sort of like a form submit button. That seemed kind of crap - because it was hard to find in some use cases, like when the user returns just to publish. Moving it to the top of the page would make it more visible, but not useful if your scrolled all the way down, like you just finished writing your article.

###Sticky menu bar to the rescue.###
The view page already had a menu bar just above the banner image, so I tweaked that, moved the buttons off to the right, and added a little area for contextual instructions (more on that later).


##The Mockups

![New Article Edit Bar]({{BASE_PATH}}/assets/img/edit-bar-versions.jpg)

The mock-ups above are in order of oldest on the bottom.  We started out with an all red bar as it matched the previous static bar we were using.

The red bar was way **too much red** (obvious now).  So, we switched colors to remove the urgency from the bar, and now we're onto something.  Now the buttons follow the language of the rest of the site and the text is more readable.  Now the biggest problem was that delete was too significant.  It's not a common task, not one we want to encourage, and certainly not a feature we want you to accidentally click on.

In the third version we found a good balance in the buttons, but something was still very wrong - The 'Saved' button didn't make any damn sense.  It was going to be used to show the saved state, but our editor intentionally doesn't have a save button.  So it had to go - and with it a re-flow of the entire bar.

Finally we ended up moving the buttons to the right, moving the extra functions into a _more..._ roll-over text link, and everything got a little cleaner.  More to come, just thought we'd share an interesting - and somewhat frustrating - path from need to solution.