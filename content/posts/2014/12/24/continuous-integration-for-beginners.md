Title: Continuous Integration (for Beginners)
Date: 2014-12-24
Category: Programming
Tags: agile
Slug: continuous-integration-for-beginners
Summary: Continuous Integration and other Scary Buzzwords for Beginners

**Ooh that's a fancy buzzword.**

I am certain you have heard it a few times - "CI" is a hot term that gets
frequently tossed around other agile/XP concepts. It can sound intimidating,
but in practice it's fairly straightforward. This is one of the core skills
that separates professionals from the amateurs, and having a good understanding
of it will help you progress from a script kiddie to an engineer as you enter
the industry.

### What It Does, and Why We Need It

The basic intention behind continuous integration is simple: merge your changes
with your team's changes frequently and regularly. (In practice, this should
happen at least once a day.) This allows the whole team to progress in step,
staying in sync until the project is shipped.

A team that does not employ continuous integration will often encounter
problems with multiple versions of the same codebase with several weeks of work
in between them. These can take an excruciatingly long time to merge, and will
likely lead to unpredictable integration problems.

### How To Get Started

If you use git (or some other version control tool, such as mercurial),
continuous integration just means that

- changes are made on feature/patch branches;
- branches are kept up-to-date with the master branch daily; and
- branches are merged into the master branch regularly.

For example, my workflow for some Feature X could be

    :::sh
    # checkout master branch from source
    git checkout master
    git pull origin master

    # create a new branch named after Feature X from the master branch
    git checkout -b feature-x

    # work on my branch, adding unit tests where necessary
    git commit -m "..."

    # pull updates on the master branch into my branch daily
    git pull origin master

    # push my branch to the source when it's ready
    git push origin feature-x

    # merge my branch into the master branch to share my work with the team
    # using GitHub pull requests

In practice, it's tricky to ensure that things continue to work as expected
after merging. To mitigate the problem, we use static code analysis tools and
unit tests after each step to verify the "health" of the codebase. The entire
sequence of checks and tests is called a "build"; a change that causes a
check/test to fail is said to have "broken the build". An active project will
have several "builds" a day.

CI encourages frequent merges and code reviews, forces regular communication to
resolve differences in implicit assumptions.

Thoughts, comments, criticism? Fire away.

### Learn More

- A much more [detailed explanation] (from 2006) by Martin Fowler
- [travis-ci] offers free online builds for open-source projects
- [jenkins-ci] is a popular tool amongst larger teams/companies

  [detailed explanation]: http://martinfowler.com/articles/continuousIntegration.html
  [travis-ci]: https://travis-ci.org/
  [jenkins-ci]: http://jenkins-ci.org/
