## Многопоточность и многопроцессность

Прежде чем погрузиться в изучение многопоточности и многопроцессной обработки данных, обязательно изучите их типовые сценарии использования. Возможны ситуации, когда выигрыш будет минимальным или будет отсутствовать вовсе.

Попробуйте реализовать совместную быструю обработку данных и ожидание пользовательского ввода, меняющего исходные данные для расчетов, это даст вам понимание возможностей, плюсов и минусов разных подходов.

Не пытайтесь использовать сразу все возможности, предоставляемые Python, отталкивайтесь от решаемой задачи.

```mermaid
flowchart TD

subgraph Multithreading_&_Multiprocessing
direction LR

Multithreading -.-> asyncio -.-> Multiprocessing -.->Synchronization

subgraph Multithreading
direction LR
Thread(Thread)
Thread_Pool_Executor("Thread pool executor")
Timer
end

subgraph asyncio
direction LR
subgraph High_level_API
sleep(sleep)
run(run)
create_task(create_task)
gather(gather)
hilapi_more("...")
end
subgraph asyncio_Queues
asQueue(Queue)
asPriorityQueue(PriorityQueue)
asLifoQueue(LifoQueue)
end
subgraph asyncio_Streams
StreamReader(StreamReader)
StreamWriter(StreamWriter)
end
subgraph Low_level_API
new_event_loop(new_event_loop)
run_forever(run_forever)
lowlapi_more("...")
end
end

subgraph Multiprocessing
direction LR
Pool(Pool)
Process(Process)
Pipe(Pipe)
Value(Value)
muArray(Array)
Manager(Manager)
Listener(Listener)
end

subgraph Synchronization
direction LR
Lock(Lock)
Event(Event)
Condition(Condition)
Semaphore(Semaphore)
BoundedSemaphore(BoundedSemaphore)
Barrier(Barrier)
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px

class Thread trainee;
class sleep trainee;
class run trainee;
class create_task trainee;
class gather trainee;
class asQueue trainee;
class Pool trainee;
class Lock trainee;
class Event trainee;
```
