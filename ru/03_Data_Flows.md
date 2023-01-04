## Потоки данных

Добавьте к своим навыкам управления данными более специфичные возможности. Все рассмотренные темы крайне необходимы в процессе практического программирования и в том или ином виде присутствуют во всех современных языках. Так что если со временем вы будете переходить с Python на Java, C# или C++ — полученные знания не станут балластом.

```mermaid
flowchart TD

subgraph Data_Flows
direction LR

itertools -.-> enumerate -.-> Generator -.-> Decorator -.-> Context_managers

subgraph itertools
direction LR

subgraph Infinite_Iterators
icount(count)
icycle(cycle)
irepeat(repeat)
end

subgraph Finite_Iterators
accumulate(accumulate)
chain(chain)
compress(compress)
dropwhile(dropwhile)
takewhile(takewhile)
fimore(...)
end

subgraph Combinatorics
product(product)
combinations(combinations)
permutations(permutations)
combinations_with_replacement(combinations_with_replacement)
end
end

enumerate(enumerate)

subgraph Generator
direction LR
yield("yield")
yield_from("yield from")
Generator_expression("Generator expression")
end

subgraph Decorator
direction LR
decorator(decorator)
LRUCache("LRU Cache")
param_decorator("Parameterized decorator")
end

subgraph Context_managers
direction LR
enter_exit_cm("__enter__, __exit__")
contextlib(contextlib)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px

class icount trainee;
class icycle trainee;
class irepeat trainee;
class accumulate trainee;
class chain trainee;
class compress trainee;
class dropwhile trainee;
class takewhile trainee;
class product trainee;
class combinations trainee;
class enumerate trainee;
class yield trainee;
class decorator trainee;
class enter_exit_cm trainee;
```
