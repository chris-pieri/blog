---
title: The case for technical excellence
author: Chris Pieri
pubDatetime: 2025-08-01T07:00:00.000Z
slug: monorepos
featured: false
draft: true
tags:
  - monorepo
description: How to align developers and business to build more agile software
---

The more developers and the business - people with the money - align the better the software.
Communicating, however, is difficult and the terms we use are overloaded. What do we mean by software design, technical debt and Agile? If we are not clear the business can't prioritize, and the system will suffer from diminishing developer productivity.

Both sides want the same thing — valuable software that keeps delivering — but misaligned language often leads to stalled projects, frustrated teams, and wasted money.

Why is it so hard to get time to refactor technical debt?

We, as developers, know techniques to improve the design of software - microservices, monorepos, feature flags, and observability to name a few. So, why is it so hard to convince the business to let us add these.

Part of it may be the terms we use.

Let's start with Agile.


## Agile

The first principle of the Agile Manifesto is:

> Our highest priority is to satisfy the customer through early and continuous delivery of valuable software

This is in contrast to the traditional waterfall approach where a large up front design is prioritized. This has drawbacks because the beginning of a project is when we know the least about our requirements. And requirements will change which means we are usually wrong about our assumptions. Throughout the lifetime of a project we often need to pivot.

Agile's antidote - the minimally viable product - just enough design to prove the worth of our idea. Over time the system evolves to meet new requirements. A simple way of expressing this is instead of building a ferrari start with a scooter. This will derisk the system.

In short, we deliberately make a set of design tradeoffs to release the product sooner rather than later. 

If you are doing this your practicing agile, but this comes with consequences. A familiar foe appears - tech debt.

We have a name for this, though it may not be how you use it, its called technical debt.

## Not your dad's technical debt

Technical Debt is a term used to explain decreasing developer productivity. 
As developers, we experience it in our day to day work. We've come to expect it but what is frustrating is we rarely get opportunities to fix it.

But the real cost isn't just slower releases - it's **missed opportunities**.

As a product grows, you need more developers. More developers require independent teams. Independent teams require independent releases. But most minimally viable products aren’t designed to support that.

Technical debt doesn’t just make development harder — it stalls product growth.

And because debt is invisible to the business, it’s on developers to explain it in business terms: not as “ugly code” or “refactoring,” but as the difference between a product that can evolve and one that gets left behind.

If you express technical debt this way you'll get the business's attention.


the design trade-off’s that software developers and business stakeholders must often make in order to meet schedules and customer expectations. 

In other words, you may need to use suboptimal designs in the short term, because the schedule does not allow longer term designs to be used.

Technical debt can accumulate "interest" over time, making future changes more difficult and costly.

What's interesting about tech debt is that its invisible to the business. Only the developers know about it. So it is the developers responsibility to express this to the business. How can we effectively communicate to someone who's not an active contributor? We need to be concrete when we refer to software design.

## Software Design

At its core, software design is about shaping the software so that it’s easier to change in the future. It's the opposite of technical debt and will allow us to react to rapidly changing requirements - a quality of good agile software. 


“Software design”, however, can mean anything from variable naming and code comments to infrastructure, deployment pipelines, and architecture.

`IMAGE OF SOFTWARE DESIGN TERMS`

As it currently stands, it is difficult understand the relationship of the terms. So, I will reorganize them to fall within to categories - System Design and Code Design.


Good design gives us options. Poor design locks us in.

## The tech debt line

Here I'm proposing a way to think about tech debt within software design. We need to know what to include and what to leave out.

<!-- ![The tech debt line](../../assets/images/software-design-line.svg) -->
*The tech debt line*

Everything above the tech debt line is fair game. If you express these concerns the business should give you the time to refactor. 

Everything below the line is too discrete for the business to understand. It is best to fix this tech debt during normal feature development. There are many techniques for this. Look into Tidy First? by Kent Beck and Refactoring by Martin Fowler for methods to pay down this tech debt.

## Summary

