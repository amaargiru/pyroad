## Манипуляция данными

Пробуйте управлять вашими данными, почувствуйте, как вы можете лепить всё что угодно из этой податливой глины. Попробуйте создать структуру данных на много элементов (миллион, например), отсортируйте (sort) их, молниеносно найдите нужные значения при помощи bisect и запишите полученные результаты в JSON-файл.

Если всё идет по плану, попробуйте копнуть «серые» темы: примените regex для решения какой-нибудь несложной задачи или запишите ранее полученные данные в формате Pickle, наглядно, по размеру получившихся файлов, поняв, зачем нужны двоичные форматы файлов.

Здесь вы видите первые пункты, помеченные оранжевым. Погуглите, что такое TensorFlow и Keras, какие задачи они решают. Может быть, это ваша будущая работа, ваше призвание?

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
