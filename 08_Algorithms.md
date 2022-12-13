## Algorithms

One of those areas of human knowledge that you can delve into endlessly. On the other hand, the learning curve of this discipline for covering the practical needs of the average programmer has long been known, so the initial stages shouldn't be too difficult for you. Who knows, maybe you'll enjoy it so much and drag it out that in time you might even be able to contribute a new robust argument in the discussion of “[Equality of P and NP classes](https://en.wikipedia.org/wiki/P_versus_NP_problem)”!

```mermaid
flowchart TD

subgraph Algorithms
direction LR
FizzBuzz -.-> bigo -.-> Sort -.-> Graphs -.-> Search -.-> Methods
Recursion ==> Recursion

FizzBuzz(FizzBuzz)
bigo("O(n)")

subgraph Sort
direction LR
BubbleSort(BubbleSort)
QuickSort(QuickSort)
MergeSort(MergeSort)
HeapSort(HeapSort)
InsertionSort(InsertionSort)
RadixSort(RadixSort)
end

subgraph Graphs
direction LR
Adjacency_Matrix("Adjacency matrix")
Incidence_Matrix("Incidence matrix")
Adjacency_List("Adjacency list")
Incidence_List("Incidence list")
end

subgraph Search
direction LR
Linear_Search("Linear search")
Binary_Search("Binary search")
DFS(DFS)
BFS(BFS)
Dijkstras(Dijkstras)
Bellman_Ford("Bellman–Ford")
end

subgraph Methods
direction LR
divide_and_conquer("Divide and conquer")
Dynamic_programming("Dynamic programming")
Greedy_algorithm("Greedy algorithm")
Recursion(Recursion)
methmore("...")
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

class FizzBuzz trainee;
class bigo trainee;
class BubbleSort trainee;
class QuickSort trainee;
class RadixSort trainee;
class Adjacency_Matrix trainee;
class Adjacency_List trainee;
class Linear_Search trainee;
class Binary_Search trainee;
class DFS trainee;
class divide_and_conquer trainee;
class Recursion trainee;
class Greedy_algorithm trainee;

class methmore middle;
```
