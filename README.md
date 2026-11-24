# PawMade Games – strona

Statyczna strona (HTML + CSS) pod GitHub Pages: strona główna, polityka prywatności PL/EN i `app-ads.txt`.

## Pliki

| Plik | Do czego |
|---|---|
| `index.html` | strona główna studia i gry |
| `privacy.html` / `privacy-pl.html` | polityka prywatności (EN / PL) |
| `app-ads.txt` | weryfikacja sprzedawcy reklam AdMob, musi leżeć w katalogu głównym |
| `assets/style.css` | wspólny wygląd |

## Do uzupełnienia przed publikacją

Wszystko oznaczone na stronach żółtym tłem (`[...]`) to miejsca do uzupełnienia:

- dane wydawcy (nazwa, adres) i adres e-mail kontaktowy,
- okres przechowywania danych i region BigQuery,
- granica wieku w polityce to 16 lat: ustaw ocenę wiekową i grupę docelową w sklepach spójnie z tym,
- linki do sklepów, gdy gra będzie live,
- przycisk „Privacy settings" w grze (polityka mówi, że istnieje).

Polityka jest szkicem, nie poradą prawną. Przed publikacją niech ją sprawdzi ktoś, kto zna RODO.

## `app-ads.txt`

Linia w pliku to wydawca z konta AdMob (`pub-…`). Dokładną linię sprawdź w AdMob → Apps → app-ads.txt i porównaj. Plik musi być dostępny pod `https://TWOJA-DOMENA/app-ads.txt`, a ta sama domena musi być wpisana jako strona dewelopera w App Store i Google Play.

## Wdrożenie na GitHub Pages

1. Nowe repozytorium na GitHubie (np. `pawmade-games-site`), wrzuć do niego te pliki.
2. Settings → Pages → Source: gałąź `main`, katalog `/ (root)`.
3. Po minucie strona działa pod adresem pokazanym w ustawieniach.
4. Własna domena: dodaj ją w Settings → Pages → Custom domain (GitHub utworzy plik `CNAME`) i ustaw rekordy DNS według instrukcji GitHuba.
5. W AdMob wpisz adres polityki (`https://…/privacy.html`) przy obu aplikacjach.
