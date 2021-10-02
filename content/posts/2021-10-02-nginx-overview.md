---
template: post
title: Nginx - Overview
slug: /nginx-overview
draft: false
priority: 5
date: 2021-10-02T12:00:02.039Z
description: Popular server when it comes to Reverse proxy, load balancing, performance.
category: nginx
tags:
  - nginx
  - reverse proxy
  - load balancer
  - performance
---

![logo](https://cdn.icon-icons.com/icons2/2107/PNG/256/file_type_nginx_icon_130305.png)

Over the past few years, I have started using Nginx extensively and had few hiccups understanding various components, rewrites and many more. Over the next few weeks, I will be publishing short tutorials on Nginx where we will cover the important aspects and how to use them effectively to get your application up and running with greater speed and efficiency.

To begin , let's understand what Nginx is and how is it different from Apache Server.

## What is Nginx ?

Nginx was created by Igor Sysoev in 2004 when he was not happy with Apache and eventually wanted to build a replacement which is capable of handling 10000 concurrent connections with focus on high performance, high concurrency and low memory usage.

Nginx today serves the majority of the world's top 500 websites. This growth is largely not just due to its performance but also because its easy to get started with. It's really good at making practical tasks such as caching or video streaming very easy to implement.
And cherry on the cake there's a large number of first and third party modules which help extend its core functionality.

Most people consider Nginx as a Web Server but thats not true. However, it's an reverse proxy server at its core, and it's because of this design that it performs so well.

## Difference between Nginx and Apache

By default, Apache is configured in what's called a **pre fork** mode which means it spawns a set number of processes, each of which can serve a single request at a time, regardless of whether that request is for a script or an image or something else.

Nginx, on the other hand, deals with requests asynchronously, meaning that a single process can serve multiple requests concurrently with that number, basically just depending on the system resources available to the Nginx process. That said, because of this asynchronous design, Nginx, unlike Apache, can't embed server side programming languages into its own processes, meaning that all requests for dynamic content has to be dealt with by a completely separate process like FPM and then reverse proxy back to the client via Nginx.

Of course, not having to deal directly with embedded programming languages like Apache, does makes Nginx a lot less resource hungry.

Unlike Apache, the server side language modules don't need to be run for every single request the server receives.Instead, Nginx will handle serving static resources without ever knowing about it, whereas Apache will handle every request with that costly overhead.

So essentially a well configured Nginx Web server serving mixed content, meaning both static and dynamic resources, should always be more efficient and less demanding on system resources than a similar Apache set up.

## Performance - Nginx vs Apache

You've most likely read or heard that Nginx is faster than Apache. Nginx can't magically deliver data to the client any faster than the Internet connection will allow but it can serve static resources much faster than Apache and is able to handle a much larger number of concurrent requests.

Remember, Nginx will serve static resources without the need to involve any server side languages and this gives it quite an advantage over Apache. And as for handling concurrent requests, Nginx can potentially receive thousands of requests on a single processing thread and respond to them as fast as it can without turning down any of those requests.

Apache, on the other hand, will accept requests up to the pre configured number and then simply reject the rest.

So if we define performance or being fast in terms of how many clients can be served under high load, assuming the usual mix of static and dynamic resources, then yes, and Nginx is definitely faster than Apache.

## Installing Nginx

You can download the distribution based on your operation system from here : https://nginx.org/en/download.html

Installation is self explanatory and straightforward.

- On MAC OS, you can install it directly from homebrew `brew install nginx` . How installed, you can restart your shell session and execute `nginx` to start and `nginx -s stop` to stop the server.
- On Ubuntu , `apt update && apt install nginx -y`. Here, its started by default and you can stop it using `service nginx stop`
- On Windows, you can follow the wizard and start/stop using the windows services.

## Summary

Here we saw the basics of Nginx and the differences with the Apache server. We also saw why it's faster and can handle concurrent requests.
In the next tutorial, we will see about **Nginx configuration , Virtual hosts , Location blocks and more**. Till then, happy learning.
