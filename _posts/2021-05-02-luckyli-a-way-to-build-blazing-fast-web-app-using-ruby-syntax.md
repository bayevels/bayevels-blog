---
layout: post
title:  "Luckily I find a way to build blazing fast Web Apps using Ruby syntax"
description: Introducing my idea of building a super simple yet super powerful :) plateform that will let job seekers find easily job offers and job offerers create understandable job posts within a **WEEK** from now (Monday 19th 2021) to the next Monday
categories: WebDev
tags:
  - Lucky
  - Rails Like
  - Crystal
  - Software development
keywords:
  - Lucky Framework
  - Crystal Language
  - APIs
  - Ruby Syntaxe
---
Let me introduce to you [Lucky](https://www.luckyframework.org/) a blazing fast web framework written in Crystal.

But wait, yet another language to learn.

If you're a Rails developer or you use Ruby regularly, Crystal is a great option to look for when building type checked and blazing fast apps using the Ruby syntax, the learning curve is almost near to 0 for you. 

If you're not familiar to Ruby, it's probably one of the most _programmer happiness centric_ scripting language and reading or writting Ruby code feel generally like reading or writting english. Crystal main aim is to recreate the efficiency and friendliness of the Ruby language in a compiled and typed fashion 
> We love Ruby's efficiency for writing code.
> 
> We love C's efficiency for running code.
> 
> We want the best of both worlds.
> 
> We want the compiler to understand what we mean without having to specify types everywhere.
> 
> We want full OOP.
> 
> Oh, and we don't want to write C code to make the code run faster.

# Crystal Lang
**Crystal** is a compiled programming language with a syntax similar to **Ruby** (but compatibility is not a goal). The v1.0.0 was released on [March 2021](https://github.com/crystal-lang/crystal/pull/10500). Crystal has a good community support with more than 16k stars on Github at the time I write this blog. Crystal docs and guides are also really great and concise and you can learn and grasp the language at the speed of light :). Crystal is typically accompanied by [Shards](https://crystal-lang.org/reference/the_shards_command/index.html), its dependency manager.

# Lucky Framework
Lucky is a Rails like Framework written in Crystal with a great, clear and concise documentation, according to the TechEmpower web framework benchmarks [Round 20](https://www.techempower.com/benchmarks/#section=data-r20&hw=ph&test=json&c=e), Lucky is one of the fasters framework out there. the key point to notice here is Lucky is not a micro framework it's a "Full-Stack" frameworks that provide you all the necessary tools to build complete web apps.
![Web Framework Benchmarks](/assets/images/webframeworkbench.jpg)
[Lucky](https://www.luckyframework.org/guides/handling-files/file-uploads) comes with all the good stuffs like HTTP and Routing, Frontend and HTML, Database, JSON and APIs, Authentication, etc... When it's come to specific thinks like file attachement you can quickly find a shard that does the work for you. Shards are generally heavily inspired by Ruby gems, this makes then really easy to use when you have experience with the Ruby version. For exemple [shrine.rc](https://github.com/jetrockets/shrine.cr) used for file attachment is inspired by [shrinerb](https://github.com/shrinerb/shrine). You can use [Awesome Crystal](https://crystal.libhunt.com/) a curated list of awesome Crystal shards, tools and frameworks to find quickly the shard that you're looking for.

# How requests are processed
![Requests Overview](/assets/images/request-overview-diagram.png)
1. Browser or client makes an HTTP request.
2. Lucky routes the request to a matching Action.
3. Action processes the request. For example:
  * Query the database with [Avram](https://www.luckyframework.org/guides/database/intro-to-avram-and-orms).
  * Create or update db records with [Avram](https://www.luckyframework.org/guides/database/intro-to-avram-and-orms).
  * Send an email with [Carbon](https://www.luckyframework.org/guides/emails/sending-emails-with-carbon).
4. The Action generates a response for the browser or client. For example:
  * Generate an HTML page.
  * Redirect to another URL or Action.
  * Send JSON.
* Finally the response is delivered to the browser or client.

# Wrap Up
I think that Lucky is great tool for teams that are already familiar with Ruby using Ruby On Rails or Sinatra and have  of the systems that they maintain. 
To keep this post concise, I have wrote a post where I have builded using Lucky a "car model data" api that return YEAR, Make, Model and Body style of nearly all cars manufactured between 1992 and 2020 approximately 10K car models. I try to explain there in detail how to build APIs using 
## Useful links
* [Lucky](https://www.luckyframework.org/)
* [Crystal Lang](https://crystal-lang.org/)
* [Action](https://www.luckyframework.org/guides/http-and-routing/routing-and-params)
* [Avram](https://www.luckyframework.org/guides/database/intro-to-avram-and-orms)
* [Carbon](https://www.luckyframework.org/guides/emails/sending-emails-with-carbon)
* [Lucky is lightning fast!](https://dev.to/konung/lucky-is-fast-2gpp)