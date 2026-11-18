# PowerCalc

Program do obliczeń instalacji elektrycznych niskiego napięcia wg PN-HD 60364, PN-EN 60909-0 i N SEP-E-002:
bilans mocy, dobór kabli i zabezpieczeń, prądy zwarciowe, samoczynne wyłączenie zasilania, selektywność, źródła
(transformator, agregat, UPS) i sieci DC. Raporty: PDF oraz Excel z działającymi formułami.

## Pobieranie i instalacja

1. Pobierz plik `PowerCalc-<wersja>-win64.zip` z zakładki **Releases** (po prawej stronie).
2. Rozpakuj go w dowolnym miejscu, np. `C:\Programy\PowerCalc`.
3. Uruchom `PowerCalc.exe`. Program nie wymaga instalacji ani uprawnień administratora.

Wymagania: Windows 10 lub 11, 64-bit.

**Ostrzeżenie Windows SmartScreen** („System Windows ochronił ten komputer”) pojawia się, bo program nie ma płatnego
podpisu cyfrowego. Kliknij **Więcej informacji → Uruchom mimo to**.

## Ważność wydania

Każde wydanie działa do daty podanej przy uruchomieniu (ok. 6 miesięcy). 30 dni przed końcem program przypomina
o nowej wersji. Po terminie pobierz aktualne wydanie z tej strony. Projekty (`.elproj`) otwierają się w nowszych
wersjach bez zmian.

## Ważne

- Wyniki obliczeń sprawdza projektant z uprawnieniami – program wspomaga obliczenia, nie zastępuje projektanta.
- Tabele selektywności producentów nie są dołączone. Do oceny selektywności wpisz wartości z dokumentacji
  producenta aparatów; bez nich program ocenia selektywność metodami zastępczymi (bezpieczniki gG 1:1,6,
  porównanie charakterystyk t-I).
- Wkładki gG liczone są z bramek PN-EN 60269-1 (bez danych katalogowych producenta) – czasy wyłączania i całka
  Joule'a są po stronie bezpiecznej. Dokładniejsze wartości wpisz z karty producenta.
- Katalog zawiera tylko aparaty ogólne (wartości normowe i typowe), bez serii konkretnych producentów. Zdolność
  wyłączalną i nastawy wybranego aparatu wpisz z jego karty katalogowej.
- Brak danych ogniw baterii stacyjnych – przed doborem baterii DC wpisz krzywe rozładowania i typoszereg ogniw
  z karty producenta (Katalogi → Edytor katalogów: „bateria_kt”, „baterie”).
- Program wolno używać na warunkach pliku `LICENCJA.txt`. Nie udostępniaj go dalej – inne osoby pobierają
  program z tej strony.

## Błędy i uwagi

Zgłaszaj w zakładce **Issues** tego repozytorium: opis, kroki do powtórzenia i – jeśli możesz – plik projektu
oraz dziennik błędów `%LOCALAPPDATA%\PowerCalc\powercalc.log`.
