---
name: Coding in the Wild
nav_order: 4
parent: Workplace Basics
---

# Coding in the Wild

This post will go through a typical development workflow, or software development life cycle. Your experience will vary depending on what framework your organization uses to deliver software, but there are some basic concepts that are universal throughout.

The components of software development life cycle:

1. Requirements Gathering
2. Planning
3. Implementation
4. Delivery
5. Support

## 1. Requirements Gathering

The first thing you'll need to do is to determine what you need to build. This comes in the form of requirements. Requirements are the specification for what you need to build. If an engineer was told to build a bridge across a river - some requirements might be the length of the river, the max weight across the bridge, the usage of the bridge, etc.

There are two trains of thoughts when it comes to requirements - everything up from (waterfall) or find out as we go (agile). Agile has become the more popular methodology because with modern software we've found that it is impossible to know everything upfront, and it is more important to get working software out and change it later.

There are two types of requirements: Functional (FR) and Non-Functional (NFR).

### Functional Requirements

Functional requirements are those that define the behavior and look/feel of the feature.

For example if you were building a shopping cart, you would need to define how the items are organized, what functionalities you can do to the items, what content of the items to display for each item, etc. 

These are business cases that are usually composed of:
* Actors - The users interacting with the system
* System - What is the intended behavior of the product
* Goals - The purpose of the interaction

[More about functional requirements](https://www.altexsoft.com/blog/business/functional-and-non-functional-requirements-specification-and-types/)

### Non-Functional Requirements

Non-Functional requirements are those that define the technical specifications of the feature.

For example if you were building a payment processing system, you would need to define security and expected throughput.

Non-Functional requirements are ones that you usually need to figure out earlier in the process because there are none negotiables that are fundamental to the feature.

More examples:

* Performance and Scalability
* Portability and Compatibility
* Reliability, Availability, Maintainability
* Security
* Localization
* Usability

[More about non-functional requirements](https://www.altexsoft.com/blog/non-functional-requirements/)

## 2. Planning

Again actual planning mechanisms will differ, but each approach has some sort of system of defining how much you can work on for a given amount of time.

If you are a a team of one, planning may not be all that important because you can just work on whatever you need to right then. But unfortunately that is usually not the case as you will be working on a team with many people and there are dependencies and different expectations for your work. Because we need to collaborate we need to determine what we can realistically complete and work that we cannot. I want to put emphasis on the "cannot" because that it is all too common that we developers overestimate our ability to complete things in a given amount of time which in turn results in missed deadlines which causes problems for both technical tasks and business expectations. More importantly this can places a big toll on you as a developer where you will find yourself overworked and burnt out. A key skill you will develop as a developer is to manage your expectations of yourself and to deliver on-time and on-expectation - that is a true sign of a mature developer.

## 3. Implementation

Get it done!

But really the implementation phase is where the bulk of your work will be. There are two main components to this: Development and Testing. Development may get all of the glory, but both are important.

The goal of development is to deliver something that works, remember working software is king. How does one approach the development component of this?

The first thing you will need to do is make sure you fully understand the given requirements to a __T__. If you don't you may very well be building the wrong thing!

The second part is to get working code. This will depend on how you like approaching a problem, but a general rule of thumb is to not worry about style too much in the first pass. When you have something working you can always go back and refactor the code to your liking. You should do some local testing to verify that your code works.

The third part is code review. You've finalized what you want to deliver and now want to make sure that you covered all your bases functionally and stylistically. Usually this is done by a more senior developer, but that doesn't always have to be the case. I'll probably circle back on this in a later post about what is a good code review.

The fourth part is integration testing. Your code has been verified and you can now deploy it to a remote environment. In most cases your place should have a "develop" environment where people push their code to test if it works on a remote environment and if it integrates well with other people's code. During this phase you can also get business verification to verify that what you built satisfies the business requirements, and also open it up to further testing from QA resources. If you need to make changes you can move back to step 2.

And that's pretty much it. There may be more environments like "stage" or "pre-production", but it's pretty much just step 4 again.

## 4. Delivery

This is the scary part for some, where we finally push our changes to production and out to the world. Each organization will have their own way of doing it, some will have some change records where you need to get sign-offs, but it usually involves getting some sort of approval and then using tooling to deploy your code out.

Once your code is out, you're going to be doing some validation. On the easy side of things you just test the feature yourself. In more complicated places you might do some canary build where you have the old and new versions of the code out and see if the new code is behaving as expected before moving all of the instances to the new code.

## 5. Support

Then we move on to the last stage of the life cycle where your code is out in the wild and you are responsible to make sure that it stays working. Your code will be tested against all kinds of inputs you wouldn't imagine, and some really funny bugs can pop up. What's not fun is when it is reported to your team some feature is not working and you have to hunt through the logs to find out what is not working.

Depending on how your team has agreed upon, you may get called out at any time of the night to hop on a call and help troubleshoot the issue. Sometimes they may say we need to fix this now if this is a major business need, or they may choose to delay it to the next day if they're nice. That's why testing a lot before hand is important because it raises your confidence that your code will stand against production when released.
