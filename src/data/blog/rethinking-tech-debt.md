---
title: Reframing Tech Debt
author: Chris Pieri
pubDatetime: 2025-08-21T01:00:00.000Z
featured: false
draft: false
slug: reframing-tech-debt
tags:
  - software design
  - tech debt
description: Can the way we talk about tech debt have an affect on the success of the product?
---

The first principle of the Agile Manifesto is:

> Our highest priority is to satisfy the customer through early and continuous delivery of valuable software

In practical terms, this means developers and business stakeholders deliberately make design tradeoffs to release the product early. Developers implement just enough design to produce a minimally viable product (MVP) - trading robust architecture for speed to market.

After the MVP launches, teams gather user feedback and add features while adapting to changing requirements. Initially, the MVP design suffices, but as the product grows, those design tradeoffs inevitably catch up, and growth slows. 

## Growing pains

Consider the familiar challenges of a scaling team:

- **No clear boundaries** - Developers work across tangled domains. Work can't be divided because the architecture doesn't support independent teams. This overlap increases cognitive load and creates communication overhead.

- **Infrequent deployments** - Large merge conflicts, poor test coverage, missing CI/CD, all delay deployments - and thus customer feedback.

- **Code duplication** - Without reusable modules, teams do redundant work and produce inconsistent results.

Developers feel these pains first and must communicate the issues to business stakeholders. This is where things get tricky.

## The tech debt trap

Often developers will express theses issues with the familiar but overloaded term "tech debt". And often we fail to get our point across. To be fair though, fixing tech debt is hard to advocate for. It's not feature development, customers will never see it, and it feels like acknowledging failure. You can almost hear stakeholders say "Well if the devs just got it right the first time, we wouldn't be in this mess".

But before you start spewing a bunch of technical jargon, remind yourself the business and developers **together** made design tradeoffs to release the product early. This tech debt is a byproduct of Agile Development, not a failure of software development. Agile got us in this mess, and it will get us out because agile is cyclical - just enough design then feature development and repeat. We just went through one phase, the next step is to improve the current design. 

## A new lense

When you view tech debt this way you'll realize a few things. 

- **It's unavoidable** - A natural consequence of Agile Development

- **It's the inverse of design** - Investing in design decreases tech debt

- **It's actually a sign of success** - You only feel tech debt's pain if the product has grown

But also realize, this is a pivotal point in the lifetime of the product. You need to get business to invest in design. Otherwise, this will be your first - and last - trip around agile wheel. That's why we need to be strategic when talking tech debt to the business.

## Convincing to the biz

When talking to the biz, don't talk about how the messy code is hard to change, instead frame it as an **investment in optionality**.

Kent Beck explains this concept in his book "The Good News Factory":

> “The trickiest yet potentially most significant economic driver of software products is optionality. How many different features can you implement next? It’s like keeping multiple doors open, not knowing which one will lead to the treasure room. Software design keeps those doors propped open.
>
> A codebase riddled with quick fixes and technical debt reduces optionality.”

Optionality means the ability to pivot. To pursue multiple opportunities. To reduce risk in an uncertain future. Software design and technical debt are at the core of this concept.

## The bottom line

Addressing technical debt isn't about cleaning up a mess, it's about investing in your product's future. Features drive today's revenue. Design drives tomorrow's options. Without both, growth stalls.

Frame technical debt as an investment in optionality, and you'll capture stakeholder's attention while securing the resources needed for sustainable growth.