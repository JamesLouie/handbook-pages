---
name: Describing Software Architecture
nav_order: 2
parent: Technology Talks
---

# Describing Software Architecture

Talking about software can be hard some times, because software covers the entirety of a field. There are different levels that people look at it through, and each level has different language. Let's think of an example scenario - you get two developers in a room and you ask them the white board the architecture of their software system. More likely than not, the two pictures created can look vastly different. One developer may focus on the "code" architecture and may emphasize how the different code components fit together. The other developer may focus on the relation between systems and how they communicate. Neither answer is right, in fact both pictures are probably 100% correct. The difference is how the developers chose to represent their software architecture.

![Whiteboard Example](https://miro.medium.com/max/700/0*vKpLnPmklW2PkB2t.jpg)
[White Board Example, c4model.com](https://c4model.com/)


One system that seeks to solve this problem is called [C4 Model](https://en.wikipedia.org/wiki/C4_model) and it attempts to create a common language that we can use to discuss software systems on every level - from code to systems.

The C4 system is composed of:
* **C**ontext
* **C**ontainers
* **C**omponents
* **C**ode

Each _C_ represents a different level of abstraction that allows us to create a separation of specificity of our system. Each level of abstraction can serve to describe how granular we want to describe it to serve different purposes — Do we want to describe the overall structure of our systems to IT infrastructure team, or do we want to define the dependency of an existing service we are changing.

![C4 Model](https://miro.medium.com/max/700/0*SyYMkFlmlNqyLskL.png)
[C4 Model, Simon Brown](http://www.codingthearchitecture.com/blogentries/7.html)

Watch the [Youtube video](https://www.youtube.com/watch?v=x2-rSnhpw0g) for an in-depth explanation by the creator Simon Brown.

## System Context

The System Context level defines the highest level of abstraction of our architecture. In this level we describe components by separation of complete systems, where a system is a collection of related “containers” or deploy-able applications. This level is useful for describing the overall structure of the complete system and what the high level integrations between systems are. This can be useful for audience to make larger non-technical decisions to match the owner’s initiatives.

Layer Terminology: System, People

## Containers

The container level defines the layer where we start to describe boundaries between each deploy-able application. By organizing our structure into containers, we can start to define the structure of a system. This level is helpful for the main development team of the system and technical parties evaluate changes and diagnose issues.

Layer Terminology: Deployments, Hosting, Resources, Application, Database, API, Website

## Components

The component level defines how a container is logically split up between its different parts, so that you can inspect the general design of a container. This view is useful to see which technologies implement specific parts of a container. This level is generally used for the planning stage of developers as they start to work on features. The structure is usually defined by the software architect.

Layer Terminology: Frameworks (ASP.NET, Entity Framework, Serilog, Autofac, etc), Libraries, Projects

## Code

The code level defines how the components are actually implemented.This level can be considered optional by the standard, due to its difficulty to maintain, and little advantage it brings over having the code base itself.

Layer Terminology: Classes, Interfaces, Design Patterns, Languages

***

Originally published on [Medium](https://jameslouie12.medium.com/c4-model-describing-software-architecture-55565dddd660).