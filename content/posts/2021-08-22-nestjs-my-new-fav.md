---
template: post
title: NestJS - My new favorite framework
slug: /nestjs-framework
draft: false
priority: 5
date: 2021-08-22T12:00:02.039Z
description: Why NestJS is my goto framework these days.
category: coding
tags:
  - nestjs
  - javascript
  - framework
---

![logo](https://d33wubrfki0l68.cloudfront.net/e937e774cbbe23635999615ad5d7732decad182a/26072/logo-small.ede75a6b.svg)

This article is rather special to me as I never taught I would write an article on a framework that's based on JavaScript. In my decades of experience, I have always been designing APIs using Java frameworks like SpringBoot, JPA etc. I never found Javascript to be an alternative to Spring considering code structure, dependency injection etc.

Last year when I was browsing through courses on Udemy, I came across a course from Airel Weibenger on NestJS. The course was short so I decided to give it a shot. Never did I feel that this course would make me fall in love with NestJS. The code convention, architecture, code isolation resembled what I have been loving in SpringBoot and this gave me a chance to try it out and let me tell you, it's an AWESOME framework.

Why would you choose NestJS, over the widely-used, well-known, and ‘usual’ frameworks, you’re quite used to? Perhaps, you want the development process to complete quickly and efficiently by using the boilerplates and controllers. Maybe you want to build scalable and easy-to-maintain apps. Or, you just want to choose a convenient and effective framework to work with. Let me assure you, NestJS fulfils all these needs.

**NestJS** is a framework for building efficient and scalable Node.js server-side applications built with and fully supporting TypeScript. It uses robust HTTP Server frameworks like Express or Fastify. It provides a level of abstraction above the common Node.js frameworks and exposes their APIs to the developer. This gives a great amount of freedom to use third-party modules.

A good reason to choose NestJS over ExpressJS (one of the most popular Node.js frameworks) is the fact that when a new project in Node.js is started it is a clear architecture based on a few simple components (controllers, modules and providers). This gives great ease to split applications into microservices.

## What is NestJS?

As mentioned, NestJS is an open-source, extensible, versatile, progressive Node.js framework for creating compelling and demanding backend systems. It is currently the fastest-growing Node.js framework in TypeScript.

NestJS is used for writing scalable, testable and loosely coupled applications. It brings scalable Node.js servers to a whole new level. It supports databases like PostgreSQL, MongoDB, MySQL. NestJS is heavily influenced by Angular, React and Vue and offers dependency injection right out of the box.

As of August 2021, it has over 39.8k GitHub stars and its weekly npm download rate is almost 775k. It encourages developers to try, learn and use some well-known software development paradigms and its documentation has lots of examples, recipes and code sources.

NestJS is easily extensible, as it can be used with other libraries; versatile thanks to its adaptive fully-fledged ecosystem and progressive, bringing JavaScript features and design patterns.

## Building blocks of NestJS

**Modules:** used to organize the code and split features into logical reusable units. Grouped TypeScript files are decorated with “@Module” decorator which provides metadata that Nest makes use of to organize the application structure.

**Providers:** also called services, which are designed to abstract any form of complexity and logic. Providers can be created and injected into controllers or other providers.

**Controllers:** responsible for handling incoming requests and returning appropriate responses to the client-side of the application (for example call to the API).

In addition, it also has **Service** and **Repository** concepts. It also has great integration with ORM frameworks like TypeORM, Sequelize and Mongoose.

## Why Nest.js?

Many reasons make Nest.js preferable over other NodeJS frameworks, some of them are:

- It leverages TypeScript - strongly typed language which is a superset of JavaScript
- Support Monorepo
- Made for monoliths and microservices
- DevOps support is ready
- Powerful CLI to boost productivity and ease development
- Detailed and well-maintained documentation
- Active codebase development and maintenance
- It is open-source (MIT license)
- Support for dozens of nest-specific modules that help you easily integrate with common technologies and concepts like TypeORM, Mongoose, GraphQL, Logging, Validation, Caching, WebSockets and much more
- Built-in support for microservices & transport layers
- Dependency injection container
- Easy database interaction
- Framework adaptive nature
- Domain-driven development
- Built-in Exception Filter
- Use of third-party modules
- Dependency Injection

NestJS with its out-of-box microservice architecture (similar to Angular.js), makes developer’s life a lot easier and happier by enabling them to build scalable, loosely coupled, highly testable, and easily maintainable applications.

If you are having second thoughts about whether or not Nest is for you or not, you should check out the Nest CLI- A Command Line Interface (CLI) is the tool that assists in multiple ways- from helping in initialization and development to maintenance of the Nest applications.
Not only does the Nest CLI assist in project scaffolding and building applications for production but also embodies best-practice architectural patterns.

You can install the Nest CLI and set up a new project using the following command -

```
npm i -g @nestjs/cli
nest new project-name
```

**Framework Independence**: Under the hood, Nest uses powerful HTTP server frameworks like Express and is also compatible with other frameworks such as Fastify. Nest makes use of a framework adapter to achieve this framework independence that works as a proxy middleware to carry out some library-specific implementations.

### Summary

Java as a programming language is more than 20 years old. For many years, it was the main framework for creating business applications, but recently, the focus shifted towards Node.js. Because of its speed, Node.js took the developer world by storm allowing one to enjoy all the benefits of JavaScript and writing both frontend and backend in the same programming language.
NestJS gives developers a great head start. All you need to start the development is to set up a new app and you are ready to go. This framework gives you a huge boost right at the very beginning while helping you take further steps by defining proper app architecture.

NestJS uses modern solutions and technologies, so the applications created with it are maintainable and long-lasting. It can be connected with GraphQL, WebSockets or used for building microservices.

If you want to know more about NestJS, let me know in the comments. Till then, Signing off !!
