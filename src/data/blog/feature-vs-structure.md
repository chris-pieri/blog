---
title: Features vs Structure
author: Chris Pieri
pubDatetime: 2025-08-13T07:00:00.000Z
featured: false
draft: true
tags:
  - software design
description: Read this one because I told you so
---

## Table of contents

A great lead
Mystery
Discovery
Little bits at time
End quickly
Clear, concise, simple

## Mission Statement

Delivering features requires design tradeoffs.

Tradeoffs add technical debt to a system.

Developer productivity decreases as technical debts increase.

Refactoring structure pays down technical debt.

Business and developers are not aligned when it comes to technical debt. 

How can we work together to fix this situation.

## Lead

Choosing between new features and improving the structure of a system can feel like a game of tug of war. 
On one side you have your customers. They don't know what structure development means. All they want are new features, bugs fixed, and <add something specific>. On the other side are the developers. What's interesting is they want most of the same things but they can't get to them because the system has become to complicated.

There needs to be balance. But when should you prioritize structure? How do you convince the business? And what techniques will simplify the complex system? 

But first how did we get here. We know the answer is technical debt but that has become a loaded term. Let's try to make it more concrete.

## Revisiting technical debt

Technical debt is abstract concept that over the years has become overloaded to mean anything from messy code to full rewrites.

To make it more concrete we'll start at the beginning.

The term Technical Debt was created by Ward Cunningham to describe the engineering trade-off’s that software developers and business stakeholders must often make to meet schedules and customer expectations. In short, you may need to use suboptimal designs in the short term, because the schedule does not allow longer term designs to be used.

These are deliberate design tradeoffs the team needs to make. 

At the start of a project you don't have time to develop all the techniques of robust system. Continuous delivery, full test suite, etc.
Instead your concern is a minimally viable product. Just enough to know if the idea is something people would use.

This is in contrast to a popular use of the term - messy code.

Messy code is not technical debt. A mess is just a mess. Technical debt decisions are made based on real project constraints. They are risky, but they can be beneficial. The decision to make a mess is never rational, is always based on laziness and unprofessionalism, and has no chance of paying off in the future. A mess is always a loss.

This is not to say messy code should not be refactored - it should - but it should not warrant its own story.

### What does it look like

It can take make forms. But the biggest offender is coupling.

Lack of robustness, scalability.

### Why does it occur

The pressure to deliver. Changing requirements.

### Dangers of technical debt

Technical debt limits productivity. And that's stressful. Its stressful for the developers, the customers, and the business. 

Developers are forced to figure out how to make sushi in a McDonald's.

That's stressful, a smart developer will realize the situation and attempt to fix that. But often will be denied the opportunity
so the best thing to do in that case is leave.

increases complexity
makes it harder to predict release schedules
By increasing the cost of ongoing maintenance, technical debt makes it harder to predict release schedules. Increases in complexity make it increasingly difficult to accurately estimate effort, resulting in delays, missed deadlines, and stress on engineering teams, which can result in higher staff turnover, compounding the problem.[16] Carrying technical debt into production increases the risk of outages, financial losses, and potential legal issues due to breached service-level agreements. Future refactoring becomes riskier and costlier, with modifications to production code introducing greater chances of disruption.[citation needed]

Failure to address technical debt can cause productivity to decline and slow down the delivery of features. The cumulative effects of technical debt result in increasingly fragile systems that can make bold improvements difficult. The domination of incremental changes, along with delays to critical refactoring, can result in stressed systems with inconsistent design, causing users to suffer from degraded performance and limited functionality while developers struggle to maintain quality.[1][17] 

### How to fix it

Invest in continual design, not just upfront. Refactor. 

## Current understanding of Refactoring

We already have a name for structure development it's called Refactoring. But the general sense of refactoring - at least in my experience -
is more like house keeping. Pruning the edges of the system. Adding a little speed here and upgrading a dependency there, make this a little more readable. It fails to capture the essence of what we're trying to accomplish.

We want to enhance overall feature development. We want to speed up and be confident our changes will work. To do that we'll need some major changes. We're no longer pulling weeds in the garden. We're swapping the engine while the plane is in the air.

The only way they'll see it that way is if we can convince them. But how do you get them interested in something that usually only happens when there is literally nothing else to work on? You have to put it in there terms they'll understand. You need to talk money 💰

