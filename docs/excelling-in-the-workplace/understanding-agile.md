---
name: Understanding Agile
nav_order: 4
parent: Excelling in the Workplace
---

# Understanding Agile

If you work in the tech field, chances are you will be working on an "Agile" team. This article will seek to explore 1. What is agile 2. Why do we want agile 3. How to be agile.

## Software Development Life Cycle

Before we get into agile, we need to talk about what "software development life cycle" is. It is a process for which developers use to create and release software. As there are multiple solutions to solve a problem, so are there many ways to create and release software.

## Agile History

Back before potentially many of you were born, some really smart developers met at some cabin and came up with the [Agile Manifesto](https://agilemanifesto.org/) which would revolutionize how the software industry works. Prior to this much of software was developed in a structured approach called [waterfall](https://en.wikipedia.org/wiki/Waterfall_model) where all the requirements for a project were set at the beginning, development would match those specifications, and then released when everything was done. This worked for earlier software projects where software was released on floppy disks and CDs and couldn't be altered. Then came the revolution of the internet and now software could be deployed at any time. This led to a whole new opportunities within the field, which as a result much of the industry has adopted this model.

## What is Agile?

Agile is a __development practice__ which involves discovering requirements and developing solutions through collaborative effort of self-organizing and cross-functional teams and their customer(s)/end user(s). Simply put - it is a set of values that emphasize iterative development based on the needs of the end users.

Those values are:
* **Individuals and interactions** over processes and tools
* **Working software** over comprehensive documentation
* **Customer collaboration** over contract negotiation
* **Responding to change** over following a plan

I would love to copy and paste more of the wikipedia, but do yourself a favor and just read it in full - [Agile software development](https://en.wikipedia.org/wiki/Agile_software_development)

### The MOST IMPORTANT TAKEAWAY

There is a ton of things to talk about agile, but the most IMPORTANT thing is the iterative mindset - the ability to identify a problem, try a solution, get some feedback, and determine what to do next. This rings true in every aspect of software engineering - from code to management, it is important that you approach every problem with an interative mindset.

For example let's say we like to use a certain naming scheme for our variables, but we identify that people are constantly getting errors because they are not using the correct variable. We have identified a problem "code is hard to understand because the variable names are hard to read" (identify a problem). One approach we can take is to change the way we name variables so it is more clear (try a solution). See how many issues related to variables pop up (get some feedback). And then accept this naming standard as a new best practice if there are less issues (determine what to do next).

Another example would be how we can change how the team communicates updates. Let's say that there is an issue where the team doesn't know what other team members are doing (identify a problem). We decide to try meeting every day at 9am (try a solution). We check back with the team in a week to see what everyone thinks about the 9am meeting (get feedback). And if everyone likes it we can make this a permanent meeting (what to do next).

For all of you middle school science classes, this is like applying the scientific method to our development process. With each new discovery, we understand a little bit about our workplace and we improve our working environment. When you hear about 10x developers (or whatever they're called now), it's near impossible to achieve the work of ten developers - but what you can do is try to bring out the best in your team members and synergize your team for the highest output. This concept is is drilled into our field - the ability to scale. Bringing out the potential of one person can only gain you so much, but when you can effect the team, department, and organization - you can easily see how effective one good engineer can be. Being able to identify problems in your working environment will allow you to solve those opportunities to will unlock that potential and bring real change to your work life.

#### How to identify opportunities for change

Finding change can be a challenge, but you don't need to be an expert to find them - you just need to be able to listen. You will find opportunities where you hear discomfort, annoyance, and friction. Does your team complain that there has been too many production issues - opportunity, grumbles when your team has sprint planning - opportunity, takes too long to develop - opportunity. Be the people watcher, and you will see some interesting things.

Be sure to catalog things that stand out to you, and soon enough you'll have more things than you can handle. For me I have a backlog (or list) of items that can be improved and go through them I see the opportunity.

#### How to identify good opportunities for change

Once you have an understanding of some of the areas of improvement, you'll need a system for determining what you can tackle now and what you can tackle later.

Some characteristics of things that can be tackled now:
* You have expertise in the area
* The improvement would have immediate benefits
* Has impact on those around you
* You have extra time

Some characteristics of things that **cannot** be tackled right now:
* You need to gain exposure to the subject
* You require resources you don't have at the moment
* You have too much work

#### How to tackle these opportunities

Approach the issue with the steps outlined earlier:
* Identify a problem
* Implement a solution
* Get feedback
* Choose to accept or reject the approach

#### Finding Blame

When something goes wrong, people are quick to blame others - and that holds true in the workplace. I've had a CEO call out a developer for some regression bug, mind you the developer was only a few years into the job. When you seek to find a loser, ultimately you will both be losers (See the 7 Habits book). For one the developer was publicly embarrassed and even submitted an apology to the CEO, probably instilling a sense of fear and shame into him which led to him leaving. And second as an observer I lost all respect for the company at that moment which was a factor in leaving as well.

Issues are inevitable, we've seen Netflix go down, Gmail go down, even AWS go down - and those companies spend billions on entire reliability departments. It is easy to blame people for problems, but it is hard to find the root cause of the issues. In this case - how did the code pass code review from senior managers, what QA or product owner didn't verify it in lower environments, why wasn't there a backup plan to restore services quickly? I don't imagine that's the responsibility of a junior developer - this is a team problem, and a great opportunity for change. But one comment from the CEO blaming a junior developer and you'll lose a lot more than whatever revenue lost during that period.

This was a roundabout way of saying that when you are looking for causes of the issues - people are just trying to do their best, and the issue was more likely than not due to lack of proper processes in place.

### Netflix, the Pinnacle of Agile Success

In my eyes, Netflix has implemented agile at the highest level and with the most success of any company around. You can find examples of agile deeply ingrained in their culture, and can see the results they have achieved with it.

Their product is deeply influenced by agile philosophy. Netflix is no ordinary video streaming business, they are constantly look at how they can best meet their users needs. From the instant you login, you are entering Netflix's iterative improvement engine. From the video content you watch creating a better predictive model for thing you'd watch, to if a thumbnail should play for a given video - Netflix is constantly testing different features and presentations to see what end users prefer.

For the development culture, it is known throughout the industry that they value independent engineers who will figure out how to work, rather than be told what to do. Neflix is known for their [culture deck](https://www.slideshare.net/reed2001/culture-1798664) which popularized them as THE gold standard for creating effective work culture. Their __core philosophy__ is **people over process**, a core ideal borrowed from agile manifesto.

They actively seek opportunities to find faults, so that they can squash issues before they even become issues! They popularized what is known as [chaos engineering](https://en.wikipedia.org/wiki/Chaos_engineering), which is the process of intentionally bringing down parts of the website in order to find issues and to increase resiliencies to downtime and to increase quality of service.
