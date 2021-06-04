---
name: Blocking vs Non-Blocking IO
nav_order: 4
parent: Technology Talks
---

# Blocking vs Non-Blocking IO

In the world of software systems, one of the most fundamental things to performance is understanding the path that your code takes and where the performance bottlenecks are. In school we are taught all about data structures and algorithms which are important when we code, but this doesn't include the whole system - all the other systems we have to interact with.

Especially important in the distributed systems world, where internal code calls are now to external services over the internet, we are moving to a more and more latency heavy system. Where we could get information from a constants file which would be on the order of a nanoseconds while a http call could take a few milliseconds.

## What is a Blocking IO Call?

A blocking IO call is when there is some IO (Input/Output, communication with out of process system) holds onto a system resource (thread) until it has completed.

For example this blocking IO call could take the form of an HTTP request from one service to another service, or a service requesting data from a database. It is common for requests to contain at least one of these types of calls - and given the current world where we need systems to handle millions of requests, you can see that there is no way that your servers will be able to handle this amount of traffic if each requests takes a thread and waits for it to complete.

## What is Non-Blocking IO?

Non-blocking IO (NIO) has been around for a while, and is an essential solution to the problems above. Non-blocking means that when a IO action is needed, it will pause and release the current thread and wait for the external resource to come back with the results before executing the rest of the work.

With this model, threads are freed up to continue processig requests, with the waiting being done by usually some lower level construct of the operating system.

This is how something like Node.js, which is single threaded, can handle millions of requests because it delegates off all the waiting to the operating system while it manages the incoming requests.

## Further Readings

* [Explain Non-blocking vs blocking like I'm Five](https://blog.codecentric.de/en/2019/04/explain-non-blocking-i-o-like-im-five/)
* [How does non-blocking io work under the hood](https://medium.com/ing-blog/how-does-non-blocking-io-work-under-the-hood-6299d2953c74)
