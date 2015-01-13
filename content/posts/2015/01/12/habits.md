Title: One Habit to Start Writing Better Code
Date: 2015-01-12
Category: Programming
Tags: beginners, mentoring
Slug: habit-to-write-better-code

**Don't just "will" yourself to write better code. Cultivate keystone habits
and improve your craft.**

CS undergraduates and beginners often ask: how can I write better code? It is
hard to provide a definitive answer; after all, issuing instructions to the CPU
is a science, but writing good code is an art. Numerous books have been written
providing thousands of pages of guidelines advocating good practices. However,
how should one get started?

While it might be useful to keep a checklist of guidelines and review them
every time you program, it can get tedious real fast. Nobody wants to do that.
Instead, it can be much more productive to focus on creating habits that will
follow you throughout your career. Here is a keystone habit that will set you
on your way.

### Write Test Stubs In Parallel

As you create a new classes/modules/methods, also create test stubs in a
separate window. It's similar to TDD, but it is way easier to get started. All
you have to do is to create the test suites, and give your test cases
meaningful names, but you don’t have to fill them in. Add TODO comments in the
test cases if you like.

![test-stubs]({filename}/images/test-stubs-small.png)

It is a simple habit that does a few tricks. Since it reminds you that your
code needs to be testable, it encourages you to

- have a plan/design before you code;
- break up (or organize) your code into smaller bite-size chunks; and
- manage dependencies on the network or on external libraries.

Give it a shot.
