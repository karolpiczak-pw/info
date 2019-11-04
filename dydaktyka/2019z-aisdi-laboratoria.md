---
description: Algorytmy i struktury danych - zajęcia laboratoryjne
---

# 2019Z-AISDI - laboratoria

## Prowadzone grupy

* grupa 108, piątki parzyste, 8:15-10:00
* grupa 106, piątki parzyste, 10:15-12:00

## Organizacja zajęć

Laboratoria polegają na rozwiązywaniu przedstawionych zadań w zespołach dwuosobowych. Łącznie za laboratoria do zdobycia jest 30 punktów, po 6 punktów za zadania realizowane na zajęciach 2-6. Do implementacji wykorzystywany jest język C++.

| Lp. | Tematyka zajęć | Ocenianie |
| :--- | :--- | :--- |
| 1 | zajęcia wstępne, zapoznanie ze środowiskiem | - |
| 2 | sortowanie | 6 pkt. |
| 3 | drzewa | 6 pkt. |
| 4 | kopce | 6 pkt. |
| 5 | wyszukiwanie wzorca w tekście | 6 pkt. |
| 6 | grafy | 6 pkt. |
| 7 | termin rezerwowy \(oddawanie zaległych zadań\) | - |

## Kryteria oceniania

| Punktacja | Wymagania względem rozwiązania |
| :--- | :--- |
| 6 pkt. | poprawne i kompletne rozwiązanie zadania |
| 5 pkt. | rozwiązanie kompletne z niewielkimi uchybieniami \(wydajność, przypadki skrajne\) |
| 4 pkt. | nieliczne błędy implementacyjne o większym znaczeniu, schemat rozwiązania poprawny i kompletny, rozwiązanie wykazuje zrozumienie materiału |
| 3 pkt. | realizacja części zadania, liczne błędy w implementacji |
| 2 pkt. | realizacja małej części zadania, liczne błędy w implementacji |
| 1 pkt | realizacja minimalnego zakresu funkcjonalności, bardzo liczne błędy w implementacji |
| 0 pkt. | brak zgłoszonego rozwiązania |

{% hint style="info" %}
Styl kodu oceniany jest w sposób binarny: **akceptowalny \(0\)**, **niewystarczający \(-1\)**.
{% endhint %}

{% hint style="info" %}
Poprawki wprowadzone do rozwiązania po zajęciach mogą podnieść punktację co najwyżej o 2 punkty.
{% endhint %}

{% hint style="danger" %}
Błędy dostępu do pamięci \(odwoływanie się do nieważnego wskaźnika\) traktowane są zawsze jako błędy o większym znaczeniu.
{% endhint %}

## Zasady zgłaszania rozwiązań do oceny

* Rozwiązania zadań laboratoryjnych muszą zostać zaprezentowane na konsultacjach prowadzącemu, do którego są Państwo przypisani w systemie USOS. Grupy mieszane mogą wybrać prowadzącego. Drugim prowadzącym laboratoria jest Waldemar Grabski.
* Przy prezentacji zadania powinien być obecny cały zespół.
* Na konsultacje należy zapisać się w [kalendarzu](https://calendly.com/karolpiczak/) \(terminy udostępniane są na najbliższe dwa tygodnie\).
* Przy zapisywaniu się należy podać link do repozytorium na [wydziałowym GitLabie](https://gitlab-stud.elka.pw.edu.pl/) ze zgłoszonym _merge request_ sporządzonym według dalszych instrukcji.
* Zadania można zdawać do ostatnich zajęć laboratoryjnych. Proszę jednak uwzględnić mniejszą dostępność terminów pod koniec semestru.

{% hint style="info" %}
Na pojedynczych konsultacjach możliwe jest ocenienie więcej niż jednego zadania, z tym że będzie to zależało od ilości uwag i dostępnego czasu. Zwłaszcza w takim przypadku proszę o wcześniejszy kontakt - część uwag postaram się przekazać na zasadzie code review przez GitLab.
{% endhint %}

## Udostępnianie rozwiązań przez GitLab

* Dostęp do [wydziałowego serwisu GitLab](https://gitlab-stud.elka.pw.edu.pl/) możliwy jest po zalogowaniu się za pomocą danych wydziałowych \(LDAP\).
* Rozwiązanie należy sporządzać w prywatnym repozytorium zawierającym w nazwie dane członków zespołu \(`nazwisko1-nazwisko2`, małymi literami\).
* Repozytorium powinno zawierać co najmniej dwie gałęzie - roboczą i pustą \(np. `master` i `grade`\).
* Po zakończeniu prac nad zadaniem należy:
  * udostępnić repozytorium prowadzącemu \([@karolpiczak](https://gitlab-stud.elka.pw.edu.pl/karolpiczak) lub [@wgrabski](https://gitlab-stud.elka.pw.edu.pl/wgrabski)\) z [uprawnieniami](https://docs.gitlab.com/ee/user/permissions.html) na poziomie `Developer`,
  * [utworzyć nowy _merge request_](https://docs.gitlab.com/ee/gitlab-basics/add-merge-request.html) z gałęzi roboczej do gałęzi pustej \(np. `master -> grade`\),
  * zatytułować _merge request_ jako `Lab X: Nazwisko1-Nazwisko2`, gdzie `X` jest numerem zajęć,
  * przydzielić tak utworzony _merge request_ prowadzącemu \(jako `Assignee`\).