## How did we get here

A new software system starts like a McDonald’s—simple menu, specialized tools, fast delivery.
Then one day, someone asks for grilled cheese. You can do it, so you add it. Next comes fish tacos. Then pasta. Then sushi.

Soon your burger joint’s menu looks like a food court, but the kitchen is still built for burgers. Orders slow down, quality drops, and the staff is exhausted.

That’s what happens when you keep adding features without upgrading the underlying structure. At some point, you don’t need a new menu—you need a new kitchen.

---

Imagine you start a restaurant like McDonald’s.
The menu is simple. The equipment is purpose-built. Every process is optimized so you can serve millions of burgers quickly and consistently. Customers know exactly what to expect, and your kitchen hums like a well-oiled machine.

Then one day, a loyal customer asks, “Can you make a grilled cheese?”
Technically, yes—you have a grill. It’s not on the menu, but you approve the request and add it.

A few weeks later, someone asks for fish tacos. You figure, “We can make it work,” so you squeeze that in too. Then comes pasta, sushi, milkshakes. Each time, you adjust the menu and tweak your processes, telling yourself it’s just one more thing.

Months pass. Your burger joint now has a menu that looks more like a mall food court, but the kitchen is still running on the same burger-flipping equipment it started with. The grill now cooks fish and burgers—requiring extra cleaning between orders. The fryers handle onion rings and churros. Orders take longer, staff have to learn unfamiliar recipes, and new hires struggle to keep up.

Customers are confused. Some still want your famous burgers, but others expect you to excel at everything on the ever-growing menu. Meanwhile, your original efficiency is gone.

At this point, you face a choice: keep overloading your one kitchen, or spin off new specialized spaces—a sushi bar, a pasta place—each with the right tools, trained staff, and clear purpose.

## Let's talk money 

There are two ways to value a codebase, the immediate and long term.

The immediate value is the summation of all your current features, your customers and what they're willing to pay for those features.

Now, if this were most other industries you'd be satisfied with immediate value. 

By the time most products are purchased they're features were finalized long before. They've been tested, packaged and delivered. 
They're done, the only thing left is to manage the profits.

This isn't how software products are built, at least not today. In the modern age, it's all about getting to your customers quickly, hooking them in with an interesting *minimal viable product MVP* and getting them excited about the future of the product.

When software is a service, it's not a product. A product has an endpoint. Software is never finished.

Said another way, the future of the software is what matters.

How do you quantify the long term value of software?

You can roughly estimate the long term value of a particular software by understanding the cost of change. 
How difficult was it to add a minor feature, a new dashboard, a separate application? Could your current codebase
even support another application?

Depending where you are on the products journey and the decisions you prioritize, you'll have different answers to those questions.

## Proof of concept stage

Many early stage software teams find it easy to add new features. They're only bottleneck is the speed at which they type. This is justifiable because they have no customers or only a few early adopters. You can't break something nobody is using. Their focus is features and structure is an afterthought.

## Startup stage

Middle stage products begin to see technical debt accumulated during the early phase is now slowing the rate of change. Velocity drops. Bugs creep in. Every modification feels riskier than the last. Then of course is the matter of cognitive load. The few early developers can no longer manage the complexity of the whole system. You'll need to divide the system into domains and assign teams to manage each. Now you **need** a system that supports multiple applications.

Structure has entered the chat. 

The question is when do you prioritize structure?

Anyone who doesn't write the code will not understand why structure matters. It is your job to explain the cost of a poorly structured codebase.

What do you prioritize features or structure? You'll have different answers at different times.

There is a point - I don't know when - where prioritizing structure will benefit you in ways purely focusing on features won't.

## Thoughts

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



## Structure vs Feature development

There are two ways to value a codebase, the immediate and long term.

The immediate value is the summation of all your current features, your customers and what they're willing to pay for those features.

Now, if this were most other industries you'd be satisfied with immediate value. 

By the time most products are purchased they're features were finalized long before. They've been tested, packaged and delivered. 
They're done, the only thing left is to manage the profits.

This isn't how software products are built, at least not today. In the modern age, it's all about getting to your customers quickly, hooking them in with an interesting *minimal viable product MVP* and getting them excited about the future of the product.

When software is a service, it's not a product. A product has an endpoint. Software is never finished.