We can't be agile without technical debt. For a software system to evolve we need to pay down technical debt. This requires alignment between software developers and the business. We need to communicate in concrete terms. Express investing in software design as a way to introduce options to your system. 

## The restaurant biz

John makes the best burger. 

Everyone that's tried one says "You should sell these!". Finally he thinks maybe I could sell them.

John doesn’t have much money, and he's not ready to bet the farm. So, he rents a kitchen at night and sell burgers out the back door. He only has the essentials — a grill, fridge, and sink — just enough to prove people will pay for his burgers.

The grand opening surprises John. People love the burgers and for a while he has success.

Soon he realizes he has a problem.

The excitement fades. Sales slow down. Eventually everyone who wants his burger has already had one.

Well that's fine he have a grill and fridge he'll just come up with a killer recipe that will attract a whole new kind of customer. A few experiments later, grilled cheeses are on the menu. New customers arrive, and sales climb again.

John is pleased with the outcome. He now spends all his time coming up with new recipes and adding them to the menu. Each new item brings more customers. Soon the menu includes salads, fish tacos, vegan options and more.

Then, a new problem appears.

He can’t keep up with orders. Efficiency plummets. The cooks are overwhelmed juggling so many recipes. Customers get frustrated, dishes pile up, and the kitchen is constantly in chaos. Some cooks even quit because they feel "burnt out". One customer complains about a bug in the food.

John goes to complain to his cooks and as soon as he gets trough the door he realize the problem — it’s the kitchen.

The equipment was sufficient when only were made burgers, but now it’s straining under the weight of a full menu. The workflow is messy. Ingredients are stored in awkward places. No one knows the fastest way to move from the fridge to the grill to the prep station.

So John decides to invest in the kitchen itself.

He reorganizes the layout so everything flows better. He adds specialized stations for burgers, salads, and grilled cheese. He upgrades the dishwasher so cooks spend more time cooking and less time cleaning. He removes a few unpopular menu items to reduce complexity.

It’s not flashy. Customers don’t see most of the changes. But inside the kitchen, everything feels different — faster, smoother, and more reliable. Orders go out on time. Cooks have energy again. The restaurant is ready for the next big thing.

## Attempt

The term Technical Debt was created by Ward Cunningham to describe the engineering trade-off’s that software developers and business stakeholders must often make in order to meet schedules and customer expectations. In short, you may need to use suboptimal designs in the short term, because the schedule does not allow longer term designs to be used.

Technical debt can accumulate "interest" over time, making future changes more difficult and costly.

Notice we didn't mention anything about messy code. A mess is not technical debt. A mess is just a mess. You'll rarely get business to agree to invest in refactoring a mess. Therefore, it is your responsibility to fix the messes as part of your regular scheduled stories.

So the thing that is constraining the system is the design.

<!-- ![Estimating story points](../../assets/images/software-design-line.svg) -->
*How it feels to estimate story points*

With a little bit of luck though, you might convince business to invest in restructuring the design. But you'll need to put it in terms they can understand.

Technical debt decisions are made based on real project constraints. They are risky, but they can be beneficial. The decision to make a mess is never rational, is always based on laziness and unprofessionalism, and has no chance of paying off in the future. A mess is always a loss.

## Back to the world of software.

The software industry is similar to the restaurant industry. 

John is the product owner and the cooks are the developers. The kitchen is the software design.

The product owner starts with an idea. The lean movement taught us the idea is worth nothing until we have paying customers. So, the developers get to work designing and building a solution that satisfies a minimally viable product. 

In other words, we deliberately make a set of tradeoffs to release the product sooner rather than later.

With any luck we have success in the form of dollars.

We enter a new phase of development and this is all about building out features to acquire more customers

Until eventually our speedy productivity turns into a slow churn.

So far this sounds a lot like John's restaurant business. Where the analogy breaks down, however, is in the **ability see the constraints**. 

Everyone has an idea of how long a burger should take, so when it takes longer you know something must be wrong. One glimpse at a messy kitchen and you realize your issue. 

Software is not as straight-forward. 

With software the product owner can't see the kitchen; only developers can.

