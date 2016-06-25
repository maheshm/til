# Click on a tag fires 2 click events in Firefox

I saw this happen in version 41 of Firefox, but I am sure this has been an age old issue. The events are getting triggered from multiple levels in Firefox. I had faced 2 instances of the same (but for 2 different reasons).

Recent one was because there was a `method` that was defined for `link_to`. This generated a `data-method` is added to the generated `a` tag. This was resulting in two clicks to be fired from the same a tag.

If this is a `get` request you are lucky, just remove it. I am not sure what to do if it is any other verb.
