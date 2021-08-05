---
template: post
title: KrakenD - Ultra-High Performance API Gateway
slug: /api-gateway-krakend
draft: false
priority: 0
date: 2021-05-16T12:00:02.039Z
description: Modern Opensource API Gateway offering lot of features, security with no compromise on Performance
category: technical
tags:
  - api
  - gateway
  - krakend
---

![logo](https://www.krakend.io/images/krakend-waves.png)

In this article, I will touch upon KrakenD which is a modern open source API Gateway return in Go Lang. Before, we dive into its capabilities, let's first understand what an API Gateway is.

An **API Gateway** is a an entry point for the clients to your microservices. It takes all API calls from clients, then routes them to the appropriate microservice with request routing, composition, and protocol translation. Typically it handles a request by invoking multiple microservices and aggregating the results, to determine the best path. An e‑commerce site might use an API gateway to provide mobile clients with an endpoint for retrieving all product details with a single request. It invokes various services, like product info and reviews, and combines the results.

KrakenD is a 'Pure API Gateway' and running a benchmark tests across test conditions , KrakenD outperformed competitors like Kong, Vulcand, Tyk thanks to its stateless architecture (benchmark links are mentioned in below sections). It sits between the client and all the source servers, adding a new layer that removes all the complexity to the clients, providing them only the information that the UI needs.

### Features of KrakenD

- Aggregates information from many sources into single endpoints.
- Manipulates responses and allows you to group, wrap, rename...
- Filters and shrinks responses, hiding unwanted attributes or selecting them
- Throttles (rate limits) connections against KrakenD and against backends
- Protects your backends with circuit breakers and implements all kinds of security measures.
- Discovers your service instances by integrating with your SD provider
- Extends your ecosystem as it supports a myriad of middlewares and plugins, such as OAuth or security layers.
- Fine control of manipulations, validations and filtering with DSL configurations

![features](https://www.krakend.io/images/KrakendFlow.png) _Source : https://www.krakend.io/_

### Why KrakenD ?

- Increase user experience in apps. Less data consumption and faster responses
- Instant creation of a new REST API
- Add APIs in legacy systems
- Unify data coming from different sources and encodings
- Publish a fixed interface, let the backends evolve and change contracts.
- Quick Microservices adoption
- Create aggregated views from a lot of services
- Smooth transition over different API version releases

### Performance Benchmarks

Performance is where KrakenD just outperforms all its competitors. Even on an ordinary laptop , it's able to serve ~18,000 requests/second.

Krakend team has done a good job at performing various benchmarking tests and making the results available. You can find it <a href="https://www.krakend.io/docs/benchmarks/overview/">here</a> . Detailed benchmark results <a href="https://www.krakend.io/docs/benchmarks/api-gateway-benchmark/">here</a>

#### Conlusion

If you are building applications those are cloud-native and rely on microservices pattern then you will have to depend on a reliable API Gateway. There are tons of Open source offerings available in this space namely Kong, Tyk etc also managed service which do serve the purpose but are not so well placed when it comes to Performance.

I always feel that the best comes out when you host it within your own ecosystem / environment and that's where KrakenD just stood out. It was flexible, easy to configure and most importantly 0 **Good Performance**. It offers incredible features out of the box (as mentioned above) along with good performance and security.

I am impressed and soon will be pubishing another post where we will see how to deploy KrakenD within Kubernetes (local laptop) and explore various features, designers etc.

Please let me know your thoughts on the same.