The constraints are only visible to the developers.

On the one hand, estimating work is difficult. We're almost always wrong and we've learned to accept that.

One does not simply walk into software. The constraints are only visible to the developers.

In contrast, how long does it take to implement a feature such as adding filters to a table? 3 story points? 4 err I mean 5? What even is a story point? The truth is it depends. 

There's often hidden constraints and usually we won't know know about it until we're half way through a solution.

![Estimating story points](https://media0.giphy.com/media/v1.Y2lkPTc5MGI3NjExbHMzeDB2aTQzeGQ2MWwyNGplcXRzbDhnNTZyZ3d2YXRkM3I0cmdhOSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/jEM13mezJQAtdGSKeI/giphy.gif)
*How it feels to estimate story points*

Estimating feature development is tough to get right, so when we're wrong it often doesn't sound off alarms.

The business is not aware of the design of the system and its constraints. It's a black box to them.

It is the developer's responsibility to express the constraints to the business. But how do you express it to someone who's not an active contributor? You might say something like, "we have technical debt we should refactor" and technically you'd be right. But the business doesn't understand that. Over the years tech debt has become such a loaded term its lost its respect. Now, the only time we're allowed to refactor is when there is nothing else to work on.

If we stand any chance in communicating the constraints we need to be concrete in our explanations.
For this reason, I think it's worth revisiting what we mean by technical debt. 

## Technical debt

The term Technical Debt was created by Ward Cunningham to describe the engineering trade-off’s that software developers and business stakeholders must often make in order to meet schedules and customer expectations. In short, you may need to use suboptimal designs in the short term, because the schedule does not allow longer term designs to be used.

Technical debt can accumulate "interest" over time, making future changes more difficult and costly.

Notice we didn't mention anything about messy code. A mess is not technical debt. A mess is just a mess. You'll rarely get business to agree to invest in refactoring a mess. Therefore, it is your responsibility to fix the messes as part of your regular scheduled stories.

So the thing that is constraining the system is the design.

<!-- ![Estimating story points](../../assets/images/software-design-line.svg) -->
*How it feels to estimate story points*

With a little bit of luck though, you might convince business to invest in restructuring the design. But you'll need to put it in terms they can understand.

Technical debt decisions are made based on real project constraints. They are risky, but they can be beneficial. The decision to make a mess is never rational, is always based on laziness and unprofessionalism, and has no chance of paying off in the future. A mess is always a loss.

## Expressing technical debt

There are two ways to value software: short and long term.

The immediate value is the summation of all your current features, your customers and what they're willing to pay for those features.

How do you quantify the long term value of software?

You can roughly estimate the long term value of a particular software by understanding the cost of change. 
How difficult was it to add a minor feature, a new dashboard, a separate application? Could your current codebase
even support another application?

Depending where you are on the products journey and the decisions you prioritize, you'll have different answers to those questions.

---

When we talk about the value of software, we usually mean the net present value. 

You can calculate this by 

But that's only half the equation. There's also the potential features you can build in the future.

Technical debt is the constraint. The current state of the system can only support

You can roughly calculate this by summing up the revenue from all the currently supported features. After all, that's what the customers are paying for. 

That's a good start but features are not free they incur a cost. The cost is how much time it takes to develop the features. A simple way to express this is:

`Software Value = ∑ feature(revenue - cost)`

So with that we see there are two ways to increase the value of software. Increase the revenue per feature and decrease the cost per feature.

Increasing the revenue per feature is a topic of its own and I'm not prepared to talk about it. But decreasing the cost to develop features is a concrete subject. There are techniques we can use to make changes easier. We can pay down technical debt, improve documentation and enhance the design of the software. Much like John at his restaurant we are investing in the kitchen. 

When we do this enough we realize a new value of software. It's no longer the immediate value of features. It's what can the software become.

With enough technical debt some features are too costly to implement. Reducing your feature options.

Add disclaimer - This is an oversimplification. In practice its more complicated but I feel this was a good way to explain the concept of long term value.

## Ways to improve long term value

Monorepos
Continuous Delivery