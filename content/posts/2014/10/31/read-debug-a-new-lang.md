Title: How to Read/Debug a New Language Quickly
Date: 2014-10-31
Category: Programming
Tags: beginners
Slug: read-debug-a-new-lang
Summary: Tips and strategies for learning a new language quickly.

When I was starting out, I frequently felt overwhelmed by the never-ending (and
growing) list of languages and frameworks. I was constantly worrying about
whether I was (or wasn’t) spending enough time on the right languages, or
whether I was missing out on any opportunities because I didn’t know
COOL-NEW-SHINY-EVEN-DOES-YOUR-DISHES LANGUAGE X or
BEAUTIFULLY-HANDCRAFTED-BY-YOUR-GRANDMA FRAMEWORK Y. It was a constant source
of stress and contention - I was obsessed, paralyzed, and lost in FOMO-land.

I am not the only one; we have all been there. An article about the problem
recently appeared on TechCrunch, labeling the phenomenon as [Developer
Paralysis](http://techcrunch.com/2014/10/18/you-too-may-be-a-victim-of-developaralysis/).

Over the years, I realized that I am no longer worried anymore. Through months
of trial-and-error and observation, I have figured out a strategy for learning
how to read and debug code written in new languages quickly. This gave me the
much-needed confidence to take on different projects and tackle new challenges.
When it comes to picking up a new language, most folks will tell you to jump
straight in, and "use it in a project." Don’t get me wrong - this is a
perfectly reasonable tactic, and I strongly recommend it for learning your
first language. However, for your subsequent languages, this tactic also
guarantees that you will repeat the same agony and confusion every time. When I
tried it, I found myself resisting changes to my mental models, and then
quickly getting lost and being inundated by the large number of blog posts,
articles, and documentation about the shiny new language. *Diving in is fun,
but inefficient.* Most top performers I know use a more structured approach to
introduce themselves to a new language systematically.

**Day 1** Ask some basic questions:

- Is it imperative or functional? Does it have objects and classes?
- Is it interpreted or compiled?
- How do you organize code into smaller chunks? Does it have namespaces?
- How do you use libraries?
- Find the documentation for the language API and bookmark it.
- Follow the documentation to setup your environment.

Don’t try to do too much on the first day. Use your motivation to focus on
getting yourself ready, and stop at "Hello World".

**Day 2** Learn how to create a tight feedback loop. Nothing accelerates your
learning like being able to test ideas quickly and get feedback. Use it to try
out the syntax, rewrite tiny methods/functions etc.

In general, I prefer REPL over unit tests over actual program execution. If
possible, find a debugger and use it to set breakpoints and inspect variables.
Leave the advanced debugger features to later.

Note that at this point, we haven’t written much code yet, just spending time
getting ready.

**Days 3 to 7** Create tiny examples for each of the following:

- Initializing String/Lists/Arrays
- Writing Loops + Binary Search
- Using Serialization + File I/O

Use the tools you found in Days 1 and 2 to debug and build these quickly.
Tighten the feedback loop if you have to.

**Days 8 to 15** Create tiny examples for each of the following:

- Reverse String/List/Array
- Implement Your favorite OOP pattern e.g. The Strategy Pattern
- Implement Your favorite Dynamic Programming solution e.g. The Knapsack Problem

You don’t have to be an expert at every language you learn. This strategy
prepares you by deliberately acquiring the information you need to get most of
the way there.

Now go out there and code your ass off.
