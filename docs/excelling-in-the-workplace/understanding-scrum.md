---
name: Understanding Scrum
nav_order: 7
parent: Excelling in the Workplace
---

# Understanding Scrum

Now that you learned a little background about agile (if you haven't yet please refer back to [Understanding Agile](https://thehandbook.jamlouie.com/excelling-in-the-workplace/understanding-agile.html)), agile is a philosophy and scrum is a popular "implementation" of that philosophy. It takes the ideals and turns them into concrete "ceremonies" that teams can use to work in an agile way. This is a very popular framework that has been used at every job I've worked at, so chances are you will experience it at some point.

As always there are tons of online resources to learn about scrum, I would suggest [Atlassian Scrum doc](https://www.atlassian.com/agile/scrum) to read in-depth, but I'll try to give some thoughts from a development and management point of view.

## Product Team

Scrum teams are organized as **Product Teams** within an organization. Product teams are long-lived teams that are responsible for maintaining and make updates to a business feature or need. This differentiates from previous approaches where teams where "project teams" which developed a single project and moved on to another project.

For example in a ecommerce website, there might be a product team for "Catalog" which is in charge of making sure that the company can manage their product information. This differentiates between a project where they might request a new business process for uploading items to the catalog.

Product teams are based on the idea that the team will be more foundational, which promotes more longer term thinking. Project teams on the other hand are known to get in and then get out, leaving a trail of spaghetti behind and some other team to pick up.

## Ceremonies

**Sprints** - These are defined blocks of time (usually two weeks) that an agreed upon set of work should be completed (not really a ceremony but important)
**Sprint Planning** - The team takes a couple hours to decide what they will work on for the next Sprint
**Sprint Grooming** - The team takes some time to review incoming work and make sure the requirements makes sense to the team and is ready to work on
**Daily Standup** - Some time set aside each day to give updates and check if anyone is blocked (cannot work on) on a certain task in order to see if others on the team can help resolve it
**Retrospective** - (The most important ceremony) The team spends some time to reflect how the past Sprint went and see if they can make any improvements

[Ceremonies - Atlassian](https://www.atlassian.com/agile/scrum/ceremonies)

## Typical Scrum Workflow

Here is an example of how Scrum works in practice.

1. Sprint starts on Friday morning (it can be any day of the week as long as it's consistent)
2. Developers will pick up their new set of tasks for the sprint
3. Development team will meet at 9am in the morning for standup (which will repeat every day)
4. Development team meets the next Wednesday to groom incoming work
5. Development team meets the following Wednesday to plan the work for the next sprint
6. Development team meets on Thursday (day before sprint ends) for retrospective.
7. Start of next sprint on Friday (2 weeks after the start of the week)

## Scrum needs agile philosophy to work

Scrum was created to implement agile philosophy in the practice, so it only makes sense that you would need to follow agile philosophy to make it work. It's like you go to the basketball court without basketball. You can pretend to play basketball and go through the motions, but you won't be getting anything done - people will just be going through the motions without understanding why. If you don't approach Scrum with an agile mindset, you will not be productive as say another methodology/framework like waterfall.

To successfully run these ceremonies, it is important to understand the **intent** of each of the ceremonies. The "why" of the ceremonies.

Why do we need Sprint Planning? We need to identify how much work the team can take on and what we tell the business we will be delivering.

Why do we need Sprint Grooming? We need to understand the requirements of the work and make sure we have all the details before starting.

Why do we need Standup? We need a constant flow of information between team members to facilitate collaboration.

## Why Retrospective is the most important ceremony

Retrospective is the most important ceremony because it gives the team an opportunity to improve their workflow and create lasting change. All the ceremonies are more functional in getting the work done for that sprint, but retros are different because they allow the team to make changes that can potentially impact the future of all the following sprints.

Retro (short for retrospective), is when the team sits down and talks about "what went well" and "what didn't go well". During this time the team will provide feedback, usually through sticky notes, and then the team will talk it out and see what they think. Things that went well should be repeated, and things that didn't go so well are those areas of improvement that the team can reflect on and come up with strategies to resolve those issues. Then those strategies are turned into action items for the team to try to resolve in the next sprint.

From my experience this is also the hardest ceremony to get right, as there are a lot of barriers to get through if the team is not sold on the agile philosophy. If people use this time to blame others, retros can become arguments. If people aren't thinking of problems, there's nothing to talk about. If people don't feel comfortable speaking, the meeting will be silent.

## The Backog

Around the idea of the ceremonies is a tool called "The Backlog", which is a prioritized list of work that needs to be completed. The highest priority work is at the "top" of the backlog and when work is needed it is pulled from the top. The lower the work is on the backlog, the less "ready" or less priority is has.

Backlogs are continuously "groomed" depending on changing business or technical needs, and is seen as a living document.

[The Backlog - Atlassian](https://www.atlassian.com/agile/scrum/backlogs)

### Epics

Epics are large bodies of work that take longer than one sprint and is composed of many stories.

[Epics - Atlassian](https://www.atlassian.com/agile/project-management/epics)

### Stories

Stories are units of work that contain general explanations of the software feature from the perspective of the end user. These units of work should be able to be completed within a single sprint. If they potentially take longer than a sprint, then the work be split up to multiple stories.

They follow the template: `As a [persona], I [want to], [so that]`

The purpose of describing software features in this way is to focus on what will bring value to the users. By defining that as part of the description, the work that leads up to that feature will be focused on what we can deliver to the users. This allows the team to focus on what can deliver that value, instead of some specific software implementation. Often times the team can come up with a variety of different ways to solve that same problem.

[User Stories - Atlassian](https://www.atlassian.com/agile/project-management/user-stories)

## Team Roles

Within a Scrum there are three roles:

* Development Team
* Product Owner
* Scrum Master

Although there are defined roles, each team member can contribute to any work needed for the success of the team. For example the development team can step in and assist with some product requirements for the product owner where necessary and vice-versa depending on their skills.

[Scrum Roles - Atlassian](https://www.atlassian.com/agile/scrum/roles)

### Development Team

The development team consists of all the team members that create value (deliverables). This can be engineers, designers, etc. 

### Product Owner

The product owner is the captain of the ship. They decide what direction the team should be moving towards. That means they work with the business to define the features that will be implemented as well as define priority of incoming work.

They are also the first line of defense against business needs, as they can determine what is priority and what does not. 

### Scrum Master

The scrum master is in charge of making sure that the team is running effectively and following agile principles. They serve as a "servant-leader" which leads by serving the needs of the team. They run the ceremonies, make sure the backlog is clean, tries to unblock development team, clarifies ambiguities about the scrum process and makes sure that discussions are healthy.
