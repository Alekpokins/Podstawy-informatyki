# Topologie Sieci

## Sieci Fizyczne
Sieci fizyczne odnoszą się do fizycznego ułożenia kabli, urządzeń i połączeń. Przykłady:

- **Topologia magistrali** (Bus): Jest to topologia, w której wszystkie urządzenia są podłączone do jednej linii transmisyjnej (kabel). Dane wysyłane przez jedno urządzenie przechodzą przez całą magistralę, aż dotrą do celu.

  - **Wady**:
    - Awaria kabla głównego przerywa całą sieć.
    - Ograniczona przepustowość, szczególnie przy dużej liczbie urządzeń.
    - Trudność w diagnozowaniu problemów.

  - **Zalety**:
    - Prosta w instalacji i tania.
    - Mniejsza liczba kabli w porównaniu do innych topologii.
    - Łatwość w rozbudowie sieci.

  - **Gdzie stosowane**:
    - Stosowana głównie w starszych sieciach LAN.
    - Małe biura, mniejsze instalacje.

---

- **Topologia pierścienia** (Ring): Jest to topologia, w której urządzenia są połączone w zamknięty pierścień, a dane przesyłane są w jednym kierunku przez wszystkie urządzenia, aż dotrą do celu.

  - **Wady**:
    - Awaria jednego urządzenia lub kabla przerywa całą sieć.
    - Trudność w naprawie sieci w przypadku problemów.
    - Wysoka latencja przy większej liczbie urządzeń.

  - **Zalety**:
    - Wydajna w małych sieciach.
    - Brak kolizji danych, ponieważ tylko jedno urządzenie może nadawać w danym czasie.

  - **Gdzie stosowane**:
    - Starsze technologie sieciowe, takie jak Token Ring.
    - Stosowane w sieciach wymagających synchronizacji danych.

---

- **Topologia gwiazdy** (Star): Jest to topologia, w której każde urządzenie jest połączone bezpośrednio z centralnym urządzeniem, takim jak koncentrator (hub) lub przełącznik (switch).

  - **Wady**:
    - Zależność od centralnego urządzenia — awaria koncentratora lub switcha przerywa całą sieć.
    - Wyższe koszty rozbudowy w porównaniu do innych topologii.

  - **Zalety**:
    - Łatwa w instalacji i rozbudowie.
    - Wysoka niezawodność — awaria jednego urządzenia nie wpływa na inne.

  - **Gdzie stosowane**:
    - Nowoczesne sieci LAN w biurach, szkołach, domach.
    - W sieciach o dużej liczbie urządzeń, gdzie centralny punkt zarządzający ułatwia kontrolę.

---

## Sieci Logiczne
Sieci logiczne opisują sposób przesyłania danych między urządzeniami, niezależnie od fizycznej struktury. Przykłady:

- **Punkt-punkt** (Point-to-Point): Jest to topologia, w której dwa urządzenia są bezpośrednio połączone i komunikują się ze sobą bez pośredników.

  - **Wady**:
    - Ograniczona do połączenia tylko dwóch urządzeń.
    - Wymaga dedykowanego połączenia, które może być kosztowne, gdy urządzenia są w dużej odległości.

  - **Zalety**:
    - Prosta w konfiguracji i instalacji.
    - Niska latencja, ponieważ dane nie muszą przechodzić przez inne urządzenia.

  - **Zastosowanie**:
    - Połączenia między dwoma routerami w sieciach WAN.
    - Połączenia między komputerami, np. przy połączeniu Ethernetowym bezpośrednio.

---

- **Przekazywanie żetonu** (Token Passing): Jest to metoda dostępu do medium transmisyjnego, w której tylko urządzenie posiadające specjalny token (żeton) może nadawać dane. Token krąży po sieci, przekazując prawo do transmisji.

  - **Wady**:
    - Jeśli token zostanie zagubiony lub zablokowany, cała sieć przestaje działać.
    - Wymaga synchronizacji urządzeń, co może być złożone do zarządzania w dużych sieciach.

  - **Zalety**:
    - Minimalizuje ryzyko kolizji, ponieważ tylko jedno urządzenie może nadawać w danym czasie.
    - Gwarantowana kontrola dostępu do medium transmisyjnego.

  - **Zastosowanie**:
    - Stosowane w sieciach Token Ring.
    - Sieci wymagające synchronizacji transmisji danych.

---

- **Wielodostępowa** (Multiple Access): W tej topologii wiele urządzeń ma dostęp do wspólnego medium transmisyjnego. W przypadku kolizji danych urządzenia muszą retransmitować dane, aby uniknąć konfliktów.

  - **Wady**:
    - Kolizje w sieci powodują opóźnienia w transmisji.
    - Wydajność sieci spada wraz z liczbą urządzeń korzystających z medium.

  - **Zalety**:
    - Prosta instalacja, niskie koszty.
    - Łatwość w rozbudowie sieci przez dodanie nowych urządzeń.

  - **Zastosowanie**:
    - Sieci Ethernet, zwłaszcza w starszych konfiguracjach.
    - Sieci bezprzewodowe, w których urządzenia dzielą ten sam kanał transmisyjny.
