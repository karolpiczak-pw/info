---
description: Zakres materiału obowiązującego na kolokwium
---

# Kolokwium

## Ćwiczenia \#1

### **Tablica, std::array, std::vector**

{% tabs %}
{% tab title="Zakres materiału" %}
* podstawowe operacje i ich złożoność:
  * dostęp,
  * wstawianie elementu \(na końcu/w środku\),
  * usuwanie elementu \(z końca/ze środka\),
  * wyszukiwanie elementu o określonej wartości
* różnica między `std::vector::size()` a `std::vector::capacity()`,
* wykorzystanie iteratorów
{% endtab %}
{% endtabs %}

### **Lista jedno- i dwukierunkowa**

{% tabs %}
{% tab title="Zakres materiału" %}
* podstawowe operacje i ich złożoność:
  * dostęp,
  * wstawianie elementu,
  * usuwanie elementu,
  * wyszukiwanie elementu o określonej wartości
* wyszukiwanie ze strażnikiem
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
{% tab title="Przykładowe zadania:" %}
\*\*\*\*
{% endtab %}

{% tab title="\#1" %}
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

{% tab title="\#2" %}
Zaimplementuj metodę, która dla listy jednokierunkowej zwróci trzeci element od końca. Załóż, że długość listy nie jest znana.
{% endtab %}

{% tab title="\#3" %}
Zaimplementuj metodę, która zwróci środkowy element listy jednokierunkowej. Załóż, że długość listy nie jest znana.
{% endtab %}

{% tab title="\#4" %}
Zaproponuj sposób odwracania listy jednokierunkowej w jednym przejściu bez tworzenia kopii wszystkich elementów.
{% endtab %}

{% tab title="\#5" %}
Zaproponuj sposób usuwania węzła mając tylko odwołanie do niego. Załóż, że nie jest to ostatni węzeł listy.
{% endtab %}

{% tab title="\#6" %}
Zaimplementuj uproszczony iterator \(tylko operacje `->` i `++` \) po elementach listy. Jak wyglądałby taki iterator, gdyby miał zwracać najpierw elementy na rosnących pozycjach nieparzystych listy, a następnie na parzystych?
{% endtab %}
{% endtabs %}

### **Kolejka \(FIFO\), stos \(LIFO\)**

{% tabs %}
{% tab title="Zakres materiału" %}
* pojęcie abstrakcyjnego typu danych \(_abstract data type, ADT_\),
* kolejka i stos jako przykłady ADT,
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
* drzewo binarne, definicja, podstawowe własności,
* binarne drzewo poszukiwań \(_binary search tree_, _BST_\):
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
{% tab title="Przykładowe zadania:" %}

{% endtab %}

{% tab title="\#1" %}
Narysuj binarne drzewo poszukiwań utworzone przez wstawienie w kolejności elementów:

`31, 72, 23, 44, 85, 106, 17, 28, 9, 30, 41`
{% endtab %}

{% tab title="\#2" %}
Zaimplementuj metody wstawiania i wyszukiwania węzła w drzewie BST.
{% endtab %}

{% tab title="\#3" %}
Zaimplementuj rekursywne przechodzenie po węzłach drzewa w kolejności "in-order".
{% endtab %}

{% tab title="\#4" %}
Zaimplementuj uproszczony iterator \(tylko operacje `->` i `++` \), który będzie przechodził węzły drzewa w kolejności "in-order".
{% endtab %}

{% tab title="\#5" %}
Zaimplementuj w klasie drzewa BST funkcjonalność usuwania węzła o zadanej wartości.
{% endtab %}
{% endtabs %}

## Ćwiczenia \#2

### Algorytmy sortowania

{% tabs %}
{% tab title="Zakres materiału" %}
**Algorytmy:**

* sortowanie przez wybieranie \(_selection sort_\),
* sortowanie przez wstawianie \(_insertion sort_\),
* sortowanie bąbelkowe \(_bubble sort_\),
* sortowanie szybkie \(_quicksort_\),
* sortowanie przez scalanie \(_merge sort_\),
* sortowanie przez kopcowanie \(_heapsort_\),
* sortowanie kubełkowe \(_bucket sort_\)

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

## Ćwiczenia \#3

### Drzewa

{% tabs %}
{% tab title="Zakres materiału" %}
* drzewa BST zrównoważone i niezrównoważone,
* rotacje drzew,
* drzewa splay:
  * implementacja i złożoność obliczeniowa:
    * operacja _splay_,
    * wyszukiwanie elementu,
    * wstawianie elementu,
    * usuwanie elementu,
  * zastosowania drzewa splay, zalety i wady
* drzewa AVL:
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
{% tab title="Przykładowe zadania:" %}

{% endtab %}

{% tab title="\#1" %}
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

{% tab title="\#2" %}
Dane jest drzewo splay o takiej samej strukturze jak drzewo A z zadania \#1.

Wykonaj w kolejności następujące operacje:

* znajdź element o wartości `30`,
* znajdź element o wartości `50`,
* wstaw element o wartości `25`,
* wstaw element o wartości `22`,
* usuń element o wartości `50`,
* usuń element o wartości `25`.
{% endtab %}

{% tab title="\#3" %}
Stwórz drzewo AVL przez wstawianie kolejno wartości:

`10, 20, 30, 40, 50, 60, 70`

Na stworzonym drzewie przeprowadź operacje:

* wstaw element o wartości `55`,
* wstaw element o wartości `52`,
* usuń element o wartości `52`,
* usuń element o wartości `70`.
{% endtab %}
{% endtabs %}

## Ćwiczenia \#4

