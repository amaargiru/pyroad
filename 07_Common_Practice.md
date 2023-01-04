## Common Practices

Description of common methods used in almost all software projects, not just in Python. I/O, profiling, and logging apply universally.

Testing in general constitutes a separate profession, and often the quality of a software product can be judged by the test coverage of the source code. For example, the code of the SQLite database is 100% [covered by tests](https://www.sqlite.org/testing.html), while one line of "combative" code requires 608 lines of tests.  
Jokes aside, projects with 100% coverage are not common, but pytest used wisely is the best guarantor of your sound sleep at night!

```mermaid
flowchart TD

subgraph Common_Practice
direction LR

Logging -.-> Profiling -.-> Random -.-> Input -.-> Print -.-> Cryptography -.-> Testing

subgraph Logging
direction LR
StreamHandler(StreamHandler)
ColoredFormatter(ColoredFormatter)
Log_formatting("Log formatting")
RotatingFileHandler(RotatingFileHandler)
TimedRotatingFileHandler(TimedRotatingFileHandler)
ELK_Stack("ELK Stack")
end

subgraph Profiling
direction LR
Stopwatch(Stopwatch)
perf_counter(perf_counter)
timeit(timeit)
Call_Graph("Call Graph")
end

subgraph Random
direction LR
random_mod(random)
secrets(secrets)
end

subgraph Input
direction LR
input(input)
Command_Line_Arguments("Command Line Arguments")
Argument_Parser("Argument Parser")
end

subgraph Print
direction LR
simple_print(print)
json_print("json.dumps")
Pretty_Print(pprint)
end

subgraph Cryptography
direction LR
MD5(MD5)
AES(AES)
cryptomore("...")
end

subgraph Testing
direction LR
pytest(pytest)
mock(mock)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

class StreamHandler trainee;
class Stopwatch trainee;
class timeit trainee;
class random_mod trainee;
class input trainee;
class Command_Line_Arguments trainee;
class simple_print trainee;
class MD5 trainee;
class AES trainee;
class pytest trainee;

class ELK_Stack middle;
class cryptomore middle;
```
