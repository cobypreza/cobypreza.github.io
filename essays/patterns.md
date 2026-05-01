---
layout: essay
type: essay
title: "From Bus Stops To Code Blocks"
# All dates must be YYYY-MM-DD format!
date: 2026-04-30
published: true
labels:
  - Software Engineering
  - Design Patterns
---

<img width="300px" img height = "450px" class="rounded float-start pe-4" src="../img/busroute.png">

## Finding Patterns
Let’s say you take the bus to work every day. It is a fixed route that reliably gets you to your workplace, one that you have already tested and found to be efficient. Now, suppose a new cafe opens near your workplace. For the sake of this example, you really like coffee and you want to try out this new place. You don’t have to completely redesign your commute, rather you might consider a few options based off of your reliable, tested route. For example, you may get off a stop earlier, transfer to another bus for a slightly different stop, or choose an alternative route that gets you to roughly the same area. In this context, you are using a design pattern. The problem here is finding an efficient route to reach locations in the general area. Rather than designing a completely new solution, we are reusing a proven route and making small adjustments to meet a slightly different goal.


## Pick Your Pattern
One of the patterns we go over is the Singleton. Using it with the example bus, it is as if there is only one main bus terminal that everyone depends on. A Singleton is where only one instance exists. Using a Singleton makes it easier to control the access and behavior of a class. Though using a Singleton is usually not thread-safe and having a global state is often unwise while software engineering.

Another pattern we go over are Factories. This is like requesting a bus and being given a bus of the right type (e.g., double-decker, electric). A Factory is where you create objects without the exposure of underlying logic. Using a factory allows for an easier way to add additional object types. A consequence of using a Factory is that they can be more complicated than object oriented class constructors.

In ICS 314, we also go over observers. Using the example again: a commuter has an app that notifies all commuters when a bus is going to arrive by the minute. An Observer is a pattern used for when a set of objects (the Observers) are to be informed whenever a change in state happens to another object (the Subject). This pattern can be great but poor implementations can lead to performance issues. They may also be harder to reason and to debug.

Finally, we go over Model-View-Controllers (MVC). You decide you want to go to the cafe (Controller), so the system checks the routes and stops (Model), finally the system shows you your updated options (View). For MVCs we are decoupling the internal representation information from how it is presented to how it is accepted by the user. MVCs may be harder to implement as they tend to be more complex than some of the other patterns we described earlier.


## Routing Smarter
Though I may not have heard about design patterns beforehand, a lot of Computer Science is recognizing patterns and adjusting it ever-so-slightly. For our final project we are making a website that helps hoopers around the island find new courts to play at and teammates to play with. On our current final project, we used the Factory pattern where we can create new objects through a function, or in our case our API. We also use the Observer pattern where other users are updated when another user joins a court. The Observer pattern can also be found in our “Looking For Team” page as it updates other users when another court is created. We also display an MVC pattern. We store the information of the courts, users, and teams in our Prisma schema. Then we may view all this information through our UI using React. Finally, we have our API routes as the controller to make sure that everything is functioning the way it’s supposed to. To conclude, even though I may have not given design patterns as much thought in the past, I have always used them subconsciously.
