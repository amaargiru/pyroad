## Architecture

Please try not to memorize architectural principles by heart; they are not Shakespeare's timeless poems. The rambling about how “Liskov's substitution principle means that if S is a subtype of T, then objects of type T in a program can be...” offers no advantage to anyone.
Just try applying the same LSP to the program you are writing. What benefit would compliance with this principle give you? What problems will result from not following it? What price will you have to pay for its implementation and support?

Try messing around with the functional paradigm. Applying the functional approach and using it in practice is possible not only in Haskell or F#, but also in Python, and it doesn't have to be done only within functools.

Figure out the reasoning behind the job interviewer's request to “say the three main words” (it's not “I love you”, by the way, it’s “inheritance, encapsulation, polymorphism”) and why this triad should be supplemented with the “abstraction”.

Try to understand what specific, tangible problems of the old paradigms the developers of Agile or the popularizers of microservice architecture faced. Figure out what's wrong with main(), which calls all the other procedures, since this is common practice in embedded programming. Weigh the cost of additional layers of abstraction between the root business logic and the outside world.

```mermaid
flowchart TD

subgraph Architecture
direction LR
WhatIsArch -.-> Principles -.-> Paradigms -.-> Object-oriented -.-> Design_Patterns -.-> Microservices -.-> System_Design -.-> Practices

WhatIsArch("What is?")
subgraph Principles
direction LR

subgraph SOLID
SRP(SRP)
OCP(OCP)
LSP(LSP)
ISP(ISP)
DIP(DIP)
end

coupling_vs_cohesion("Coupling vs cohesion")
KISS(KISS)
DRY(DRY)
YAGNI(YAGNI)

end

subgraph Paradigms
direction LR
Procedural(Procedural)
Structured(Structured)
parObject-oriented(Object-oriented)
Functional(Functional)
end

subgraph Object-oriented
direction LR
ooInheritance(Inheritance)
Encapsulation(Encapsulation)
Polymorphism(Polymorphism)
Abstraction(Abstraction)
end

subgraph Microservices
direction LR

Decentralization(Decentralization)
Smart_endpoints_dumb_pipes("Smart endpoints, dumb pipes")
Design_for_failure("Design for failure")

subgraph Messaging
direction LR
RabbitMQ(RabbitMQ)
Apache_Kafka("Apache Kafka")
end
end

subgraph Design_Patterns
direction LR

Observer(Observer)
Decorator_Method(Decorator)
Factory_Method("Factory Method")
Adapter_Facade("Adapter, Facade")

Creational_patterns("Creational patterns")
Structural_patterns("Structural patterns")
Behavioral_patterns("Behavioral patterns")
end

subgraph System_Design
direction LR
CQRS(CQRS)
Two_Phase_Commit("Two-Phase Commit")
Load_Balanced_Services("Load-Balanced Services")
Pattern_of_Distributed_Systems("Patterns of Distributed Systems")
Cloud_Design_Patterns("Cloud Design Patterns")
end

subgraph Practices
direction LR
Agile(Agile)
Scrum(Scrum)
Kanban(Kanban)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

class WhatIsArch trainee;
class SRP trainee;
class OCP trainee;
class LSP trainee;
class ISP trainee;
class DIP trainee;
class coupling_vs_cohesion trainee;
class Procedural trainee;
class parObject-oriented trainee;
class ooInheritance trainee;
class Encapsulation trainee;
class Polymorphism trainee;
class Abstraction trainee;
class Observer trainee;
class Decorator_Method trainee;
class Factory_Method trainee;
class Adapter_Facade trainee;
class Decentralization trainee;
class Smart_endpoints_dumb_pipes trainee;
class CQRS trainee;

class Functional middle;
class Creational_patterns middle;
class Structural_patterns middle;
class Behavioral_patterns middle;
class RabbitMQ middle;
class Apache_Kafka middle;
class Pattern_of_Distributed_Systems middle;
class Cloud_Design_Patterns middle;
class Scrum middle;
```
