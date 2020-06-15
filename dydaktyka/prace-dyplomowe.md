---
description: Proponowane tematy prac dyplomowych.
---

# Prace dyplomowe

### \[inż.\] **Aktywne uczenie modeli klasyfikacji dźwięku**

#### Zarys problemu

Uczenie aktywne \([_active learning_](https://en.wikipedia.org/wiki/Active_learning_%28machine_learning%29)\) jest formą uczenia maszynowego, w którym algorytm uczący może interaktywnie pytać użytkownika o etykiety dla wybranych przykładów. Ta forma jest szczególnie użyteczna, gdy dysponujemy zbiorem danych bez adnotacji, a koszt ręcznego etykietowania całego zbioru danych jest zbyt duży. 

#### Cel i etapy pracy

Celem pracy jest stworzenie prostej aplikacji webowej, która umożliwiałaby interaktywne uczenie modelu sztucznej sieci neuronowej, implementacja wybranego modelu klasyfikatora dźwiękowego oraz porównanie technik dobierania przykładów do interaktywnej adnotacji pod kątem uzyskiwanej oszczędności \(liczby etykietowanych przykładów koniecznych do uzyskania oczekiwanej dokładności na zbiorze walidacyjnym\).

#### Wykorzystywane narzędzia

* **Języki programowania:** Python 3.7+, JavaScript/TypeScript
* **Biblioteki ML:** _Pytorch_ lub _TensorFlow_
* **Frameworki:** _Flask_ lub _Django_ \(ewentualnie [_Dash_](https://plotly.com/dash/)\)
* **Repozytorium kodu**: _GitHub.com_ lub zakładowy _GitLab_ 
* **Edycja pracy:** _LaTeX_ \(np. przez [Overleaf.com](https://www.overleaf.com/)\) 
* **Sprzęt:** W ramach zasobów Zakładu Sztucznej Inteligencji dostęp do systemu z GPU GeForce RTX 2080 Super \(Ubuntu\)

### **\[inż.\] Klasyfikacja nagrań dźwiękowych ptaków za pomocą modeli ze skupianiem uwagi**

**Zarys problemu**

Charakterystyczną cechą problemu klasyfikacji gatunków ptaków w nagraniach dźwiękowych jest niewielki udział użytecznego sygnału uczącego \(poszczególnych wokalizacji\) w stosunku do całości nagrania \(zarówno w dziedzinie czasu, jak i częstotliwości\). W takiej sytuacji jednym ze sposobów poprawy efektów uczenia sztucznych sieci neuronowych jest mechanizm skupiania uwagi \([_attention mechanism_](http://akosiorek.github.io/ml/2017/10/14/visual-attention.html)\), który koncentruje sieć na najważniejszych fragmentach nagrania. 

**Cel i etapy pracy**

Celem pracy jest stworzenie systemu rozpoznawania gatunków ptaków w nagraniach dźwiękowych wykorzystującego sieci neuronowe z mechanizmem skupiania uwagi oraz zweryfikowanie działania systemu na przykładowych nagraniach. Potencjalnym rozszerzeniem pracy może być zgłoszenie systemu w cyklicznym konkursie BirdCLEF.

**Wykorzystywane narzędzia**

* **Języki programowania:** Python 3.7+
* **Biblioteki ML:** _Pytorch_ lub _TensorFlow_
* **Repozytorium kodu**: _GitHub.com_ lub zakładowy _GitLab_ 
* **Edycja pracy:** _LaTeX_ \(np. przez [Overleaf.com](https://www.overleaf.com/)\) 
* **Sprzęt:** W ramach zasobów Zakładu Sztucznej Inteligencji dostęp do systemu z GPU GeForce RTX 2080 Super \(Ubuntu\)

