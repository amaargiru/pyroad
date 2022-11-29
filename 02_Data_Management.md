## Data Management

Try to manipulate your data, feel how you can mold anything you want out of this malleable clay. Try creating a data structure with many elements (a million, for example), sort them, quickly find the values you want with bisect, and write the results in a JSON file.

If everything goes according to plan, try to dig into the less obvious topics: apply regex to solve some simple task or save previously obtained data in Pickle format, understanding the reason for binary file formats after observing the size of the resulting files.

This is where you will find the first entries marked in orange. Google what TensorFlow and Keras are and what tasks they solve. Perhaps, this could be your future job, your vocation!

```mermaid
flowchart TD

subgraph Data_Management
direction LR
slice(slice) -.-> Sorting -.-> Comprehension -.-> String_Management -.-> Datetime_Management -.-> bisect(bisect) -.-> Functools -.->File -.-> Data_Analysis -.-> Neural_Networks
subgraph Sorting
direction LR
sort(sort)
sorted(sorted)
end

subgraph Comprehension
direction LR
listcomprehension(list)
dictcomprehension(dict)
setcomprehension(set)
end

subgraph String_Management
direction LR
String_Built-in_Functions("Built-in functions")
regex(regex)
end

subgraph Datetime_Management
direction LR
encode(encode)
decode(decode)
dtmath(math)
end

subgraph Functools
direction LR
fmap(map)
ffilter(filter)
freduce(reduce)
fpartial(partial)
fmore(...)
end

subgraph File
direction LR
Read_Write("read/write")
Text_Binary("text/binary")
JSON(JSON)
Pickle("Pickle")
Protocol_Buffers("Protocol Buffers")
paths(paths)
end

subgraph Data_Analysis
direction LR
Data_Built-in_Functions("Built-in functions")
NumPy(NumPy)
Pandas(Pandas)
Matplotlib_Seaborn("Matplotlib/Seaborn")
end

subgraph Neural_Networks
direction LR
PyTorch(PyTorch)
TensorFlow("TensorFlow/Keras")
end

end

classDef trainee fill:#6ADA6A, stroke-width:3px
classDef middle fill:#FF9900, stroke-width:3px

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

class PyTorch middle;
class TensorFlow middle;
```
