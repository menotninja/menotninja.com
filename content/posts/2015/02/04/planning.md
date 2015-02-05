Title: The Joy of Planning
Date: 2015-02-04
Category: Programming
Tags: beginners, mentoring
Slug: the-joy-of-planning

### Fighting the Kraken

A long long time ago, the assignments and tasks I worked on were incredibly
simple. I could bang out a half-assed solution with my eyes closed, submit it
with minimal tests, and still get a decent score. Of course this inflated my
confidence, and I never bothered learning how to plan. Yeah, I was that
arrogant guy in your CS class.

"Ah! Looks trivial. Just give me a day and I will figure it out."

Heh. What an idiot I was.

If you have worked on any significant project, you know that this attitude
wouldn’t serve me well. I was young and naïve; as projects got harder, I
thought that I could increase productivity by using some shiny framework, some
fancy automation tool, a particular brand of mechanical keyboards, or even a
_different keyboard layout_. Of course that didnt work. What was I thinking?

A few years after I started learning how to code, I worked on a distributed
system with a partner (let’s call him Ted.) We were both hot blooded and
wanted to jump straight to the code and bang it out as fast as we could,
because we thought we were "ninjas". LOL. We had a great time, and were
consistently coming up with new ideas every day and wanted to add "cool"
features to our project.

"Oh! Wouldn’t it be cool if it did this?"

We worked feverishly, and kept adding more and more features to the project.
"Because we can! Haha!" The codebase grew uncontrollably, and work became
harder and harder to coordinate. It grew rapidly out of control, and complexity
skyrocketed. It was a mess. It was the worst spaghetti code, ever. On top of
that, the large number of features we had to support made it difficult to use
and very tricky to debug.

Eventually, it became to much for us to handle. We spent several weeks
obsessively refactoring the code and organized various pieces into separate
components. We barely made the deadline, and fell short of our expectations.

It sucked, but it was a good lesson for us.

### Drawing a Map, Writing the Story

![planning]({filename}/images/sf-bay.jpg)

I didn’t glean the lesson entirely until a few years later; I realized that
the root cause was our lack of discipline to plan ahead.

When you start working on a large project, it can often be exciting and
overwhelming at the same time. Where do I start? What features should I build?
Occasionally, you might be tempted to jump straight in and soak it up (which
was what we did.) Instead, break it down into smaller pieces. Whittle away at
the problem until it becomes tractable.

Ha! I can already hear some of you yelling: "I am AGILE! Who needs a plan?
*rolls eyes*" Sorry to have to burst your bubble, but it is a myth that agile
software development and planning are [mutually exclusive ideas][dilbert].
Agile doesn’t mean “no plan required” - it means that you plan to collect
feedback at the end of each iteration to update the plan.

> Practical design does not anticipate what will happen to your application; it
> merely accepts that something will and that, in the present, you cannot know
> what. - Sandi Metz, _Practical Object-Oriented Design In Ruby: An Agile
> Primer_

Start with a short plan. It doesn’t have to be very involved, but it should
give you a map showing you where to go, and how to get started.

1. Describe the purpose of the project. If possible, identify existing
   solutions and abstractions (e.g. It’  a "distributed cache" or "REST
   server").
1. Make a list of desired features, organizing them into 'must have', and 'nice
   to have'. Decide what you are definitely _not_ building.
1. Figure out the components and their interfaces. Create a story - what
   features belong together naturally?
1. Identify important libraries and dependencies. Say, you need JSON parsers: pick one.
1. (Advanced) Make a list of assumptions. For example, you might assume that
   the your processes have complete ownership of the disk (or other devices) in
   other to make some optimizations.
1. (Advanced) Pick design patterns (link to GOF) you intend to use. Decide if
   you wish to use a dependency injection framework.

Here’s the kicker: this plan is not final. In fact, it’s likely to change as
the project grows, but it makes every change visible and forces you to think
about that change.

Creating a short plan (like the one above) makes it easier to

- split up the work,
- identify difficult components that require more research, and
- design the components so that they are easy to test/change.

Now get out there and code your ass off.

  [dilbert]: http://dilbert.com/strip/2007-11-26
