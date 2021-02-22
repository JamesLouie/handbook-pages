---
name: Fundamentals of Good Code
nav_order: 6
parent: Excelling in the Workplace
---

# Fundamentals of Good Code

Another one of those topics where reading [Clean Code](https://amzn.to/3iIzw4h) is going to show you a lot more, but I'll try to explain what "good" code is, and how you can write good code as well.

## What is Good Code?

There is no such thing as perfect code, but good code - yeah thats more like it. Good code is code that does it's job and lands just long enough to be useful. Very ambiguous I know right, but that is the name of the game. We work in an ever-changing world, and so must our software change as well. We just have to find the right balance between the requirements to be good enough. If you haven't read the section on [pragmatism](https://thehandbook.jamlouie.com/excelling-in-the-workplace/pragmatism.html), you should read it now.

There are some basic principles we should all follow, but each has different importances depending on the situation. The same code put in different contexts can have totally different value.

Code made for user authentication will have totally different priorities compared to code used to track financial transactions. Everything is a trade-off, sometimes you will want speed, other times you will want consistency, and sometimes it just just makes sense to be more readable.

## Level 1: Foundational Principles

There are certain principles of good code that is universally valuable. You should try to write code that maximizes these principles.

### Maintainable

For me this is the most important attribute of good code - how well can we maintain this code. This principle is how easy this code is to work with. If code is not easy to work with, more than likely the next person to work on the code will pass it off as a bad solution and try and reimplement it or extend it improperly.

### Readable

The most underrated principle is how readable is your code. How quickly can someone understand a code block without prior knowledge. In the software industry, your code is never just your code and can change hands, so it's important for people to be able to read your code.

### Flexible

Code should be flexible so that it can adapt to changing requirements and usages. What was true one day may not be true the next, as the software requirements are fluid - one day we want PayPal as our payment provider the next we want to use Square.

### Testable

Code should be testable so that you can protect yourself against side effect of future changes. Having tests allow you to confidently make changes at the code level and verify you haven't made changes to the behavior during refactoring.

### Consistent

Code should be consistent across your application. The more uniform your code style, the easier it is to traverse different code within your application. It's important to say that doesn't mean not to change, but changes should be purposeful and should change the future direction of the application.

### Performant

Code should be performant because of the nature of technology and scalabilty. Code can be used for one user or a million users, small problems can turn into big problems very quickly.

One especially important mention for this section is the overvaluation of this principle and the trap that it can put developers in. The issue is with over-optimization, where you are spending time for value that may never be needed. This may sound contradictory to the the above statement about scalability, but this is one of those things you need to approach with pragmatism and your decision-making builds with experience.

## Level 2: Design Principles

The second level of design principles applies the foundational principles into practical advice.

### Keep it Simple, Stupid (KISS)

Code that is simpler is better than code that is complex. When code is complex, it makes it harder to maintain and takes more time and effort to read and change. That is not to say there is no complex code in the world, but try to simplify it such that it removes unneccessary ambiguity.

### Don't Repeat Yourself (DRY)

Code is power because it defines a specific set of actions, once defined never has to be defined again. Unfortunately that is not the case and we repeat our code all over the place. Copy...Pasta... all over. We realize we need to change that code, now we have to find all the instances of that copy/paste and update them to follow the new pattern.

Within applications we usually create some abstraction around this by creating a utility class or create a shared library to resolve these kinds of issues.

One major trap is trying to abstract two things that are not the same, leaving you with code that is worse than before! It is important to apply this principle where it makes sense, and it is okay to have code that may look alike if it truly is something different.

### Single Responsibility Principle

The single responsibility principle is the idea that one class does one thing. This is a way of thinking helps you decompose your code into little building blocks, which makes your code much more extendable because you have clear boundaries between different code segments.

This is the S in [SOLID](https://www.freecodecamp.org/news/solid-principles-explained-in-plain-english/), a set of popular object oriented design principles. I'll include a few more that I believe are essential, although all of them play a role.

### Dependency Inversion Principle

This is one of those harder to grasp topics unless you've seen or written code against this, but this is that your classes should depend on __interfaces__ or __abstract classes__ instead of concrete implementations because it forces you to come up with contracts between two classes which allows you to swap out different implementations depending on the situation. For example in the payment processor example earlier we might have a `PaymentProcessorInterface` class and have three classes: `SquarePaymentProcessor`, `PaypalPaymentProcessor`, and `UnitTestingPaymentProcessor` which we can inject into the caller class depending on the situation.

This is the D from [SOLID](https://www.freecodecamp.org/news/solid-principles-explained-in-plain-english/).

### Composition over Inheritance

When it comes to relating code, you have two strategies: inheritance or composition.

Inheritance is when you say that something is something else. For example a Tesla Model X is a car.

Composition is when something is composed of multiple other things. For example a Tesla Model X has a steering wheel, seats, some wheels, and much more.

It's much better to think in components compared to inheritance, because inheritance implies a lot more and if used improperly can make your code incorrect. It's better to treat code as components which can be swapped around like Legos to create new results.

### Reducing Side Effects

A big push in the industry to is move towards functional programming, and for good reason - state is generally increases complexity. That is why many developers love writing "pure functions", which are functions with clearly declared inputs which results in outputs without side effect (affecting any form of state - object state, network, database, etc) until the last possible moment.

Tons of good information in this [article](https://towardsdatascience.com/why-developers-are-falling-in-love-with-functional-programming-13514df4048e), and much more on the internet about how functional programming can reduce side effects.

In the field I generally think there is room for both object oriented and functional programming, and they are both tools for you to create good code. The real secret is to know in what situations they apply to and what is better for your team.

## Write Code that Has Value

There is a lot of theory and philosophy in this section, but the ultimately good code is something that has produces value. You'll hear time and time again how many of these super successful tech firms are held up by some old monster of a code they built back when they were starting out that runs the core part of their business. It might not be the most artistic code you've ever seen, but what is create crucial value and it works - and that's all it really needs to do.