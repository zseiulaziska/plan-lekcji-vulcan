# Plan lekcji - Zespół Szkół

Plan lekcji publikowany z programu **Plan lekcji Optivum** (VULCAN) z nowoczesnym, responsywnym stylowaniem.

## Struktura

| Katalog | Opis |
|---------|------|
| `plany/` | Plany lekcji: `o*.html` (oddziały), `n*.html` (nauczyciele), `s*.html` (sale) |
| `css/` | Arkusze stylów (automatycznie nadpisywane przez GitHub Actions) |
| `scripts/` | Skrypty JS (nawigacja, druk) |
| `images/` | Obrazy (logo VULCAN) |

## Automatyczna aktualizacja stylów

Po wgraniu nowych planów przez program Optivum, GitHub Actions automatycznie:

1. **Przywraca nowoczesne style** — kopiuje wzorcowe pliki CSS z `.github/styles/` do `css/`
2. **Dodaje meta viewport** — wstrzykuje tag `<meta name="viewport">` do plików HTML dla responsywności na urządzeniach mobilnych

Wzorcowe pliki CSS znajdują się w `.github/styles/` — edytuj je, aby zmienić wygląd.

