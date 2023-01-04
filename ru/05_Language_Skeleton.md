## Специфика языка

Так, отлично, еще немного глубже. Изучение особенностей работы GIL или GC даст вам понимание, почему в том или ином случае всё идет наперекосяк, совсем не так, как вы планировали. А исключения вы, возможно, уже вовсю используете, учитывая их возможное возникновение при некоторых операциях со структурами данных, так что просто изучите их поглубже.

```mermaid
flowchart TD

subgraph Language_Skeleton
direction LR
Garbage_Collector -.-> Exception -.-> Typing -.-> Introspection -.-> Other

subgraph Garbage_Collector
direction LR
reference_counting("Reference counting")
garbage_collector("Garbage collector")
debug_objgraph("GC debug / objgraph")
pypygc("PyPy GC")
end

subgraph Exception
direction LR
exception_handling("Exception handling")
built_in_exceptions("Built-in exceptions")
exception_raising("Exception raising")
user_exception("User exceptions")
exception_object("Exception Object")
end

subgraph Typing
direction LR
typing_loc(typing)
Protocol(Protocol)
final("final (name mangling)")
Literal(Literal)
TypedDict(TypedDict)
end

subgraph Introspection
direction LR
variables(variables)
attributes(attributes)
parameters(parameters)
end

subgraph Other
direction LR
GIL(GIL)
args_kwargs("*, *args, **kwargs")
lambda(lambda)
Closure(Closure)
Operator(Operator)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px

class reference_counting trainee;
class garbage_collector trainee;
class exception_handling trainee;
class built_in_exceptions trainee;
class exception_raising trainee;
class typing_loc trainee;
class variables trainee;
class GIL trainee;
class args_kwargs trainee;
class lambda trainee;
```
