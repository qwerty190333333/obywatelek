# Wersja statyczna dla GitHub Pages

Ta paczka została uporządkowana do hostowania na GitHub Pages.

## Co zostało zmienione
- usunięto katalog `functions/`, ponieważ GitHub Pages nie obsługuje funkcji serwerowych,
- poprawiono `index.html`, aby otwierał istniejącą stronę `gen.html`,
- wyłączono sprawdzanie sesji przez `/api/session-check`,
- dodano plik `.nojekyll`.

## Jak opublikować
1. Rozpakuj archiwum.
2. Wgraj **zawartość tego folderu** do głównego katalogu repozytorium GitHub.
3. Upewnij się, że `index.html` znajduje się bezpośrednio w głównym katalogu repozytorium.
4. Wejdź w `Settings` → `Pages`.
5. Ustaw:
   - Source: `Deploy from a branch`
   - Branch: `main`
   - Folder: `/(root)`
6. Zapisz i poczekaj na publikację.

Uwaga: GitHub Pages obsługuje tylko strony statyczne. Elementy wymagające backendu/API muszą działać po stronie przeglądarki albo zostać przeniesione na hosting obsługujący funkcje serwerowe.
