# Baza Przewoźników Kolejowych

Lekki, działający w całości po stronie przeglądarki panel zarządczy (dashboard) do obsługi bazy przewoźników kolejowych w Polsce. Narzędzie wspiera proces monitorowania kontaktów handlowych oraz zarządzania zebranymi informacjami z zachowaniem pełnej prywatności danych[cite: 1].

Aplikacja nie wymaga wdrażania środowiska serwerowego ani zewnętrznej bazy danych – funkcjonuje niezależnie, wykorzystując natywne mechanizmy przeglądarek internetowych[cite: 1].

**[Uruchom aplikację on-line](https://mateusz-hub1.github.io/Dashboard-lista-przewoznikow/)**

## Główne funkcjonalności

* **Lokalna persystencja danych (LocalStorage):** Wprowadzane zmiany, w tym modyfikacje statusu realizacji oraz notatki przypisane do konkretnych firm, są automatycznie zapisywane w pamięci lokalnej przeglądarki użytkownika[cite: 1]. Gwarantuje to zachowanie ciągłości pracy bez ryzyka utraty danych po odświeżeniu sesji[cite: 1].
* **Zaawansowane mechanizmy filtrowania:** Moduł pozwala na precyzyjne segmentowanie bazy według priorytetu (kategorie A-E), lokalizacji (województwo) oraz statusu[cite: 1]. Dodatkowo zaimplementowano wielokryteriową wyszukiwarkę tekstową (uwzględniającą m.in. NIP, osobę decyzyjną czy nazwę podmiotu)[cite: 1].
* **Adaptacyjny interfejs:** Możliwość płynnego przełączania widoków pomiędzy interaktywnymi kartami podmiotów a zagęszczonym widokiem tabelarycznym, optymalizującym pracę na dużych zbiorach danych[cite: 1].
* **Generowanie raportów:** Mechanizm eksportu umożliwia pobranie aktualnie wyselekcjonowanego zestawu danych do formatu CSV lub wygenerowanie sformatowanego zestawienia w formacie PDF, gotowego do druku[cite: 1].
* **Moduł analityczny:** Wbudowany panel statystyk na bieżąco przelicza i wizualizuje stopień realizacji celów (np. procent obdzwonionych firm), sygnalizując osiąganie kolejnych kamieni milowych w projekcie[cite: 1].

## Stos technologiczny

Projekt zrealizowano z naciskiem na wysoką wydajność oraz eliminację zewnętrznych zależności (Zero Dependencies):
* **HTML5:** Semantyczna struktura interfejsu[cite: 1].
* **CSS3:** Zoptymalizowany, responsywny układ bazujący na CSS Grid, mechanizmie Flexbox oraz zmiennych CSS[cite: 1].
* **Vanilla JavaScript:** Modułowa obsługa logiki biznesowej, dynamiczne renderowanie interfejsu (DOM manipulation), zarządzanie stanem aplikacji oraz obsługa pamięci przeglądarki[cite: 1].

## Wdrożenie i uruchomienie

Z uwagi na architekturę typu SPA (Single Page Application) bez warstwy backendowej, proces uruchomienia jest trywialny:
1. Sklonuj repozytorium do przestrzeni lokalnej.
2. Otwórz plik `index.html` przy użyciu dowolnej, współczesnej przeglądarki internetowej.
3. Aplikacja natychmiast inicjuje środowisko pracy, ładując ewentualny stan z LocalStorage[cite: 1].
