# Developer Handbook

This document outlines 5app's developer best practices - at the risk of appearing dogmatic.

It is [like us] a work in progress and open to suggestion and adaptation.


## Fundamentals

It's important that we openly discuss and share the work we have done, so that we learn off oneanother, share problems and solutions. Possibly all of the best practices revolve around this fundamental.


## Code less

Coding should *not* take up the majority of your time. And the good news is there's lots to do besides.

1. Inspect tickets: Have a look at the tickets which are new or are being worked on, if it's a bug try to replicate it and let everybody know #metoo. Add your comments, emoji or even just beautify the markdown if it's not already.
2. Review Pull Requests: Perhaps before you take on another ticket, checkout open Pull Requests and see if you understand what's going on, it not ask. If you do, and your happy, give it your stamp of approval.
3. Read More: Try out new things and make suggestions to the team.


## Creating PR's

1. Writing down on the ticket/PR what the changes made are doing. This helps reduce confusion
2. Keep PR's size to a minimum to ensure that it's easy for other members to read. It might be tempting to refactor parts of the code base. But that often makes the PR harder to understand and actual functionality changes can be hard to pick out.
3. Request PR reviews from people from the team (Github recommends people which is a great place to start)


## Working on Epic's

1. Epics can be big, and so should be broken down. This means many people on the team can be working on the epic at the same time. As well as making the task less daunting.

2. When an epic is to be tested, it maybe required to create a temporary branch to test all the features of the epic in one place. This will allow the stakeholder to provide feedback, as well as QA testers the ability to test the feature in a relatively stable environment.
