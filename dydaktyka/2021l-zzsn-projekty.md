---
description: Zaawansowane zagadnienia sieci neuronowych - projekty
---

# 2021L-ZZSN - projekty

## Prowadzone grupy

* grupa 101
* grupa 102
* grupa 103
* grupa 104

## Organizacja zajęć

Część projektowa zajęć z _Zaawansowanych zagadnień sieci neuronowych_ polega na implementacji zaawansowanych modeli sieci neuronowych nawiązujących do tematów omawianych na wykładzie.

Projekty realizowane są w zespołach dwuosobowych. Celem projektu jest rozwiązanie problemu o charakterze użytkowym lub badawczym i jednoczesne zrozumienie danego zagadnienia przez zespół. Oznacza to, że przy realizacji można się posiłkować publicznymi implementacjami, ale nie zwalnia to zespołu z przygotowania się do dokładnego wytłumaczenia zasady działania prezentowanego rozwiązania.

Projekty powinny być realizowane w języku _Python 3.8+_ z wykorzystaniem biblioteki _PyTorch,_ ewentualnie _TensorFlow_. Sugerowanym podejściem do ustrukturyzowania kodu jest wykorzystanie biblioteki _PyTorch Lightning_. __Szkielet takiego rozwiązania zostanie udostępniony w późniejszym okresie.

Dodatkowe informacje udostępniane będą na bieżąco w zespole MS Teams przedmiotu.

### Zasady oceniania

Za część projektową można uzyskać łącznie 35 punktów:

* dokumentacja wstępna - 5 punktów, 
* implementacja modelu - 15 punktów,
* dokumentacja końcowa i prezentacja projektu - 15 punktów.

Dokumentacja wstępna powinna zawierać opis zadania, przewidywany sposób rozwiązania problemu i wyjaśnienie poczynionych założeń \(typ modelu, wybrane zbiory danych, narzędzia, zakładana funkcjonalność itp.\).

W ramach implementacji, poza zrealizowaną funkcjonalnością i zakresem eksperymentów, oceniana jest przede wszystkim jakość i czytelność wygenerowanego kodu. Kod powinien dać się uruchomić po postawieniu środowiska _conda_ według pliku _environment.yml_ z repozytorium \(w wyjątkowych przypadkach obraz z _Dockerfile_\). Mile widziane są adnotacje typowania statycznego i podstawowy zakres testów adekwatny do specyfiki testowania projektów machine learningowych, ale elementy te nie są wymagane do uzyskania maksymalnej liczby punktów, jeżeli nie ma żadnych innych zastrzeżeń.

W dokumentacji końcowej należy zawrzeć opis rozwiązania ze zwięzłym wyjaśnieniem kontekstu danego zagadnienia lub zasady działania modelu, wyniki eksperymentów i wnioski po realizacji projektu.

Dokumentację i kod źródłowy należy umieścić w repozytorium _git_ dedykowanym dla zespołu \(dokładne informacje na kanale MS Teams\).

