## Архитектура

Пожалуйста, постарайтесь не заучивать архитектурные принципы наизусть, это не бессмертные стихи Александра «Наше Всё» Пушкина. Никому еще не прибавляло ума бубнение о том, что «Принцип подстановки Барбары Лисков означает, что если S является подтипом T, тогда объекты типа T в программе могут быть...».  
Просто попробуйте приложить тот же LSP к программе, которую пишете. Что вам даст соблюдение этого принципа? Какие проблемы последуют за его несоблюдением? Какую цену придётся заплатить за его имплементацию и поддержку?

Попробуйте поиграться с функциональной парадигмой. Применение функционального подхода и его практическое использование вполне возможно не только в Haskell или F#, но и в Python, причём совершенно не обязательно делать это только в рамках functools.

Разберитесь, что стоит за просьбой интервьюера «Сказать три главных слова» (если что, это не «я тебя люблю», а «наследование, инкапсуляция, полиморфизм») и почему следует дополнить эту триаду понятием «уровень абстракции».

Попробуйте понять, с какими конкретными, осязаемыми проблемами старых парадигм столкнулись разработчики Agile или популяризаторы микросервисной архитектуры. Разберитесь, чем плох main(), который вызывает все остальные процедуры, ведь в эмбеддед программировании это распространенная практика. Взвесьте цену дополнительных слоёв абстракции, наворачиваемых между корневой бизнес-логикой и внешним миром.

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
