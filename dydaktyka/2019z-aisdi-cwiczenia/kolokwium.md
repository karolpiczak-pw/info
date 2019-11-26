---
description: Zakres materiału obowiązującego na kolokwium
---

# Kolokwium

## Ćwiczenia 1

### **Tablica, std::array, std::vector**

{% tabs %}
{% tab title="Zakres materiału" %}
* podstawowe **operacje na tablicy/wektorze** i ich złożoność:
  * dostęp,
  * wstawianie elementu \(na końcu/w środku\),
  * usuwanie elementu \(z końca/ze środka\),
  * wyszukiwanie elementu o określonej wartości
* różnica między `std::vector::size()` a `std::vector::capacity()`,
* wykorzystanie **iteratorów**
{% endtab %}
{% endtabs %}

### **Lista jedno- i dwukierunkowa**

{% tabs %}
{% tab title="Zakres materiału" %}
* podstawowe **operacje na liście** i ich złożoność:
  * dostęp,
  * wstawianie elementu,
  * usuwanie elementu,
  * wyszukiwanie elementu o określonej wartości
* **wyszukiwanie ze strażnikiem**
{% endtab %}

{% tab title="Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [https://www.geeksforgeeks.org/data-structures/linked-list/](https://www.geeksforgeeks.org/data-structures/linked-list/)

**Wykorzystanie strażnika:**

* [https://en.wikipedia.org/wiki/Sentinel\_node](https://en.wikipedia.org/wiki/Sentinel_node)
* [https://stackoverflow.com/a/5384593/308759](https://stackoverflow.com/a/5384593/308759)

**Wizualizacje:**

* [https://visualgo.net/en/list](https://visualgo.net/en/list)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Przykładowe zadania (**lista**):" %}
{% endtab %}

{% tab title="1.1" %}
Dany jest następujący szkielet klasy listy jednokierunkowej:

```cpp
struct Node {
    Node* next;
    int value;
};

class LinkedList {
  public:
    int length;
    Node* head;

    LinkedList();

    void erase_after(int pos);  // usuwa elem. za pozycją pos
    void insert_after(int pos, int value);  // wstawia elem. za pozycją pos
    void pop_front();  // usuwa pierwszy element
    void push_front(int value);  // wstawia element na początek listy
};
```

Zaimplementuj brakujące metody.
{% endtab %}

{% tab title="1.2" %}
Zaimplementuj metodę, która dla listy jednokierunkowej zwróci trzeci element od końca. Załóż, że długość listy nie jest znana.
{% endtab %}

{% tab title="1.3" %}
Zaimplementuj metodę, która zwróci środkowy element listy jednokierunkowej. Załóż, że długość listy nie jest znana.
{% endtab %}

{% tab title="1.4" %}
Zaproponuj sposób odwracania listy jednokierunkowej w jednym przejściu bez tworzenia kopii wszystkich elementów.
{% endtab %}

{% tab title="1.5" %}
Zaproponuj sposób usuwania węzła mając tylko odwołanie do niego. Załóż, że nie jest to ostatni węzeł listy.
{% endtab %}

{% tab title="1.6" %}
Zaimplementuj uproszczony iterator \(tylko operacje `->` i `++` \) po elementach listy. Jak wyglądałby taki iterator, gdyby miał zwracać najpierw elementy na rosnących pozycjach nieparzystych listy, a następnie na parzystych?
{% endtab %}
{% endtabs %}

### **Kolejka \(FIFO\), stos \(LIFO\)**

{% tabs %}
{% tab title="Zakres materiału" %}
* pojęcie **abstrakcyjnego typu danych** \(_abstract data type, ADT_\),
* **kolejka** i **stos** jako przykłady ADT,
* implementacja funkcjonalności kolejki i stosu na bazie listy dwukierunkowej
{% endtab %}

{% tab title="Materiały pomocnicze" %}
{% hint style="info" %}
**ADT:**

* [https://en.wikipedia.org/wiki/Queue\_\(abstract\_data\_type\)](https://en.wikipedia.org/wiki/Queue_%28abstract_data_type%29)
* [https://en.wikipedia.org/wiki/Stack\_\(abstract\_data\_type\)](https://en.wikipedia.org/wiki/Stack_%28abstract_data_type%29)

**Wizualizacje:**

* [https://visualgo.net/en/list?slide=5](https://visualgo.net/en/list?slide=5)
* [https://visualgo.net/en/list?slide=4](https://visualgo.net/en/list?slide=4)
{% endhint %}
{% endtab %}
{% endtabs %}

### Binarne drzewo poszukiwań \(BST\)

{% tabs %}
{% tab title="Zakres materiału" %}
* **drzewo binarne**, definicja, podstawowe własności,
* **binarne drzewo poszukiwań** \(_binary search tree_, _BST_\):
  * podstawowe operacje i ich złożoność:
    * dostęp,
    * wyszukiwanie elementu,
    * wstawianie elementu,
    * usuwanie elementu
  * przechodzenie po węzłach drzewa:
    * in-order,
    * pre-order,
    * post-order
  * implementacja iteratora dla drzewa
{% endtab %}

{% tab title="Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [https://en.wikipedia.org/wiki/Binary\_tree](https://en.wikipedia.org/wiki/Binary_tree)
* [https://pl.wikipedia.org/wiki/Binarne\_drzewo\_poszukiwa%C5%84](https://pl.wikipedia.org/wiki/Binarne_drzewo_poszukiwa%C5%84)
* [https://www.programiz.com/dsa/breadth-first-search-tree](https://www.programiz.com/dsa/breadth-first-search-tree)

**Przechodzenie drzewa:**

* [https://en.wikipedia.org/wiki/Tree\_traversal](https://en.wikipedia.org/wiki/Tree_traversal)
* [https://leetcode.com/problems/binary-search-tree-iterator/solution/](https://leetcode.com/problems/binary-search-tree-iterator/solution/)

**Wizualizacje:**

* [https://visualgo.net/en/bst](https://visualgo.net/en/bst)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Przykładowe zadania (**BST**):" %}

{% endtab %}

{% tab title="1.7" %}
Narysuj binarne drzewo poszukiwań utworzone przez wstawienie w kolejności elementów:

`31, 72, 23, 44, 85, 106, 17, 28, 9, 30, 41`
{% endtab %}

{% tab title="1.8" %}
Zaimplementuj metody wstawiania i wyszukiwania węzła w drzewie BST.
{% endtab %}

{% tab title="1.9" %}
Zaimplementuj rekursywne przechodzenie po węzłach drzewa w kolejności "in-order".
{% endtab %}

{% tab title="1.10" %}
Zaimplementuj uproszczony iterator \(tylko operacje `->` i `++` \), który będzie przechodził węzły drzewa w kolejności "in-order".
{% endtab %}

{% tab title="1.11" %}
Zaimplementuj w klasie drzewa BST funkcjonalność usuwania węzła o zadanej wartości.
{% endtab %}
{% endtabs %}

## Ćwiczenia 2

### Algorytmy sortowania

{% tabs %}
{% tab title="Zakres materiału" %}
**Algorytmy:**

* sortowanie przez wybieranie \(_**selection sort**_\),
* sortowanie przez wstawianie \(_**insertion sort**_\),
* sortowanie bąbelkowe \(_**bubble sort**_\),
* sortowanie szybkie \(_**quicksort**_\),
* sortowanie przez scalanie \(_**merge** **sort**_\),
* sortowanie przez kopcowanie \(_**heapsort**_\),
* sortowanie kubełkowe \(_**bucket sort**_\)

**Dla przedstawionych algorytmów:**

* implementacja,
* złożoność czasowa \(najlepsza, średnia, najgorsza\),
* złożoność pamięciowa,
* stabilność
{% endtab %}

{% tab title="Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [https://en.wikipedia.org/wiki/Sorting\_algorithm](https://en.wikipedia.org/wiki/Sorting_algorithm)
* [https://en.wikipedia.org/wiki/File:Sorting\_stability\_playing\_cards.svg](https://en.wikipedia.org/wiki/File:Sorting_stability_playing_cards.svg)
* [https://www.oreilly.com/library/view/algorithms-in-a/9781491912973/ch04.html](https://www.oreilly.com/library/view/algorithms-in-a/9781491912973/ch04.html)

**Algorytmy:**

* [selection sort](https://www.w3resource.com/python-exercises/data-structures-and-algorithms/python-search-and-sorting-exercise-5.php)
* [bubble sort](https://www.w3resource.com/javascript-exercises/javascript-function-exercise-24.php)
* [insertion sort](https://www.w3resource.com/python-exercises/data-structures-and-algorithms/python-search-and-sorting-exercise-6.php)
* [quicksort](https://www.w3resource.com/csharp-exercises/searching-and-sorting-algorithm/searching-and-sorting-algorithm-exercise-9.php)
* [merge sort](https://www.101computing.net/merge-sort-algorithm/)
* [heapsort](https://www.hackerearth.com/practice/algorithms/sorting/heap-sort/tutorial/)
* [bucket sort](https://www.programiz.com/dsa/bucket-sort)

**Wizualizacje:**

* [http://sorting.at/](http://sorting.at/)
* [https://visualgo.net/en/sorting](https://visualgo.net/en/sorting)
* [https://www.cs.usfca.edu/~galles/visualization/ComparisonSort.html](https://www.cs.usfca.edu/~galles/visualization/ComparisonSort.html)
* [https://www.toptal.com/developers/sorting-algorithms](https://www.toptal.com/developers/sorting-algorithms)
* [https://www.cs.usfca.edu/~galles/visualization/BucketSort.html](https://www.cs.usfca.edu/~galles/visualization/BucketSort.html)
{% endhint %}
{% endtab %}
{% endtabs %}

## Ćwiczenia 3

### Drzewa

{% tabs %}
{% tab title="Zakres materiału" %}
* drzewa BST zrównoważone i niezrównoważone,
* **rotacje drzew,**
* **drzewa splay**:
  * implementacja i złożoność obliczeniowa:
    * operacja _splay_,
    * wyszukiwanie elementu,
    * wstawianie elementu,
    * usuwanie elementu,
  * zastosowania drzewa splay, zalety i wady
* **drzewa AVL**:
  * wysokość, współczynnik wyważenia,
  * operacje równoważenia drzewa AVL,
  * implementacja i złożoność obliczeniowa:
    * wyszukiwanie elementu,
    * wstawianie elementu,
    * usuwanie elementu
{% endtab %}

{% tab title="Materiały pomocnicze" %}
{% hint style="info" %}
**Zrównoważenie drzewa BST:**

* [wyważanie drzewa](https://pl.wikipedia.org/wiki/Binarne_drzewo_poszukiwa%C5%84#Wywa%C5%BCanie_drzewa)

**Rotacje:**

* \*\*\*\*[https://en.wikipedia.org/wiki/Tree\_rotation](https://en.wikipedia.org/wiki/Tree_rotation)

**Drzewa splay:**

* [https://pl.wikipedia.org/wiki/Drzewo\_splay](https://pl.wikipedia.org/wiki/Drzewo_splay)
* [https://cs.stackexchange.com/q/1229/8837](https://cs.stackexchange.com/q/1229/8837)
* [https://www.cs.cmu.edu/~sleator/papers/self-adjusting.pdf](https://www.cs.cmu.edu/~sleator/papers/self-adjusting.pdf)
* [https://people.eecs.berkeley.edu/~jrs/61b/lec/36](https://people.eecs.berkeley.edu/~jrs/61b/lec/36)

**Drzewa AVL:**

* [https://en.wikipedia.org/wiki/AVL\_tree](https://en.wikipedia.org/wiki/AVL_tree)
* [https://www.codesdope.com/course/data-structures-avl-trees/](https://www.codesdope.com/course/data-structures-avl-trees/)

**Wizualizacje:**

* [https://www.cs.usfca.edu/~galles/visualization/SplayTree.html](https://www.cs.usfca.edu/~galles/visualization/SplayTree.html)
* [https://visualgo.net/en/bst?slide=14](https://visualgo.net/en/bst?slide=14)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Przykładowe zadania (**drzewa**):" %}

{% endtab %}

{% tab title="3.1" %}
Stwórz dwa drzewa BST przez wstawianie w kolejności następujących wartości:

`A: 40, 20, 60, 10, 30, 50, 70`

`B: 10, 20, 30, 40, 50, 60, 70`

Porównaj złożoność podstawowych operacji dla obydwu drzew.

Następnie dla drzewa niezrównoważonego **B** wykonaj kolejno operacje rotacji:

* `L(40)`
* `L(30)`
* `L(20)`
* `L(10)`
* `L(20)`

{% hint style="info" %}
Zapis `L(R)` oznacza rotację lewą, dla której korzeniem jest węzeł o wartości `R`.
{% endhint %}
{% endtab %}

{% tab title="3.2" %}
Dane jest drzewo splay o takiej samej strukturze jak drzewo A z zadania 1.

Wykonaj w kolejności następujące operacje:

* znajdź element o wartości `30`,
* znajdź element o wartości `50`,
* wstaw element o wartości `25`,
* wstaw element o wartości `22`,
* usuń element o wartości `50`,
* usuń element o wartości `25`.
{% endtab %}

{% tab title="3.3" %}
Stwórz drzewo AVL przez wstawianie kolejno wartości:

`10, 20, 30, 40, 50, 60, 70`

Na stworzonym drzewie przeprowadź operacje:

* wstaw element o wartości `55`,
* wstaw element o wartości `52`,
* usuń element o wartości `52`,
* usuń element o wartości `70`.
{% endtab %}
{% endtabs %}

## Ćwiczenia 4

### Kopce

{% tabs %}
{% tab title="Zakres materiału" %}
* kolejka priorytetowa \(_**priority queue**_, _ADT_\),
* **kopiec binarny**:
  * własność kopca _**min-heap**_, _**max-heap**_,
  * reprezentacja tablicowa kopca \(_implicit data structure_\),
  * implementacja i złożoność obliczeniowa operacji:
    * dostęp do najmniejszego elementu,
    * wstawianie nowego elementu,
    * usuwanie najmniejszego elementu,
    * budowa kopca:
      * metoda Williamsa \(sukcesywne wstawianie elementów\),
      * metoda Floyda \(przywracanie własności kopca dla tablicy\)
* **kopce** _**d**_**-arne**:
  * _3_-heap \(_ternary heap_\) i _4_-heap \(_quaternary heap_\),
  * zalety i wady zastosowania arności wyższego rzędu,
* **kopiec dwumianowy**:
  * kopiec dwumianowy jako przykład kopca złączalnego \(_**mergeable heap**_\),
  * własności kopca dwumianowego,
  * implementacja i złożoność obliczeniowa operacji:
    * dostęp do najmniejszego elementu,
    * wstawianie nowego elementu,
    * usuwanie najmniejszego elementu,
    * scalanie kopców
* **kopiec Fibonacciego**:
  * implementacja i złożoność obliczeniowa operacji:
    * dostęp do najmniejszego elementu,
    * wstawianie nowego elementu,
    * usuwanie najmniejszego elementu,
    * scalanie kopców
{% endtab %}

{% tab title="Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [https://en.wikipedia.org/wiki/Priority\_queue](https://en.wikipedia.org/wiki/Priority_queue)
* [https://en.wikipedia.org/wiki/Heap\_\(data\_structure\)](https://en.wikipedia.org/wiki/Heap_%28data_structure%29)
* [https://en.wikipedia.org/wiki/Implicit\_data\_structure](https://en.wikipedia.org/wiki/Implicit_data_structure)

**Kopiec binarny:**

* [https://en.wikipedia.org/wiki/Binary\_heap](https://en.wikipedia.org/wiki/Binary_heap)
* [https://stackoverflow.com/questions/9755721/how-can-building-a-heap-be-on-time-complexity](https://stackoverflow.com/questions/9755721/how-can-building-a-heap-be-on-time-complexity)
* [https://brilliant.org/wiki/binary-heap/](https://brilliant.org/wiki/binary-heap/)

**Kopce** _**d**_**-arne:**

* [https://en.wikipedia.org/wiki/D-ary\_heap](https://en.wikipedia.org/wiki/D-ary_heap)
* [https://stackoverflow.com/questions/29126428/binary-heaps-vs-d-ary-heaps](https://stackoverflow.com/questions/29126428/binary-heaps-vs-d-ary-heaps)
* [https://stackoverflow.com/questions/48843677/why-dont-we-use-ternary-or-quaternary-heaps](https://stackoverflow.com/questions/48843677/why-dont-we-use-ternary-or-quaternary-heaps)

**Kopiec dwumianowy:**

* [https://en.wikipedia.org/wiki/Binomial\_heap](https://en.wikipedia.org/wiki/Binomial_heap)
* [https://brilliant.org/wiki/binomial-heap/](https://brilliant.org/wiki/binomial-heap/)
* [https://www.growingwiththeweb.com/data-structures/binomial-heap/overview/](https://www.growingwiththeweb.com/data-structures/binomial-heap/overview/)

**Kopiec Fibonacciego:**

* [https://en.wikipedia.org/wiki/Fibonacci\_heap](https://en.wikipedia.org/wiki/Fibonacci_heap)
* [https://brilliant.org/wiki/fibonacci-heap/](https://brilliant.org/wiki/fibonacci-heap/)

**Wizualizacje:**

* [https://visualgo.net/en/heap](https://visualgo.net/en/heap)
* [https://www.cs.usfca.edu/~galles/visualization/Heap.html](https://www.cs.usfca.edu/~galles/visualization/Heap.html)
* [https://www.cs.usfca.edu/~galles/visualization/BinomialQueue.html](https://www.cs.usfca.edu/~galles/visualization/BinomialQueue.html)
* [https://www.cs.usfca.edu/~galles/visualization/FibonacciHeap.html](https://www.cs.usfca.edu/~galles/visualization/FibonacciHeap.html)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="Przykładowe zadania (**kopce**):" %}

{% endtab %}

{% tab title="4.1" %}
Zapisz w reprezentacji tablicowej drzewo binarne następującej postaci:

![](../../.gitbook/assets/tree%20%283%29.png)
{% endtab %}

{% tab title="4.2" %}
Dla zapisu tablicowego:

`[95, 80, 85, 40, 70, 90, 50, 30, 10, 20]`

narysuj zupełne drzewo binarne. Czy drzewo to przedstawia kopiec typu _max-heap_?
{% endtab %}

{% tab title="4.3" %}
Do pustego **kopca binarnego** _**max-heap**_ wstaw w kolejności elementy o wartościach klucza:

`43, 24, 11, 47, 13, 67, 59, 95, 29, 17, 54, 40`

Następnie trzykrotnie wykonaj operację usunięcia największego elementu z kopca.

Zilustruj stan kopca po każdym kroku.
{% endtab %}

{% tab title="4.4" %}
Z podanej tablicy stwórz **kopiec binarny typu** _**max-heap**_ metodą Floyda \(przywracanie własności kopca kolejnym poddrzewom\):

`[2, 7, 26, 25, 19, 17, 1, 90, 3, 36]`

Zlicz ilość wykonanych operacji, porównaj z metodą tworzenia kopca przez wstawianie.
{% endtab %}

{% tab title="4.5" %}
Do pustego **kopca 3-arnego \(**_**ternary heap**_**\) typu** _**max-heap**_ ****wstaw w kolejności elementy o wartościach klucza:

`43, 24, 11, 47, 13, 67, 59, 95, 29, 17, 54, 40`

Następnie trzykrotnie wykonaj operację usunięcia największego elementu z kopca.

Zilustruj stan kopca po każdym kroku.
{% endtab %}

{% tab title="4.6" %}
Do pustego **kopca dwumianowego typu** _**min-heap**_ wstaw w kolejności elementy o wartościach klucza:

`43, 24, 11, 47, 13, 67, 59, 95, 29, 17, 54, 40`

Następnie trzykrotnie wykonaj operację usunięcia najmniejszego elementu z kopca.

Zilustruj stan kopca po każdym kroku.
{% endtab %}

{% tab title="4.7" %}
Do pustego **kopca Fibonacciego typu** _**min-heap**_ wstaw w kolejności elementy o wartościach klucza:

`43, 24, 11, 47, 13, 67, 59, 95, 29, 17, 54, 40`

Następnie trzykrotnie wykonaj operację usunięcia najmniejszego elementu z kopca.

Zilustruj stan kopca po każdym kroku.

Porównaj stany przejściowe kopca stworzonego na bazie poniższego ciągu operacji:

* `push(43)`,
* `push(24)`,
* `push(11)`,
* `push(47)`,
* `pop()`,
* `push(13)`,
* `push(67)`,
* `pop()`,
* `push(59)`,
* `push(95)`,
* `pop()`,
* `push(29)`,
* `push(17)`,
* `pop()`,
* `push(54)`,
* `pop()`,
* `push(40)`.
{% endtab %}
{% endtabs %}
