## Language Skeleton

Perfect, a bit deeper now. Studying how GIL or GC works will give you an understanding of why things go awry in one case or another, not at all the way you planned. You are likely to use exceptions all the time, given that they can occur in some operations with data structures, so study them further.

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
classDef middle fill:#FF9900, stroke-width:3px

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
