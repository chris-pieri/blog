---
title: Monorepos-2
author: Chris Pieri
pubDatetime: 2025-08-01T07:00:00.000Z
slug: monorepos
featured: false
draft: true
tags:
  - monorepo
description: The only thing that will save your job from the AI
---

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