# Developer Handbook

This document outlines 5app's developer best practices - at the risk of appearing dogmatic.

It is [like us] a work in progress and open to suggestion and adaptation.


## Fundamentals

It's important that we openly discuss and share the work we have done, so that we learn off oneanother, share problems and solutions. Possibly all of the best practices revolve around good communication


## Code less

Coding should *not* take up the majority of your time. And the good news is there's lots to do besides.

1. Inspect tickets: Have a look at the tickets which are new or are being worked on, if it's a bug try to replicate it and let everybody know #metoo. Add your comments, emoji or even just beautify the markdown if it's not already.
2. Review Pull Requests: Perhaps before you take on another ticket, checkout open Pull Requests and see if you understand what's going on, it not ask. If you do, and your happy, give it your stamp of approval.
3. Read More: Try out new things and make suggestions to the team.


## Branching Model: Git Flow

Follow the [Git-Flow branching model](https://nvie.com/posts/a-successful-git-branching-model/)

- Master is always production deployable
- Staging is the next release, and made available for regression tests
- Dev is the culmination of a sprint
- Feature branches are based off dev

This flow might not make sense for all projects which dont have a manual QA function.


## Creating Feature Branches

1. Use semver in the title e.g. `feat(sharing): allow for users"
 - this helps us generate the changelog
2. Include the `fixes #1337` in the body so that tickets can be automatically closed.
3. A concise and clear descriptions along with any concerns you have over your changes will help in the review stage.
4. Keep PR's size to a minimum to ensure that it's easy for other members to digest.
5. Dont refactor (at least try not to): KISS (keep it simple stupid), those changes add complexity and attract bugs.
    - Create another PR if you want to refactor something.
6. Request PR reviews from people on the team (Github recommends people which is a great place to start)
7. Once approved please [Squash Merge](https://help.github.com/en/github/collaborating-with-issues-and-pull-requests/about-pull-request-merges#squash-and-merge-your-pull-request-commits) this will again make it easier to read the changelogs.

## Working on Epic's

1. Epics can be big, and so should be broken down. This means many people on the team can be working on the epic at the same time. As well as making the task less daunting.

2. When an epic is to be tested, it maybe required to create a temporary branch to test all the features of the epic in one place. This will allow the stakeholder to provide feedback, as well as QA testers the ability to test the feature in a relatively stable environment.

## Commit Messages

Commit messages provide a valuable summary of the code changes made. A good commit message will look like:

> fix(homepage): change api request, #1337

- **semantic commit message**: starts with fix, feat, test, style, docs, refactor
- **issue number**: appears at the end of the message and provides a way to track the change
- **message**: is short and concise
