---
description: Zakres materiału obowiązującego na kolokwium
---

# Kolokwium

## Ćwiczenia 1

{% hint style="info" %}
Przykłady implementacji struktur listowych dostępne są w [repozytorium z materiałami do przedmiotu](https://github.com/karolpiczak-pw/2019Z-AISDI/tree/master/examples/01-list-bst).
{% endhint %}

### 1.1 **Tablica, std::array, std::vector**

{% tabs %}
{% tab title="1.1 Zakres materiału" %}
* podstawowe **operacje na tablicy/wektorze** i ich złożoność:
  * dostęp,
  * wstawianie elementu \(na końcu/w środku\),
  * usuwanie elementu \(z końca/ze środka\),
  * wyszukiwanie elementu o określonej wartości
* różnica między `std::vector::size()` a `std::vector::capacity()`,
* wykorzystanie **iteratorów**
{% endtab %}
{% endtabs %}

### 1.2 **Lista jedno- i dwukierunkowa**

{% tabs %}
{% tab title="1.2 Zakres materiału" %}
* podstawowe **operacje na liście** i ich złożoność:
  * dostęp,
  * wstawianie elementu,
  * usuwanie elementu,
  * wyszukiwanie elementu o określonej wartości
* **wyszukiwanie ze strażnikiem**
{% endtab %}

{% tab title="1.2 Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [Linked list data structure \(Geeks for Geeks\)](https://www.geeksforgeeks.org/data-structures/linked-list/)

**Wykorzystanie strażnika:**

* [Sentinel node \(Wikipedia\)](https://en.wikipedia.org/wiki/Sentinel_node)
* [Using sentinel nodes \(Stack Overflow\)](https://stackoverflow.com/a/5384593/308759)

**Wizualizacje:**

* [List \(VisuAlgo\)](https://visualgo.net/en/list)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="1.2 Zadania:" %}

{% endtab %}

{% tab title="1.2.1" %}
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

{% tab title="1.2.2" %}
Zaimplementuj metodę, która dla listy jednokierunkowej zwróci trzeci element od końca. Załóż, że długość listy nie jest znana.
{% endtab %}

{% tab title="1.2.3" %}
Zaimplementuj metodę, która zwróci środkowy element listy jednokierunkowej. Załóż, że długość listy nie jest znana.
{% endtab %}

{% tab title="1.2.4" %}
Zaproponuj sposób odwracania listy jednokierunkowej w jednym przejściu bez tworzenia kopii wszystkich elementów.
{% endtab %}

{% tab title="1.2.5" %}
Zaproponuj sposób usuwania węzła mając tylko odwołanie do niego. Załóż, że nie jest to ostatni węzeł listy.
{% endtab %}

{% tab title="1.2.6" %}
Zaimplementuj uproszczony iterator \(tylko operacje `->` i `++` \) po elementach listy. Jak wyglądałby taki iterator, gdyby miał zwracać najpierw elementy na rosnących pozycjach nieparzystych listy, a następnie na parzystych?
{% endtab %}
{% endtabs %}

### 1.3 **Kolejka \(FIFO\), stos \(LIFO\)**

{% tabs %}
{% tab title="1.3 Zakres materiału" %}
* pojęcie **abstrakcyjnego typu danych** \(_abstract data type, ADT_\),
* **kolejka** i **stos** jako przykłady ADT,
* implementacja funkcjonalności kolejki i stosu na bazie listy dwukierunkowej
{% endtab %}

{% tab title="1.3 Materiały pomocnicze" %}
{% hint style="info" %}
**ADT:**

* [Queue ADT \(Wikipedia\)](https://en.wikipedia.org/wiki/Queue_%28abstract_data_type%29)
* [Stack ADT \(Wikipedia\)](https://en.wikipedia.org/wiki/Stack_%28abstract_data_type%29)

**Wizualizacje:**

* [Queue \(VisuAlgo\)](https://visualgo.net/en/list?slide=5)
* [Stack \(VisuAlgo\)](https://visualgo.net/en/list?slide=4)
{% endhint %}
{% endtab %}
{% endtabs %}

### 1.4 Binarne drzewo poszukiwań \(BST\)

{% tabs %}
{% tab title="1.4 Zakres materiału" %}
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

{% tab title="1.4 Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [Binary tree \(Wikipedia\)](https://en.wikipedia.org/wiki/Binary_tree)
* [Binarne drzewo poszukiwań \(Wikipedia\)](https://pl.wikipedia.org/wiki/Binarne_drzewo_poszukiwa%C5%84)
* [Binary search tree \(Programiz\)](https://www.programiz.com/dsa/breadth-first-search-tree)

**Przechodzenie drzewa:**

* [Tree traversal \(Wikipedia\)](https://en.wikipedia.org/wiki/Tree_traversal)
* [Binary search tree iterator \(LeetCode\)](https://leetcode.com/problems/binary-search-tree-iterator/solution/)

**Wizualizacje:**

* [BST \(VisuAlgo\)](https://visualgo.net/en/bst)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="1.4 Zadania" %}

{% endtab %}

{% tab title="1.4.1" %}
Narysuj binarne drzewo poszukiwań utworzone przez wstawienie w kolejności elementów:

`31, 72, 23, 44, 85, 106, 17, 28, 9, 30, 41`
{% endtab %}

{% tab title="1.4.2" %}
Zaimplementuj metody wstawiania i wyszukiwania węzła w drzewie BST.
{% endtab %}

{% tab title="1.4.3" %}
Zaimplementuj rekursywne przechodzenie po węzłach drzewa w kolejności "in-order".
{% endtab %}

{% tab title="1.4.4" %}
Zaimplementuj uproszczony iterator \(tylko operacje `->` i `++` \), który będzie przechodził węzły drzewa w kolejności "in-order".
{% endtab %}

{% tab title="1.4.5" %}
Zaimplementuj w klasie drzewa BST funkcjonalność usuwania węzła o zadanej wartości.
{% endtab %}
{% endtabs %}

## Ćwiczenia 2

{% hint style="info" %}
Przykładowe implementacje omawianych algorytmów sortowania dostępne są w [repozytorium z materiałami do przedmiotu](https://github.com/karolpiczak-pw/2019Z-AISDI/tree/master/examples/02-sorting).
{% endhint %}

### 2.1 Algorytmy sortowania

{% tabs %}
{% tab title="2.1 Zakres materiału" %}
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

{% tab title="2.1 Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [Sorting algorithm \(Wikipedia\)](https://en.wikipedia.org/wiki/Sorting_algorithm)
* [Sorting stability \(Wikipedia\)](https://en.wikipedia.org/wiki/File:Sorting_stability_playing_cards.svg)
* [Sorting algorithms \(O'Reilly\)](https://www.oreilly.com/library/view/algorithms-in-a/9781491912973/ch04.html)

**Algorytmy:**

* [Selection sort \(w3resource\)](https://www.w3resource.com/python-exercises/data-structures-and-algorithms/python-search-and-sorting-exercise-5.php)
* [Bubble sort \(w3resource\)](https://www.w3resource.com/javascript-exercises/javascript-function-exercise-24.php)
* [Insertion sort \(w3resource\)](https://www.w3resource.com/python-exercises/data-structures-and-algorithms/python-search-and-sorting-exercise-6.php)
* [Quicksort \(w3resource\)](https://www.w3resource.com/csharp-exercises/searching-and-sorting-algorithm/searching-and-sorting-algorithm-exercise-9.php)
* [Merge sort \(101computing\)](https://www.101computing.net/merge-sort-algorithm/)
* [Heapsort \(HackerEarth\)](https://www.hackerearth.com/practice/algorithms/sorting/heap-sort/tutorial/)
* [Bucket sort \(Programiz\)](https://www.programiz.com/dsa/bucket-sort)

**Wizualizacje:**

* [Sorting \(sorting.at\)](http://sorting.at/)
* [Sorting \(VisuAlgo\)](https://visualgo.net/en/sorting)
* [Comparison sorting \(USF\)](https://www.cs.usfca.edu/~galles/visualization/ComparisonSort.html)
* [Sorting algorithms \(toptal\)](https://www.toptal.com/developers/sorting-algorithms)
* [Bucket sort \(USF\)](https://www.cs.usfca.edu/~galles/visualization/BucketSort.html)
{% endhint %}
{% endtab %}
{% endtabs %}

## Ćwiczenia 3

### 3.1 Drzewa

{% tabs %}
{% tab title="3.1 Zakres materiału" %}
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

{% tab title="3.1 Materiały pomocnicze" %}
{% hint style="info" %}
**Zrównoważenie drzewa BST:**

* [Wyważanie drzewa \(Wikipedia\)](https://pl.wikipedia.org/wiki/Binarne_drzewo_poszukiwa%C5%84#Wywa%C5%BCanie_drzewa)

**Rotacje:**

* [Tree rotation \(Wikipedia\)](https://en.wikipedia.org/wiki/Tree_rotation)

**Drzewa splay:**

* [Drzewo splay \(Wikipedia\)](https://pl.wikipedia.org/wiki/Drzewo_splay)
* [Splay tree rotation \(Stack Exchange\)](https://cs.stackexchange.com/q/1229/8837)
* [Self-Adjusting Binary Search Trees paper \(CMU\)](https://www.cs.cmu.edu/~sleator/papers/self-adjusting.pdf)
* [Splay trees lecture notes \(Berkeley\)](https://people.eecs.berkeley.edu/~jrs/61b/lec/36)

**Drzewa AVL:**

* [AVL tree \(Wikipedia\)](https://en.wikipedia.org/wiki/AVL_tree)
* [AVL trees \(CodesDope\)](https://www.codesdope.com/course/data-structures-avl-trees/)

**Wizualizacje:**

* [Splay tree \(USF\)](https://www.cs.usfca.edu/~galles/visualization/SplayTree.html)
* [AVL \(VisuAlgo\)](https://visualgo.net/en/bst?slide=14)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="3.1 Zadania:" %}

{% endtab %}

{% tab title="3.1.1" %}
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

{% tab title="3.1.2" %}
Dane jest drzewo splay o takiej samej strukturze jak drzewo A z zadania 1.

Wykonaj w kolejności następujące operacje:

* znajdź element o wartości `30`,
* znajdź element o wartości `50`,
* wstaw element o wartości `25`,
* wstaw element o wartości `22`,
* usuń element o wartości `50`,
* usuń element o wartości `25`.
{% endtab %}

{% tab title="3.1.3" %}
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

{% hint style="info" %}
Przykładowe implementacje omawianych kopców dostępne są w [repozytorium z materiałami do przedmiotu](https://github.com/karolpiczak-pw/2019Z-AISDI/tree/master/examples/04-heaps).
{% endhint %}

### 4.1 Kopce

{% tabs %}
{% tab title="4.1 Zakres materiału" %}
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

{% tab title="4.1 Materiały pomocnicze" %}
{% hint style="info" %}
**Ogólne:**

* [Priority queue ADT \(Wikipedia\)](https://en.wikipedia.org/wiki/Priority_queue)
* [Heap \(Wikipedia\)](https://en.wikipedia.org/wiki/Heap_%28data_structure%29)
* [Implicit data structure \(Wikipedia\)](https://en.wikipedia.org/wiki/Implicit_data_structure)

**Kopiec binarny:**

* [Binary heap \(Wikipedia\)](https://en.wikipedia.org/wiki/Binary_heap)
* [Building a heap in O\(n\) time \(Stack Overflow\)](https://stackoverflow.com/questions/9755721/how-can-building-a-heap-be-on-time-complexity)
* [Binary heap \(Brilliant\)](https://brilliant.org/wiki/binary-heap/)

**Kopce** _**d**_**-arne:**

* [D-ary heap \(Wikipedia\)](https://en.wikipedia.org/wiki/D-ary_heap)
* [Binary heap vs d-ary heap \(Stack Overflow\)](https://stackoverflow.com/questions/29126428/binary-heaps-vs-d-ary-heaps)
* [Ternary and quaternary heaps \(Stack Overflow\)](https://stackoverflow.com/questions/48843677/why-dont-we-use-ternary-or-quaternary-heaps)

**Kopiec dwumianowy:**

* [Binomial heap \(Wikipedia\)](https://en.wikipedia.org/wiki/Binomial_heap)
* [Binomial heap \(Brilliant\)](https://brilliant.org/wiki/binomial-heap/)
* [Binomial heap \(Growing with the Web\)](https://www.growingwiththeweb.com/data-structures/binomial-heap/overview/)

**Kopiec Fibonacciego:**

* [Fibonacci heap \(Wikipedia\)](https://en.wikipedia.org/wiki/Fibonacci_heap)
* [Fibonacci heap \(Brilliant\)](https://brilliant.org/wiki/fibonacci-heap/)
* [Fibonacci heap lecture notes \(Princeton\)](https://www.cs.princeton.edu/~wayne/teaching/fibonacci-heap.pdf)

**Wizualizacje:**

* [Heap \(VisuAlgo\)](https://visualgo.net/en/heap)
* [Heap \(USF\)](https://www.cs.usfca.edu/~galles/visualization/Heap.html)
* [Binomial heap \(USF\)](https://www.cs.usfca.edu/~galles/visualization/BinomialQueue.html)
* [Fibonacci heap \(USF\)](https://www.cs.usfca.edu/~galles/visualization/FibonacciHeap.html)
{% endhint %}
{% endtab %}
{% endtabs %}

{% tabs %}
{% tab title="4.1 Zadania:" %}

{% endtab %}

{% tab title="4.1.1" %}
Zapisz w reprezentacji tablicowej drzewo binarne następującej postaci:

![](../../.gitbook/assets/tree%20%283%29.png)
{% endtab %}

{% tab title="4.1.2" %}
Dla zapisu tablicowego:

`[95, 80, 85, 40, 70, 90, 50, 30, 10, 20]`

narysuj zupełne drzewo binarne. Czy drzewo to przedstawia kopiec typu _max-heap_?
{% endtab %}

{% tab title="4.1.3" %}
Do pustego **kopca binarnego** _**max-heap**_ wstaw w kolejności elementy o wartościach klucza:

`43, 24, 11, 47, 13, 67, 59, 95, 29, 17, 54, 40`

Następnie trzykrotnie wykonaj operację usunięcia największego elementu z kopca.

Zilustruj stan kopca po każdym kroku.
{% endtab %}

{% tab title="4.1.4" %}
Z podanej tablicy stwórz **kopiec binarny typu** _**max-heap**_ metodą Floyda \(przywracanie własności kopca kolejnym poddrzewom\):

`[2, 7, 26, 25, 19, 17, 1, 90, 3, 36]`

Zlicz ilość wykonanych operacji, porównaj z metodą tworzenia kopca przez wstawianie.
{% endtab %}

{% tab title="4.1.5" %}
Do pustego **kopca 3-arnego \(**_**ternary heap**_**\) typu** _**max-heap**_ _\*\*_wstaw w kolejności elementy o wartościach klucza:

`43, 24, 11, 47, 13, 67, 59, 95, 29, 17, 54, 40`

Następnie trzykrotnie wykonaj operację usunięcia największego elementu z kopca.

Zilustruj stan kopca po każdym kroku.
{% endtab %}

{% tab title="4.1.6" %}
Do pustego **kopca dwumianowego typu** _**min-heap**_ wstaw w kolejności elementy o wartościach klucza:

`43, 24, 11, 47, 13, 67, 59, 95, 29, 17, 54, 40`

Następnie trzykrotnie wykonaj operację usunięcia najmniejszego elementu z kopca.

Zilustruj stan kopca po każdym kroku.
{% endtab %}

{% tab title="4.1.7" %}
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

