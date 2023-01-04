## Структуры данных

Напоминаю, если вы — начинающий разработчик, идите слева направо по пунктам, отмеченным зеленым цветом. Создайте экземпляры каждого типа, попробуйте добавить и удалить элементы, поработайте с ними в отладчике. Посмотрите, какого размера получаются объекты, попробуйте разобраться, почему list и array, содержащие одинаковые данные, отличаются в размерах. Изучите особенности каждого типа, почитайте и подумайте сами, в каких задачах какая структура данных будет смотреться оптимальнее.

Не забывайте, что это всего лишь путеводитель, оглавление для книги, которую вы должны написать сами. Активно ищите информацию в Сети, старайтесь работать с англоязычными источниками и с официальной документацией. Замените «Пикабу» и «ЯПлакал» на [Stackoverflow](https://stackoverflow.com/), там масса захватывающего чтива!

Если начинает получаться, переходите к следующему разделу, если не получается — не расстраивайтесь. Не надо ассоциировать свой ум с мечом Александра Македонского, разрубившего Гордиев узел одним чётким, уверенным движением, достойным главной страницы «Инстаграма». Будьте как рубанок — снимайте по тонкой кожурке за проход, и рано или поздно непонимание уйдёт, даже если вам кажется, что это пропасть глубиной в десять тысяч ли.

```mermaid
flowchart TD

subgraph Data_Structures
direction LR
List(list) -.-> Tuple -.-> Dict -.-> Set -.-> Array -.-> Linked_List -.->Tree -.-> Python_specific_data_structures

subgraph Tuple
direction LR
tuple(tuple)
namedtuple(namedtuple)
end

subgraph Dict
direction LR
dict(dict)
HashProblem("Hash collisions")
defaultdict(defaultdict)
Counter(Counter)
end

subgraph Set
direction LR
set(set)
FrozenSet("frozen set")
end

subgraph Array
direction LR
array(array)
bytes(bytes)
bytearray(bytearray)
end

subgraph Linked_List
direction LR
SinglyLinkedList("Singly linked list")
subgraph Doubly_Linked_List
direction LR
deque(deque)
Queue(Queue)
end
end

subgraph Tree
direction LR
tree(tree)
heap(heap)
B-tree(B-tree)
RedBlackTree("Red–black tree")
AVLTree("AVL tree")
trie(trie)
end

subgraph Python_specific_data_structures
direction LR
enum(enum)
range(range)
dataclass(dataclass)
struct(struct)
string(string)
datetime(datetime)
end
end

classDef trainee fill:#6ADA6A, stroke-width:3px

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
```