Niejasności można wyjaśniać poprzez MS Teams lub na konsultacjach \(po [zapisaniu się](https://calendly.com/karolpiczak/)\).

### Harmonogram

Wyszczególnione daty oznaczają termin na koniec dnia \(23:59\). Przez dostarczenie materiałów rozumiany jest _commit_ w udostępnionym przeze mnie repozytorium dedykowanym dla projektu.

<table>
  <thead>
    <tr>
      <th style="text-align:left">Data</th>
      <th style="text-align:left">Etap realizacji</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">19.03.2021 (pi&#x105;tek)</td>
      <td style="text-align:left">Zg&#x142;oszenie sk&#x142;ad&#xF3;w zespo&#x142;&#xF3;w wraz z preferencjami
        temat&#xF3;w
        <br />(prosz&#x119; do&#x142;&#x105;czy&#x107; loginy na GitHubie)</td>
    </tr>
    <tr>
      <td style="text-align:left">22.03.2021 (poniedzia&#x142;ek)</td>
      <td style="text-align:left">Przydzia&#x142; temat&#xF3;w do zespo&#x142;&#xF3;w</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>16.04.2021 (pi&#x105;tek)</b>
      </td>
      <td style="text-align:left">Dostarczenie dokumentacji wst&#x119;pnej</td>
    </tr>
    <tr>
      <td style="text-align:left"><b>2.06.2021 (&#x15B;roda)</b>
      </td>
      <td style="text-align:left">Dostarczenie kodu &#x17A;r&#xF3;d&#x142;owego i dokumentacji ko&#x144;cowej</td>
    </tr>
    <tr>
      <td style="text-align:left">7-11.06.2021</td>
      <td style="text-align:left">Prezentacje i ocena projekt&#xF3;w</td>
    </tr>
    <tr>
      <td style="text-align:left">16.06.2021 (&#x15B;roda)</td>
      <td style="text-align:left">
        <p>Ostateczny termin na oddanie projektu z kar&#x105; -10 punkt&#xF3;w</p>
        <p>(po tym terminie projekty nie b&#x119;d&#x105; oceniane)</p>
      </td>
    </tr>
  </tbody>
</table>

## Tematy projektów

| Lp. | Temat |
| :--- | :--- |
| 1 | **Zmiana pogody na zdjęciach za pomocą transferu stylu** |
| 2 | **Generowanie twarzy postaci z filmów animowanych za pomocą sieci GAN** |
| 3 | **Detekcja maseczek ochronnych na zdjęciach z wykorzystaniem detektora YOLO** |
| 4 | **Usuwanie tła za pomocą sieci typu U-Net** |
| 5 | **Segmentacja zdjęć lotniczych za pomocą sieci typu U-Net** |
| 6 | **Wykorzystanie sieci impulsowej do klasyfikacji dźwięku** |
| 7 | **Przeciwstawne uczenie ciągłe klasyfikatorów dźwiękowych** |
| 8 | **Rezydualne uczenie ciągłe klasyfikatorów obrazowych** |
| 9 | **Wyszukiwanie efektywnych podsieci w klasyfikatorze danych dźwiękowych** |
| 10 | **Wykorzystanie sieci kapsułkowych do klasyfikacji chmur punktów** |
| 11 | **Predykcja liczby zachorowań na COVID-19 za pomocą grafowych sieci czasowo-przestrzennych** |
| 12 | **Analiza wydźwięku depesz giełdowych za pomocą modelu typu BERT** |
| 13 | **Wykorzystanie architektury typu** _**Music Transformer**_ **do generowania dzwonków telefonicznych** |
| 14 | **Wykorzystanie uczenia samonadzorowanego do poprawy klasyfikacji dźwięku** |
| 15 | **Uczenie klasyfikatorów dźwiękowych niewielką liczbą przykładów z wykorzystaniem sieci prototypowych** |
| ? | _Możliwe tematy własne po konsultacji_ |

### **Omówienie tematów**

#### **1. Zmiana pogody na zdjęciach za pomocą transferu stylu**

{% hint style="info" %}
Celem projektu jest stworzenie narzędzia do konwersji zdjęcia z pochmurną pogodą na zdjęcie ze słoneczną pogodą.

**Schemat sugerowanego rozwiązania:**

* Pobranie obrazków z kamer internetowych \(np. [_webcamgalore.com_](https://www.webcamgalore.com/)\) z różnych momentów w czasie \(_timelapse_\).
* Wykorzystanie gotowego klasyfikatora pogody do oznaczenia zdjęcia jako pochmurne/słoneczne \(ewentualnie adnotacja ręczna\).
* Stworzenie sieci GAN do transferu stylu pochmurnie → słonecznie.
* Porównanie z uczeniem na zdjęciach, które nie pochodzą z tego samego ujęcia \(np. [Two-Class Weather Classification](http://www.cse.cuhk.edu.hk/leojia/projects/weatherclassify/index.htm)\).


{% endhint %}

**2. Generowanie twarzy postaci z filmów animowanych za pomocą sieci GAN**

{% hint style="info" %}
Celem projektu jest stworzenie narzędzia ****do generowania twarzy postaci kreskówkowych przy wykorzystaniu sieci GAN.

**Przykładowy zbiór danych:** [**iCartoonFace**](https://github.com/luxiangju-PersonAI/iCartoonFace)**,** ewentualnie [**Cartoon Set**](https://google.github.io/cartoonset/index.html)\*\*\*\*

Minimalny zakres to generowanie bezwarunkowe \(dowolna twarz\), ciekawsze rozwiązanie powinno uwzględniać możliwość sterowania charakterem generowanego obrazu.
{% endhint %}

**3. Detekcja maseczek ochronnych na zdjęciach z wykorzystaniem detektora YOLO**

{% hint style="info" %}
Celem projektu jest stworzenie detektora działającego w trybie real-time, który na zdjęciu z kamery oznaczy osoby z maseczkami ochronnymi i bez maseczek.

**Przykładowe zbiory danych:** [**Kaggle**](https://www.kaggle.com/datasets?search=face+mask)\*\*\*\*

W ramach podsumowania proszę przetestować działanie detektora na własnym filmie z kamery internetowej \(ewentualnie zdjęciach z telefonu\) albo na wybranym streamie dostępnym publicznie.
{% endhint %}

**4. Usuwanie tła za pomocą sieci typu U-Net**

{% hint style="info" %}
Celem projektu jest stworzenie narzędzia do usuwania/podmiany tła na zdjęciu twarzy.

**Przykładowy zbiór danych:** [**Matting Human Datasets**](https://www.kaggle.com/laurentmih/aisegmentcom-matting-human-datasets)

W ramach podsumowania proszę przetestować działanie narzędzia na własnych zdjęciach z telefonu lub filmie z kamery internetowej i porównać np. z rozmyciem dostępnym w MS Teams, Google Meet.

Do rozwiązania można też wykorzystać inne podejście niż wykorzystanie sieci U-Net.
{% endhint %}

**5. Segmentacja zdjęć lotniczych za pomocą sieci typu U-Net**

{% hint style="info" %}
Celem projektu jest stworzenie narzędzia do segmentacji zdjęć lotniczych wykorzystującego sieć typu U-Net.

**Przykładowy zbiór danych:** [**Aerial Semantic Segmentation Drone Dataset**](https://www.kaggle.com/bulentsiyah/semantic-drone-dataset)\*\*\*\*

W ramach podsumowania proszę przetestować działanie narzędzia na [mapach lotniczych Warszawy](http://mapa.um.warszawa.pl/mapaApp1/mapa?service=mapa).
{% endhint %}

**6. Wykorzystanie sieci impulsowej do klasyfikacji dźwięku**

{% hint style="info" %}
Celem projektu jest implementacja kilku wariantów prostych architektur sieci impulsowej i porównanie ich działania na zbiorze wizyjnym [_MNIST_](http://yann.lecun.com/exdb/mnist/) __oraz zbiorze dźwiękowym [_ESC-50/ESC-10._](https://github.com/karolpiczak/ESC-50)\_\_

**Sugerowany framework do implementacji:** [**BindsNET**](https://github.com/BindsNET/bindsnet)\*\*\*\*

Ze względu na eksperymentalny charakter zagadnienia osiągnięta dokładność klasyfikacji nie jest kryterium oceny jakości projektu, liczy się poprawność implementacji.
{% endhint %}

**7. Przeciwstawne uczenie ciągłe klasyfikatorów dźwiękowych**

{% hint style="info" %}
Celem projektu jest implementacja metody uczenia ciągłego określanej jako [_adversarial continual learning_](https://arxiv.org/pdf/2003.09553.pdf) i weryfikacja jej działania w kontekście klasyfikacji dźwięku \(np. na [ESC-50](https://github.com/karolpiczak/ESC-50), [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html) lub [FSD50K](https://zenodo.org/record/4060432#.YEo4u2hKiMo)\).

W ramach podsumowania proszę porównać efektywność tego podejścia z wybraną metodą typu regularyzacyjnego i metodą typu _replay_.
{% endhint %}

**8. Rezydualne uczenie ciągłe klasyfikatorów obrazowych**

{% hint style="info" %}
Celem projektu jest implementacja metody uczenia ciągłego określanej jako [_residual continual learning_](https://arxiv.org/pdf/2002.06774.pdf) i weryfikacja jej działania w kontekście klasyfikacji obrazów \(np. na CIFAR-10/CIFAR-100\).

W ramach podsumowania proszę porównać efektywność tego podejścia z wybraną metodą typu regularyzacyjnego i metodą typu _replay_.
{% endhint %}

**9. Wyszukiwanie efektywnych podsieci w klasyfikatorze danych dźwiękowych**

{% hint style="info" %}
Celem projektu jest przebadanie działania metody [_early bird tickets_](https://github.com/RICE-EIC/Early-Bird-Tickets) do szybkiego wyszukiwania efektywnych podsieci w klasyfikatorach dźwiękowych \(np. o architekturze zbliżonej do OpenL3\).

W ramach podsumowania proszę zweryfikować dokładność działania modelu bazowego i podsieci typu _lottery ticket_ na wybranych zbiorach z zakresu klasyfikacji dźwięku \(np. [ESC-50](https://github.com/karolpiczak/ESC-50), [UrbanSound8K](https://urbansounddataset.weebly.com/urbansound8k.html), [FSD50K](https://zenodo.org/record/4060432#.YEo4u2hKiMo) lub [innych](http://dcase.community/)\).
{% endhint %}

**10. Wykorzystanie sieci kapsułkowych do klasyfikacji chmur punktów**

{% hint style="info" %}
Celem projektu jest zastosowanie sieci kapsułkowych do klasyfikacji chmur punktów.

W ramach zadania wstępnego proszę sprawdzić działanie sieci kapsułkowej na zbiorze obrazowym \(np. CIFAR-10\).

W ramach podsumowania proszę porównać działanie sieci kapsułkowej z innym modelem \(np. [PointNet++](http://stanford.edu/~rqi/pointnet2/)\) w zadaniu klasyfikacji chmur punktów \(np. [ShapeNetCore](https://shapenet.org/)\).
{% endhint %}

**11. Predykcja liczby zachorowań na COVID-19 za pomocą grafowych sieci czasowo-przestrzennych**

{% hint style="info" %}
Celem projektu jest zastosowanie [czasowo-przestrzennej grafowej splotowej sieci neuronowej](https://arxiv.org/pdf/1709.04875.pdf) do predykcji liczby zachorowań na COVID-19 dla [danych ze Stanów Zjednoczonych](https://github.com/nytimes/covid-19-data) \(podział na hrabstwa\).

W ramach podsumowania proszę porównać działanie modelu z predykcjami prostych lokalnych modeli autoregresyjnych oraz zweryfikować poprawność implementacji na [zbiorze benchmarkowym zachorowań na ospę](https://pytorch-geometric-temporal.readthedocs.io/en/latest/modules/dataset.html#torch_geometric_temporal.data.dataset.chickenpox.ChickenpoxDatasetLoader).

Do implementacji zalecane jest wykorzystanie biblioteki [PyTorch Geometric Temporal](https://github.com/benedekrozemberczki/pytorch_geometric_temporal).

W przypadku tego projektu bardzo pożądanym elementem jest wizualizacja predykcji na mapie, np. za pomocą [Streamlit](https://docs.streamlit.io/en/stable/api.html#streamlit.map).
{% endhint %}

**12. Analiza wydźwięku depesz giełdowych za pomocą modelu typu BERT**

{% hint style="info" %}
Celem projektu jest wykorzystanie polskiego modelu typu BERT \(np. [Herbert](https://huggingface.co/allegro/herbert-large-cased) albo [Polbert](https://huggingface.co/dkleczek/bert-base-polish-cased-v1)\) do oceny wydźwięku \(_negatywny/neutralny/pozytywny_\) depesz na polskiej Giełdzie Papierów Wartościowych.

**Schemat sugerowanego rozwiązania:**

* Wykorzystanie modelu wstępnie trenowanego na korpusie języka polskiego do zadania analizy wydźwięku, np. na zbiorze [PolEmo2.0-IN](https://klejbenchmark.com/tasks/#polemo2.0-in). Porównanie działania modelu przy zmianie dziedziny \([PolEmo2.0-OUT](https://klejbenchmark.com/tasks/#polemo2.0-out)\).
* Stworzenie bazy danych z [raportów systemu ESPI](http://infostrefa.com/infostrefa/pl/raporty/espi/biezace,0,0,0,1). Adnotacją wydźwięku generowaną syntetycznie może być następująca po komunikacie nadmiarowa zmiana [kursu akcji spółki](https://www.quandl.com/data/WSE-Warsaw-Stock-Exchange-GPW) w stosunku do zmiany szerokiego rynku.
* Weryfikacja działania modelu bez uczenia na danych z dziedziny finansowej i po wykorzystaniu raportów do dotrenowywania.
{% endhint %}

**13. Wykorzystanie architektury typu** _**Music Transformer**_ **do generowania dzwonków telefonicznych**

{% hint style="info" %}
Celem projektu jest stworzenie modelu o architekturze [_Music Transformer_](https://magenta.tensorflow.org/music-transformer), którego zadaniem jest generowanie krótkich fragmentów muzycznych o charakterze dzwonka telefonicznego.

**Schemat sugerowanego rozwiązania:**

* Przygotowanie zbioru [plików MIDI](https://github.com/albertmeronyo/awesome-midi-sources) o charakterze adekwatnym dla potencjalnego zastosowania.
* Wyuczenie modelu na przygotowanym zbiorze danych pod kątem bezwarunkowego generowania sekwencji MIDI i warunkowanego krótkim fragmentem początkowym.
* Przetworzenie wygenerowanych sekwencji do postaci dźwiękowej za pomocą syntezy offline \(np. [NSynth](https://magenta.tensorflow.org/datasets/nsynth)\), wybranego odtwarzacza MIDI w JavaScript albo wykorzystania wybranego [syntezatora VSTi](https://www.kvraudio.com/plugins/instruments/windows/macosx/linux/vst-plugins/free/most-popular) \(np. przez [RenderMan](https://github.com/fedden/RenderMan)\).
{% endhint %}

**14. Wykorzystanie uczenia samonadzorowanego do poprawy klasyfikacji dźwięku**

{% hint style="info" %}
Celem projektu jest wyuczenie modelu rozumienia dźwięku w sposób samonadzorowany na zbiorze danych nieetykietowanych, np. wzorując się na podejściu [SimCLR](https://github.com/google-research/simclr) lub [MoCo](https://github.com/facebookresearch/moco). Tak wyuczony model należy następnie wykorzystać do klasyfikacji spektrogramów z mniejszego zbioru etykietowanego i porównać dokładność klasyfikacji z modelem uczonym w standardowy sposób \(w pełni nadzorowany, tylko na zbiorze etykietowanym\), ewentualnie przeanalizować odporność obydwu modeli na złośliwe modyfikacje typu _adversarial attacks_.

**Przykładowe zbiory danych:** [**ESC-US**](https://dataverse.harvard.edu/dataset.xhtml?persistentId=doi:10.7910/DVN/YDEPUT) i [**ESC-50**](https://github.com/karolpiczak/ESC-50)\*\*\*\*

Ze względu na większą złożoność obliczeniową technik samonadzorowanych wyniki podsumowania można oprzeć na modelu wyuczonym częściowo. Jeżeli sama implementacja i wytłumaczenie zespołu będzie bez zastrzeżeń, to nie wpływa to na końcową ocenę. W takim wypadku zalecałbym sprawdzenie implementacji na zbiorze CIFAR-10.
{% endhint %}

**15. Uczenie klasyfikatorów dźwiękowych niewielką liczbą przykładów z wykorzystaniem sieci prototypowych**

{% hint style="info" %}
Celem projektu jest stworzenie modelu [sieci protytypowej](https://arxiv.org/pdf/1703.05175.pdf) do uczenia klasyfikatorów dźwiękowych niewielką liczbą przykładów \(_few-shot learning_\).

**Schemat sugerowanego rozwiązania:**

* Stworzenie standardowego klasyfikatora dźwiękowego \(np. na podstawie architektury [OpenL3](https://openl3.readthedocs.io/)\) i wyuczenie go na zbiorze danych [FSD50K](https://annotator.freesound.org/fsd/release/FSD50K/).
* Sprawdzenie dokładności klasyfikacji przy standardowym uczeniu \(bez ograniczeń na liczbę przykładów per klasa\).
* Ocena tego samego modelu w uczeniu z ograniczoną liczbą przykładów \(np. połowa klas dostępna normalnie, połowa tylko po $$K=5$$ przykładów uczących\).
* Porównanie z działaniem modelu sieci prototypowej dla różnych wartości $$K$$ .
{% endhint %}

## Zalecenia zbiorcze

Poza raportem końcowym dobrze byłoby, gdyby w ramach rozwiązania można zrozumieć i sprawdzić działanie modelu na przykładach, najlepiej w sposób interaktywny.

Sugerowanym narzędziem do tego typu prostych podsumowań jest [Streamlit](https://www.streamlit.io/), ewentualnie [Dash](http://dash.plotly.com/) lub inne rozwiązania tego typu.

### Zasoby obliczeniowe

Do realizacji projektów można wykorzystać darmowe zasoby obliczeniowe:

* [Google Colab](https://colab.research.google.com/)
* [Kaggle Code](https://www.kaggle.com/code)
* [Azure for Students](https://azure.microsoft.com/pl-pl/free/students/)
* [gradient](https://docs.paperspace.com/gradient/instances/instance-types/free-instances)

Jeżeli uda się pozyskać grant edukacyjny na przedmiot, to dostępne będą dodatkowo kupony do wykorzystania w _Google Cloud_.

W szczególnych przypadkach \(np. uczenie samonadzorowane\) możliwe jest też przydzielenie zasobów z puli uczelnianej.

{% hint style="warning" %}
W zależności od wymagań projektu i dostępnych mocy obliczeniowych uczenie modeli może zająć dłuższy czas \(liczony w dniach\). Proszę uwzględnić ten fakt przy rozplanowywaniu harmonogramu prac.
{% endhint %}



