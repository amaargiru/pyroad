## Развёртывание и администрирование

Несмотря на то, что темы «git» и особенно «Linux» весьма непросты и объемны, начало кривой обучения у них не очень крутое, поэтому я крайне рекомендую начать освоение DevOps с освоения git'а (хотя бы в объёме add-commit-push, так у вас останется неидеальная, но всё же история изменений) и Linux (в объёме PuTTY + WinSCP, например; скопируйте ваши Python-скрипты через SSH и запустите их на удалённой Linux-машине). На Stepik'е, например, есть прекрасные русскоязычные курсы, подробно объясняющие, кто на ком стоял, а уж сосчитать хорошие англоязычные мануалы по этим тематикам не хватит пальцев у самого распоясавшегося мутанта.  
Поверьте, Linux-консоль, выглядящая на первый взгляд такой непривычной и неудобной, покажется вам гораздо дружелюбнее, когда вы начнете изучать vim. Всё познается в сравнении!  

Что ж, здесь наша карта заканчивается. Попробуйте дойти до последнего зеленого раздела, GitHub Actions; прогоните, например, линтер для своего open source проекта (GitHub Actions бесплатен для проектов с открытым исходным кодом).  

```mermaid
flowchart TD

subgraph DevOps
direction LR
git -.-> Linux -.-> Development_lifecycle -.-> CI_CD -.-> Containers

subgraph git
direction LR
Basics(Basics)
Branching(Branching)
Tools(Tools)
GitHub(GitHub)
end

subgraph Linux
direction LR
Install(Install)
Directory_Structure("Directory Structure")
Terminal(Terminal)
Input_Output("Input/Output")
bash(bash)
System_administration("System administration")
Network_administration("Network administration")
end

subgraph Development_lifecycle
direction LR
Git_flow("Git-flow")
trunk_based_development("Trunk-based development")
end

subgraph CI_CD
direction LR
Continuous_testing("Continuous testing")
GitHub_Actions("GitHub Actions")
Jenkins(Jenkins)
New_Relic("New Relic")
end

subgraph Containers
direction LR
Docker(Docker)
Kubernetes(Kubernetes)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

class List trainee;
class tuple trainee;
class dict trainee;
class set trainee;
class array trainee;
class bytes trainee;
class deque trainee;
class heap trainee;
class range trainee;
class string trainee;
class datetime trainee;
class slice trainee;
class sort trainee;
class sorted trainee;
class listcomprehension trainee;
class bisect trainee;
class fmap trainee;
class ffilter trainee;
class freduce trainee;
class String_Built-in_Functions trainee;
class encode trainee;
class decode trainee;
class Read_Write trainee;
class Text_Binary trainee;
class JSON trainee;
class paths trainee;
class Data_Built-in_Functions trainee;
class icount trainee;
class icycle trainee;
class irepeat trainee;
class pairwise trainee;
class product trainee;
class combinations trainee;
class enumerate trainee;
class generator trainee;
class decorator trainee;
class context trainee;
class oopBase1 trainee;
class oop_property trainee;
class staticmethod trainee;
class classmethod trainee;
class slots trainee;
class Comparable trainee;
class Hashable trainee;
class Sortable trainee;
class Iterable trainee;
class Collection trainee;
class shallow trainee;
class deep trainee;
class objInheritance trainee;
class Multiple_Inheritance trainee;
class MRO trainee;
class reference_counting trainee;
class garbage_collector trainee;
class GIL trainee;
class args_kwargs trainee;
class lambda trainee;
class exception_handling trainee;
class built_in_exceptions trainee;
class exception_raising trainee;
class create_task trainee;
class gather trainee;
class sleep trainee;
class run trainee;
class wait_for trainee;
class asQueue trainee;
class Lock trainee;
class Event trainee;
class variables trainee;
class Thread trainee;
class Pool trainee;
class Stopwatch trainee;
class timeit trainee;
class random_mod trainee;
class input trainee;
class Command_Line_Arguments trainee;
class simple_print trainee;
class MD5 trainee;
class AES trainee;
class pytest trainee;
class FizzBuzz trainee;
class BubbleSort trainee;
class QuickSort trainee;
class RadixSort trainee;
class Adjacency_Matrix trainee;
class Adjacency_List trainee;
class Linear_Search trainee;
class Binary_Search trainee;
class DFS trainee;
class bigo trainee;
class divide_and_conquer trainee;
class Greedy_algorithm trainee;
class Recursion trainee;
class Relational_model trainee;
class Transaction trainee;
class Isolation trainee;
class PostgreSQL_benefits trainee;
class peewee trainee;
class CREATE trainee;
class ALTER trainee;
class DROP trainee;
class SELECT trainee;
class INSERT trainee;
class UPDATE trainee;
class DELETE trainee;
class PRIMARY_KEY trainee;
class FOREIGN_KEY trainee;
class FROM trainee;
class WHERE trainee;
class SET trainee;
class SQLite_benefits trainee;
class Syntax_Diagrams trainee;
class Flask trainee;
class Consistency trainee;
class HTTPS trainee;
class requests trainee;
class websocket trainee;
class GitHub_Actions trainee;
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
class trunk_based_development trainee;
class aiohttp trainee;
class StreamHandler trainee;
class Observer trainee;
class Decorator_Method trainee;
class Factory_Method trainee;
class Adapter_Facade trainee;
class CQRS trainee;
class Decentralization trainee;
class Smart_endpoints_dumb_pipes trainee;
class Basics trainee;
class GitHub trainee;
class Install trainee;
class Directory_Structure trainee;
class Terminal trainee;

class bash middle;
class System_administration middle;
class Network_administration middle;
class NoSQL middle;
class Functional middle;
class RabbitMQ middle;
class Scrum middle;
class Apache_Kafka middle;
class Docker middle;
class methmore middle;
class PostgreSQL_more middle;
class SQLAlchemy middle;
class Django_ORM middle;
class Django middle;
class FastAPI middle;
class SQL_standard middle;
class Analyze_an_execution_plan middle;
class TensorFlow middle;
class Keras middle;
class cryptomore middle;
class Jenkins middle;
class Kubernetes middle;
class Creational_patterns middle;
class Structural_patterns middle;
class Behavioral_patterns middle;
class Architectural_Patterns middle;
class ELK_Stack middle;
class Pattern_of_Distributed_Systems middle;
class Cloud_Design_Patterns middle;
class New_Relic middle;
```