Said another way, the future of the software is what matters.

How do you quantify the long term value of software?

You can roughly estimate the long term value of a particular software by understanding the cost of change. 
How difficult was it to add a minor feature, a new dashboard, a separate application? Could your current codebase
even support another application?

Depending where you are on the products journey and the decisions you prioritize, you'll have different answers to those questions.

## Proof of concept stage

Many early stage software teams find it easy to add new features. They're only bottleneck is the speed at which they type. This is justifiable because they have no customers or only a few early adopters. You can't break something nobody is using. Their focus is features and structure is an afterthought.

## Startup stage

Middle stage products begin to see technical debt accumulated during the early phase is now slowing the rate of change. Velocity drops. Bugs creep in. Every modification feels riskier than the last. Then of course is the matter of cognitive load. The few early developers can no longer manage the complexity of the whole system. You'll need to divide the system into domains and assign teams to manage each. Now you **need** a system that supports multiple applications.

Structure has entered the chat. 

The question is when do you prioritize structure?

Anyone who doesn't write the code will not understand why structure matters. It is your job to explain the cost of a poorly structured codebase.

What do you prioritize features or structure? You'll have different answers at different times.

There is a point - I don't know when - where prioritizing structure will benefit you in ways purely focusing on features won't.


## Technical Debt

### What is it

The term Technical Debt was created by Ward Cunningham to describe the engineering trade-off’s that software developers and business stakeholders must often make in order to meet schedules and customer expectations. In short, you may need to use suboptimal designs in the short term, because the schedule does not allow longer term designs to be used

A mess is not a technical debt. A mess is just a mess. Technical debt decisions are made based on real project constraints. They are risky, but they can be beneficial. The decision to make a mess is never rational, is always based on laziness and unprofessionalism, and has no chance of paying off in the future. A mess is always a loss.

### What does it look like

It can take make forms. But the biggest offender is coupling.

Lack of robustness, scalability.

### Why does it occur

The pressure to deliver. Changing requirements.

### Dangers of technical debt

Technical debt limits productivity and that's stressful. Its stressful for the developers, the customers, and the business. 

Developers are forced to figure out how to make sushi in a McDonald's.

That's stressful, a smart developer will realize the situation and attempt to fix that. But often will be denied the opportunity
so the best thing to do in that case is leave.

increases complexity
makes it harder to predict release schedules
By increasing the cost of ongoing maintenance, technical debt makes it harder to predict release schedules. Increases in complexity make it increasingly difficult to accurately estimate effort, resulting in delays, missed deadlines, and stress on engineering teams, which can result in higher staff turnover, compounding the problem.[16] Carrying technical debt into production increases the risk of outages, financial losses, and potential legal issues due to breached service-level agreements. Future refactoring becomes riskier and costlier, with modifications to production code introducing greater chances of disruption.[citation needed]

Failure to address technical debt can cause productivity to decline and slow down the delivery of features. The cumulative effects of technical debt result in increasingly fragile systems that can make bold improvements difficult. The domination of incremental changes, along with delays to critical refactoring, can result in stressed systems with inconsistent design, causing users to suffer from degraded performance and limited functionality while developers struggle to maintain quality.[1][17] 

### How to fix it

Invest in continual design, not just upfront. Refactor. 


## The cost of software

People have said the cost of software is the cost of change

What does that mean?

Kent Beck explains it as coupling makes change difficult. The more coupled your software is the more things that need to change
to add functionality. Little by little this adds up to the point where a big change feels like an avalanche. Change at that point is 
very slow which drives up the cost.

This is definitely true. But I don't think its the whole picture. That's assuming you first understand the change and second have 
permission to make the change.

Theres another way coupling can affect cost: communication and coordination

The product owner is the gatekeeper of all the knowledge and the developers are just code monkeys.

A separate team owns the service that needs to change. You need to communicate, coordinate and schedule changes with that team.

An in-house built service lacks documentation. You must work with the creator, if they're still around, to understand it or read the code.

Red tape. Every company has some form of red tape - usually due to lack of trust - their may me memos you need to write first or 
change tickets you need to fill out. This can really slow things down.

Missing permissions.

Code reviews and approvals.

The cost of these changes add up not like an avalanche but more like a mountain that needs to be climbed before you can make a change.

