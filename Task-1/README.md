# Task 1 – Użyteczność serwisów internetowych (3. zajęcia)

| Zadanie | Plik | Zakres |
|---|---|---|
| 1 | [zadanie-1-nowa-aplikacja.md](zadanie-1-nowa-aplikacja.md) | Poznawanie nowej aplikacji (Obsidian) bez dokumentacji: oczekiwana funkcjonalność, 3 zadania (model koncepcyjny), proces nauki i emocje |
| 2 | [zadanie-2-gov-pl.md](zadanie-2-gov-pl.md) | Ocena użyteczności serwisu www.gov.pl: wyszukiwanie 4 spraw urzędowych, heurystyki Nielsena, porównanie z wynikami generatywnej AI |
| 3 | [zadanie-3-lotniska.md](zadanie-3-lotniska.md) | Porównanie serwisów 3 lotnisk: Warszawa-Chopin (PL), Monachium (EU), Singapur-Changi (poza Europą) + obiektywne miary |

## Metodyka (wspólna dla zadań 2 i 3)

- Przeglądanie serwisów od strony głównej, bez zewnętrznych wyszukiwarek (w zadaniu 2 zgodnie z poleceniem).
- Liczba kliknięć liczona od strony głównej do strony z odpowiedzią (rozwinięcie menu po najechaniu kursorem nie jest liczone jako kliknięcie).
- Trudność w skali 1–5 (1 = bardzo łatwo, 5 = nie udało się znaleźć).
- Pomiary techniczne (czas odpowiedzi, rozmiar HTML, obrazy bez atrybutu `alt`) wykonane narzędziem `curl` dla strony głównej w statycznym HTML (bez treści doładowywanej przez JavaScript).
- Data badania: **19.10.2026**. Serwisy zmieniają się, więc wyniki dotyczą stanu z tego dnia.

## Najważniejsze wnioski

1. **gov.pl** dobrze sprawdza się w sprawach typowych, opisanych jako „usługa” (prawo jazdy: 3 kliknięcia). Słabo radzi sobie w sprawach, które nie pasują do jego kategorii (EKUZ jest w „Wyjazdach”, a nie w „Zdrowiu”) i z informacjami z pogranicza administracji rządowej i samorządowej (stawki za odpady: nie udało się znaleźć). Strona programu „Mój prąd” jest nieaktualna od 2023 r., a nadal ma aktywny przycisk „Złóż wniosek”.
2. Najczęściej łamane heurystyki Nielsena na gov.pl: **#2** (zgodność z rzeczywistością), **#4** (spójność), **#9** (pomoc w rozpoznawaniu błędów: błędny adres przekierowuje bez komunikatu na stronę główną) oraz **#1** (widoczność stanu: nieaktualne treści bez ostrzeżenia).
3. Generatywna AI szybko podaje poprawne odpowiedzi w sprawach stabilnych (prawo jazdy). W sprawach zmiennych (Mój Prąd, EKUZ od 2026, stawki za odpady) zdarza się, że odpowiedź jest nieaktualna lub niespójna. Ocena heurystyczna wykonana przez AI bez dostępu do serwisu jest ogólnikowa.
4. Lotniska: najlepszą **nawigację** ma Monachium (parking w menu głównym, „Accessible travel” jako skrót na stronie głównej). Najbardziej **szczegółowe treści transportowe** ma Changi (taryfy taksówek, pierwsze i ostatnie pociągi MRT). Najlepsze **informacje dla osób z niepełnosprawnościami** ma Warszawa-Chopin. Wynik łączny według zaproponowanych miar jest w [zadaniu 3](zadanie-3-lotniska.md#4-wynik-łączny).
