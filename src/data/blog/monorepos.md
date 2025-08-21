---
title: Monorepos
author: Chris Pieri
pubDatetime: 2025-08-01T07:00:00.000Z
slug: monorepos
featured: false
draft: true
tags:
  - monorepo
description: The only thing that will save your job from the AI
---

A Monorepo is a tool to combat coupling and improve cohesion.
Read on the learn how monorepos can help manage complexity in your codebase.

## Table of contents

## The accidental monolith 

A team is assembled to begin work on a new project. Requirements are set, stakeholders are excited, the team is stacked, everyone is getting promoted once this is done! Somebody cracks there knuckles and everyone gets started.

Features ship, users are impressed, and the app grows. At this point upper management begins to notice.
They're so impressed they decide to spin up a second team to build on top the success. 

The feature requests keep coming. Your not sure how to handle the new team so you carve out part of the application
for them to use.

When you finally look up, you realize you now have 30+ developers working on the app spread across multiple teams each focusing on it's own *kinda* related domain.

Now every release requires sign-off from every team. CI times are creeping into hours. Your bundles are bloated, flaky tests are multiplying, and deployments feel like an O(n) problem—where n is the number of teams involved.

What went wrong?

## ChatGPTs version of above

A new project kicks off. Requirements are clear, stakeholders are fired up, and the team is stacked. Everyone’s aligned, motivated, and quietly eyeing a promotion.

Someone runs npx your-framework-here, and it’s heads down for the next two years.

The app grows. Features ship. Demos impress. Management takes notice—and decides to spin up a second team to build on top of the success. After all, why not reuse the app as the foundation for other products?

Fast forward. You look up and realize you’re no longer a tight-knit team of five. You’re 30+ developers spread across multiple teams, each focused on its own kinda related domain. And you’re all still working in the same codebase.

So…
What went wrong?

## Your success is your problem

The system, as it stands, no longer holds up. 

All the technical debt accumulated during the first phase of the project has slowed the rate of change.

The good news is, you didn't do anything wrong! This is just how software is built

You did the best you could with the context you had, you didn't know what you didn't know.

Well hang on shouldn't you have designed the system to support some of these features?

Until your product sustains itself, the long term doesn't matter - Kent Beck

Management was right to have other teams reuse the application for new projects. Starting
from scratch for every new project is a waste. 

The problem was the application didn't have the structure to support multiple teams.

Your project may be rich with features but it lacks structure.

## ChatGPTs version of above

The system, as it stands, no longer holds up.

Technical debt accumulated during the early phase is now slowing the rate of change. Velocity drops. Bugs creep in. Every modification feels riskier than the last.

But here’s the good news: you didn’t do anything wrong.
This is just how software evolves.

You made the best decisions you could with the context you had. You didn’t know what you didn’t know. And that’s okay.

    “Until your product sustains itself, the long term doesn’t matter.”
    — Kent Beck

Could you have designed the system with more flexibility? Maybe. But early on, durability and extensibility take a backseat to speed and validation. You needed to ship, learn, and iterate.

And management wasn’t wrong, either—reusing the application for new projects made sense. Starting from scratch every time is expensive and wasteful.

The real problem?
The application lacked the structure to support multiple teams, multiple domains, and evolving priorities.

Your project may be feature-rich—but without clear boundaries, modularity, or separation of concerns, it becomes fragile under the weight of its own success.

## Structure vs feature development

There are two modes of development - you're either building features or building structure to support future features.

We build features to add immediate value to the application.

We invest in structure development to support future development. 


The cost of software is the cost of change - Johnny Osetimheimer

## How can Monorepos help?


## When do Monorepos make sense

I can't think of a time where using a monorepo is a bad thing. Should you 
use a monorepo for your little side project? Why not? A monorepo with a single
app could be the start of something great.

Is it worth it though it that case, probably not. If your anything like me your side
project won't even make it to your personal GitHub.

Where monorepos really shine in the following case

Monorepos enable you to support multiple applications in the same repository. A good 
monorepo tool will support the following features

- Commands to manage serving and deploy each application
- 

## Benefits of a Monorepo

A tool to enable decoupled applications. Supports managing and building each application independently.

- Independent Deploys
- 


## The we'll do it right

Talk about the pitfalls of poly repos in practice.

## Make this a better title

Have you ever experienced something like the above? 

Talk about why this happens

- Too focused on building features not on the structure of the application

The good news factory

It's the classic problem that shows up all over software development **tight coupling** 

It's kinda like vertically scaling a server, at some point you can't add anymore resources and
you need to scale horizontally.

Enter the **monorepo**

## A new way to structure applications


## This sounds a lot like micro services

I know what you're thinking, shouldn't you 


## What about workspaces

## What about publishing packages?

Why not publish a package and use it in polyrepo. You could but in practice it's much 
harder to know if changes will effect teams.



## Developer experience and local development

## Structure vs Feature development

There are two ways to value a codebase, the immediate and long term.

The immediate value is the summation of all your current features. Your customers and what they're willing to pay for those features.

Now, if this were most other industries you'd be satisfied with immediate value. 

By the time most products are purchased they're features were finalized long before. They've been tested, packaged and delivered. 
They're done, the only thing left is to manage the profits.

This isn't how software products are built, at least not today. In the modern age, it's all about getting to your customers quickly, hooking them
in with an interesting concept and getting them excited about the future of the product.

When software is a service, it's not a product. A product has an endpoint. Software is never finished.

The future of the product is the product.

How difficult would it be to add a new feature, a new application to the current codebase. 
Could your codebase even support another feature?