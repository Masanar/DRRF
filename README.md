

DRRF
----



We study the semantics of distributed reactive programming languages
using rewriting logic. We propose a reactive event-based programming
framework with explicit support for distribution, concurrency, and
explicit time manipulation *DRRF* which has been developed on *Maude*.


Model distributed systems using Maude is a straightforward task. They
are modeled as entities, loosely coupled by some suitable communication
mechanism. Maude provides a predefined module ` CONFIGURATION` that
declares sorts representing the essential concepts of object,
attributes, message, along with a notation for object syntax. A
configuration, base application, is a set of objects (Consumers &
Producers) and messages that represent a snapshot of a possible system
state. In this framework, the entities are objects, each with a unique
identity, and the communication mechanism is message passing using
broadcast or unicast protocols.

The framework uses rewriting logic and includes a model of the
distributed base application, a model of observables and observers, and
a model for complex predicate constructs supporting explicit time
manipulation.

Modules
-------


-   [`Base-Application.maude`](/blob/gh-pages/Discrete%20Time/Reactive-XD/Rules-Base-Application.maude):
    Specify the behavior of an environment where the observables issue
    data flow toward the system.
-   `Observers.maude`: Formal model for a distributed observer that
    watches the data flow issue by an observable.
-   `Temporal-logic.maude`: Formal model for LTL formulas.
-   `Predicates.maude`: Specify LTL predicates.
-   `Vector.maude`: Specify vector clocks using in the system.


Mateo Sanabria Ardila- Mateo.sanabria@escuelaing.edu.co
