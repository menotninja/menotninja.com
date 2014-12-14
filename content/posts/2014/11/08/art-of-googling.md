Title: The Art of Googling: Hunting Down Solutions in Record Time
Date: 2014-11-08
Category: Programming
Tags: beginners
Slug: the-art-of-googling
Summary: Tips and strategies for using Google when programming.

**Few beginners know how to use Google effectively.**

Everyone knows that one should use Google; yet few beginners know how to use
Google effectively. Even fewer mentors recognize this as an important skill
that needs to be taught explicitly.

When you point your browser at google.com, you find a blank search box staring
back at you. What magical keywords should you type in there to help you solve
the problem you are tackling?

### First, imagine what you want to see in the search results.

If you are trying to debug an exception/error/unexpected behavior, odds are
someone else encountered the same problem. The first goal is to find a similar
question on StackOverflow, a thread on a mailing list etc. A subsequent goal
might be to learn more about a specific cause by looking up documentation for
some API or function.

Keeping these goals in mind, imagine what keywords are most likely to appear on
these pages.

### Cut down the search space.

Your search terms should be sufficient to uniquely describe the issue you are
tackling. Include names of languages, frameworks, libraries etc. In some
situations, it might be necessary to include version numbers as well; this is
more important in languages like Scala (2.9 ~ 2.11), Python (2.7 vs 3), and
Java (6 ~ 8).

Add and remove keywords until you get a satisfactory list of results, and use
what you learn to fine tune your search. It frequently takes me 3~4 tries to
get what I want.

### Selectively copy errors.

Copying the entire stack trace will not be useful - it will contain too many
details that are specific to your work. On the other extreme, searching for
“it doesn’t work” will not help you either. Find the sweet spot in the
middle, including just enough pertinent information to identify key aspects of
the error.

This is an art. In Java, I usually copy just the exception class and the
accompanying exception message.

We all cross a hump at some point. Eventually, you will become so familiar with
the space of problems that you know, instinctively, what to look for.

*Thoughts, comments, criticism? Fire away.*
