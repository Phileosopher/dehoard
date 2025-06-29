
When making software on a website, make it as easy and quick as possible for the new leads to poke around with it
if people get to "test drive" it, they can feel what the product is capable of

Programming languages are what programmers think in.

## Code

Code is a liability, not an asset. Aim to have as little of it as possible.

Build programs out of pure functions. This saves you from spending your brain power on tracking side effects, mutated state and actions at a distance.

Use a programming language with a rich type system that lets you describe the parts of your code and checks your program at compile time.

The expressivity of a programming language matters hugely. It’s not just a convenience to save keypresses, it directly influences the way in which you write code.

Choose a programming language that has a good module system, and use it. Be explicit about the public interface of a module, and ensure its interals don't leak out to client code.

Code is a living construct that is never “done”. You need to tend it like a garden, always improving and tidying it, or it withers and dies.

Have the same high standards for all the code you write, from little scripts to the inner loop of your critical system.

Write code that is exception safe and resource safe, always, even in contexts where you think it won’t matter. The code you wrote in a little ad-hoc script will inevitably find its way into more critical or long-running code.

Use the same language for the little tools and scripts in your system too. There are few good reasons to drop down into bash or Python scripts, and some considerable disadvantages.

In code, even the smallest details matter. This includes whitespace and layout!


## Design

Modelling - the act of creating models of the world - is a crucial skill, and one that’s been undervalued in recent years.

Model your domain using types.

Model your domain first, using data types and function signatures, pick implementation technologies and physical architecture later.

Implement functionality in vertical slices that span your whole system, and iterate to grow the system.

Resist the temptation to use your main domain types to describe interfaces or messages exchanged by your system. Use separate types for these, even if it entails some duplication, as these types will evolve differently over time.

Prefer immutability always. This applies to data storage as well as in-memory data structures.

When building programs that perform actions, model the actions as data, then write an interpreter that performs them. This makes your code much easier to test, monitor, debug, and refactor.

Dependency management is crucial, so do it from day one. The payoff for this mostly comes when your system is bigger, but it’s not expensive to do from the beginning and it saves massive problems later.

Avoid circular dependencies, always.


## Quality

I don’t care if you write the tests first, last, or in the middle, but all code must have good tests.

Tests should be performed at different levels of the system. Don’t get hung up on what these different levels of tests are called.

Absolutely all tests should be automated.

Test code should be written and maintained as carefully as production code.

Developers should write the tests.

Run tests on the production system too, to check it’s doing the right thing.


## Designing systems

A better system is often a smaller, simpler system.

To design healthy systems, divide and conquer. Split the problem into smaller parts.

Divide and conquer works recursively: divide the system into a hierarchy of simpler sub-systems and components.
	
_Corollary: When designing a system, there are more choices than a monolith vs. a thousand “microservices”._

The interface between parts is crucial. Aim for interfaces that are as small and simple as possible.

Data dependencies are insidious. Take particular care to manage the coupling introduced by such dependencies.

Plan to evolve data definitions over time, as they will inevitably change.

Asynchronous interfaces can be useful to remove temporal coupling between parts.

Every inter-process boundary incurs a great cost, losing type safety, and making it much harder to reason about failures. Only introduce such boundaries where absolutely necessary and where the benefits outweigh the cost.

Being able to tell what your system is doing is crucial, so make sure it’s observable.

Telling what your system has done in the past is even more crucial, so make sure it’s auditable.

A modern programming language is the most expressive tool we have for describing all aspects of a system.

This means: write configuration as code, unless it absolutely, definitely has to change at runtime.

Also, write the specification of the system as executable code.

And, use code to describe the infrastructure of your system, in the same language as the rest of the code. Write code that interprets the description of your system to provision actual physical infrastructure.

At the risk of repeating myself: everything is code.

_Corollary: if you’re writing JSON or YAML by hand, you’re doing it wrong. These are formats for the machines, not for humans to produce and consume. (Don’t despair though: most people do this, I do too, so you’re not alone! Let's just try to aim for something better)._

The physical manifestation of your system (e.g. choices of storage, messaging, RPC technology, packaging and scheduling etc) should usually be an implementation detail, not the main aspect of the system that the rest is built around.

It should be easy to change the underlying technologies (e.g. for data storage, messaging, execution environment) used by a component in your system, this should not affect large parts of your code base.

You should have at least two physical manifestations of your system: a fully integrated in-memory one for testing, and the real physical deployment. They should be functionally equivalent.

You should be able to run a local version of your system on a developer’s computer with a single command. With the capacity of modern computers, there is absolutely no rational reason why this isn’t feasible, even for big, complex systems.

There is a running theme here: separate the description of _what_ a system does from _how_ it does it. This is probably the single most important consideration when creating a system.


## Building systems

For a new system, get a walking skeleton deployed to production as soon as possible.

Your master branch should always be deployable to production.

Use feature branches if you like. Modern version control tools make merging easy enough that it’s not a problem to let these be long-lived in some cases.

Ideally, deploy automatically to production on every update to master. If that’s not feasible, it should be a one-click action to perform the deployment.

Maintain a separate environment for situations when you find it useful to test code separately from production. Avoid more than one such extra environment, as this introduces overheads and cost.

Prefer feature flags and similar mechanisms to control what's enabled in production over separate test/staging environments and manual promotion of releases.

Get in the habit of deploying from master to production from the very beginning of a project. Doing this shapes both your system and how you work with it for the better.

In fact, follow all these practices from the very beginning of a new system. Retrofitting them later is much, much harder.


## Technology

Beware of hyped or fashionable technologies. The fundamentals of computer science and engineering don’t change much over time.

Keep up with latest developments in technology to see how they can help you, but be realistic about what they can do.

Choose your data storage backend according to the shape of data, types of queries needed, patterns of writes vs. reads, performance requirements, and more. Every use case is different.

That said, PostgreSQL should be your default and you should only pick something else if you have a good reason.
