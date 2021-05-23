---
name: Types of Software Architectures
nav_order: 3
parent: Technology Talks
---

# Types of Architectures

It is important to understand the different types of architectures because each type brings different benefits and drawbacks. Learning them will enable you to make more effective code level decisions and create more effective systems.

## Monolith

The monolith is the basic building block of all architectures...before there was only one! You are in a monolith all the code is in one repository using the same set of server, database, and other sets of resources.

### The King on Simplicity

When we think of our code, one of the golden rules is to keep is simple. From an architecture point of view the monolith is that solution, keeping everything simple. All of your code is in one place, they all share the same resources, all calls are within the code itself so you don't worry about network failure and remediation, and much more.

The general rule in the industry is to start with a monolith, and as your system evolves and you learn more about it - can begin to think about what can be separated out.

### Sometimes the Shoe Doesn't Fit: Being Too Narrow

The industry is trending less towards having a monolithic system because it doesn't give them the flexibility they need.

You lose the flexibility of choosing the right programming language for the job. For example you may find you want to use weakly typed language instead of a strongly typed language in some situations.

Your teams are stuck to the same code repositories. As teams scale up, you can start with 5 developers on one codebase and end up with 50 developers working on the same code. This increases the complexity of collaboration and decreased overall productivity.

## Distributed Monolith

As teams begin to scale out and want to own their own repository, then they may have different code bases but deploy in the monolith pattern of using the same server, database, and other resources.

### One Step Forward, Two Steps Back From the Monolith

As organizations have scaled, some have chosen to go to the distributed monolith pattern, which seemingly presents the benefits of distributed systems without the complexity of distributed systems - but in reality doesn't get the benefits of either and all the drawbacks of both of them.

You are losing a lot of the simplicity of the monolith like single code deployment, available code packages, cross-cutting concerns, easier testing but also gaining the complexity of more complex code pipelines, requiring a strategy for sharing code, having to create infrastructure to support cross-cutting concerns, and adding the headache of distributed transactions between different segments of your monolith.

From my experience, I highly discourage this architecture from being used unless there is clear benefit for your organization.

## Distributed Systems

Distributed systems is when teams decide to split out their system into individual systems that have their own set of servers, databases, and resources.

### Expect For Failure

When we are working in a monolith environment, you can expect to some extent that when you call a piece of code from your code it will execute without fail. In distributed system world you will probably be communicating via the network which can go down for a variety of reasons (data center is down, machine is not responded, network outage, etc). This leads to a variety of weird behavior where your system might be working, then down for five minutes, and then back up the next moment.

### With Great Power Comes Great Responsibility

Distributed systems becomes the clear path for many teams as they begin to scale from small teams into larger organizations. There is only so much that you can do on a shared codebase. Distributed systems allows teams to define system boundaries between other teams and allows them to run fast within those boundaries.

The flexibility provided by distributed systems is often the driving factor when teams choose to go down the distributed systems path. Developers and teams have a higher degree of freedom to choose the right technology that will allow them to succeed.

Often this freedom can be overwhelming, as distributed systems introduce a lot of complexity that was previously not experienced when working on the monolith. These problems are relatively new and there is not a single accepted solution to them, so this can lead to variety of different solutions that may or may not solve all of the problems for you. 

If you are working in or moving to a distributed systems architecture - be ready to work through all of the complexities that they come with.

### Event Driven Distributed Systems

Event driven distributed systems is a special version of distributed systems that use events to collaborate. Systems emit events and others react to those events and may create events of their own.

I chose to include this particular architecture on top of distributed systems because this is a paradigm shift from the traditional procedural patterns used in code and many synchronous communication distributed systems. Event driven distributed systems have a totally different workflow compared to that model where you are building decoupled systems that interact only through shared events.

This type of system is great for building decoupled systems, but comes with it's own complexity by pushing the boundaries of what is distributed, in this case even behavior becomes decoupled which means it may get harder to reason about what your system is doing because things are happening all over the place. The tooling has yet to catch up to this model and I've seen new teams trying to take on this model crushed with the complexity. With that said I do think there is a future for this down the line as tooling matures and developers get more experienced with this way of thinking.