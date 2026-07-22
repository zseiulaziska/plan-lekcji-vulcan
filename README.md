# Plan lekcji - Zespół Szkół

Plan lekcji publikowany z programu **Plan lekcji Optivum** (VULCAN) z nowoczesnym, responsywnym stylowaniem.

## Struktura

| Katalog | Opis |
|---------|------|
| `plany/` | Plany lekcji: `o*.html` (oddziały), `n*.html` (nauczyciele), `s*.html` (sale) |
| `css/` | Arkusze stylów (automatycznie nadpisywane przez GitHub Actions) |
| `scripts/` | Skrypty JS (nawigacja, druk) |
| `images/` | Obrazy (logo VULCAN) |

## GitHub Actions — automatyczny deploy

Po pushu nowych planów z Optivum, GitHub Actions automatycznie:

1. **Przywraca nowoczesne style** — kopiuje wzorcowe CSS z `.github/styles/` do `css/`
2. **Dodaje meta viewport** — wstrzykuje `<meta name="viewport">` do HTML dla responsywności
3. **Deployuje na GitHub Pages** — publikuje poprawioną wersję jako stronę WWW

⚠️ **Ważne**: workflow **nie modyfikuje** brancha `main` — deploy idzie na GitHub Pages.  
Dzięki temu nie ma konfliktów przy kolejnych publikacjach z Optivum.

## Konfiguracja GitHub Pages

1. Wejdź w **Settings → Pages** swojego repozytorium
2. W sekcji **Source** wybierz **GitHub Actions**
3. Gotowe — przy następnym pushu strona zaktualizuje się automatycznie

## Modyfikacja wyglądu

Wzorcowe pliki CSS znajdują się w `.github/styles/` — edytuj je, a zmiany zostaną zastosowane przy następnym deployu.

