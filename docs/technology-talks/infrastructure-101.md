---
name: Infrastructure 101
nav_order: 1
parent: Excelling in the Workplace
---

# Infrastructure 101

If you thought code is where your job ended, that is just the tip of the iceberg. Infrastructure is what make your code actually run.

## Components of Infrastructure

There are two main components of infrastructure:
* Hardware
* Software

### Hardware

Hardware is the physical components like the computers, routers, datacenters, etc that brings your code to life. Hardware is important because it defines the resources that your application has to work with. Finding the right balance of cpu, memory, networking and disk performance is important to performance and cost.

### Sofware

Software is the logical components applications and operating systems that runs on the physical hardware to execute your code. The software is important because it is the medium for which hardware is able to interpret the code you wrote. It's important to know what environment your code will be running in, for example if you develop on a windows machine but deploy to a linux environment, you could potentially experience different bugs from a library's implementation.

## Types of Infrastructure

There are two main types of infrastructure:
* On-Premise (also called 'bare metal')
* Cloud

### On-Premise

This is when your organization's IT department owns and manages it's own physical servers and datacenters. They have a dedicated IT department that maintains and acquires new hardware to run your applications.

On-Premise is considered the 'traditional' option because it existed before cloud was available. It is good for supporting existing systems (if it ain't broke then don't fix it).

### Cloud

Cloud is when your organization is using infrastructure hosted by another company (AWS, Azure, Google Cloud). The cloud company runs a server center and then rents out computing/hardware space to other companies.

Cloud is great for companies that don't want to invest in an IT department. It allows smaller companies to setup infrastructure without buying actual hardware, and then it also allows you to scale resources as much as you have money.

## Types of Software Cloud Deployments

Within cloud deployments, there are a couple ways of deploying applications that take advantage of the scalable infrastructure.

### Containers

The most popular form of cloud deployment is to deploy your applications in a "container", which is a special run-time that includes the application and it's dependencies so that it can be delivered consistently across different types of hardware. This is important because in the cloud environment, you may not know exactly what system your code will be deployed which is why containers are so important to the cloud eco-system.

#### Kubernetes (and other container orchestration)

Building upon the idea of delivering containers to the cloud, there was a need to create a system that would facilitate the delivery of your containerized code to the cloud. That is where systems like Kubernetes (container orchestrator) to be the brains that manages where containers get deployed and how all the resources sync up.

### Serverless

Then we have serverless, which is the idea that you don't know anything about infrastructure and you only worry about the code and let the infrastucture build itself around your code. You can deploy a code snippet and let the cloud determine what will run your code.

