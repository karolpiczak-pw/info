---
description: Algorytmy i struktury danych - ćwiczenia
---

# 2019Z-AISDI - ćwiczenia

## Prowadzone grupy

* grupa 102, wtorki nieparzyste, 12:15-14:00
* grupa 103, wtorki parzyste, 12:15-14:00
* grupa 105, wtorki parzyste, 14:15-16:00

## Organizacja zajęć

Zajęcia odbywają się co dwa tygodnie. W ramach ćwiczeń do zdobycia jest 20 punktów:

* 15 punktów - kolokwium,
* 5 punktów - aktywność, prezentacje, zadania domowe.

Punkty za aktywność przyznawane są za rozwiązywanie zadań w trakcie zajęć, aktywny udział w dyskusji lub prezentację algorytmu \(do zdobycia jeden punkt na spotkanie\). Dodatkowo można zgłaszać rozwiązania zadań domowych. Maksymalnie można zgłosić trzy zadania domowe do oceny \(każde za jeden punkt\). 

| Lp. | Tematyka zajęć |
| :--- | :--- |
| 1 | lista, drzewo wyszukiwania binarnego \(_BST_\) |
| 2 | algorytmy sortowania |
| 3 | drzewa AVL, drzewa Splay |
| 4 | kopce |
| 5 | **kolokwium** |
| 6 | wyszukiwanie wzorca w tekście - prezentacje |
| 7 | algorytmy grafowe - prezentacje |

## Zasady zgłaszania zadań domowych

Rozwiązania zadań należy zgłaszać przez udostępnienie repozytorium na wydziałowym serwerze GitLab i przydzielenie _merge request_ [prowadzącemu](https://gitlab-stud.elka.pw.edu.pl/karolpiczak), analogicznie do [zasad na laboratoriach](https://pw.karolpiczak.com/dydaktyka/2019z-aisdi-laboratoria#udostepnianie-rozwiazan-przez-gitlab). _Merge request_ proszę zatytułować  `HW X: Nazwisko`.

**Termin na zgłaszanie zadań:** do kolokwium

{% hint style="info" %}
Dopuszczalne są implementacje w językach C++, Python, Java.
{% endhint %}

{% hint style="warning" %}
Rozwiązanie powinno również zawierać przynajmniej podstawowy zakres testów weryfikujących poprawność implementacji.
{% endhint %}

### Zadanie \#1

Zaimplementuj operację usuwania węzła z drzewa wyszukiwania binarnego.

### Zadanie \#2

Zaimplementuj program, który:

* wygeneruje losową permutację standardowej talii kart \(52 karty\),
* posortuje uzyskany ciąg kart w porządku rosnącym \(od dwójki do asa\) w sposób

  stabilny \(wejściowa kolejność kolorów zachowana\) wykorzystując algorytm

  _selection sort_ i strukturę listy.

{% hint style="info" %}
Sugerowane oznaczenia kolorów:  **S**♠  **H**♥  **D**♦  **C**♣ ****
{% endhint %}

