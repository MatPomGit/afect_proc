# Informatyka Afektywna

Interaktywny kurs edukacyjny z zakresu informatyki afektywnej (Affective Computing).

## Opis projektu

Projekt stanowi webową platformę edukacyjną opartą na systemie prezentacji z integracją LMS (Learning Management System). Wykorzystuje architekturę Module Federation do dynamicznego ładowania komponentów.

## Struktura projektu

```
.
├── index.html              # Główny punkt wejścia aplikacji
├── goodbye.html            # Strona końcowa/wyjściowa
├── assets/                 # Zasoby graficzne
│   ├── VF9f8IYqh3DML6vx.jpg
│   └── small.png
└── lib/                    # Biblioteki i moduły
    ├── player-0.0.11.min.js    # Główna biblioteka odtwarzacza
    ├── lzwcompress.js          # Narzędzie kompresji
    ├── icomoon.css             # System ikon
    ├── fonts/                  # Czcionki (Inter, Lato, Poppins, Icomoon)
    ├── rise/                   # Główne moduły aplikacji
    ├── learn_dist/             # Moduły federacyjne learn_distribution
    ├── mondrian/               # Moduły federacyjne mondrian
    └── sandbox/                # Środowisko piaskownicy
```

## Wymagania

- Przeglądarka internetowa z obsługą HTML5 i JavaScript ES6+
- Opcjonalnie: środowisko LMS wspierające standardy xAPI/SCORM

## Uruchomienie

### Lokalne uruchomienie

1. Otwórz plik `index.html` w przeglądarce internetowej
2. Alternatywnie, uruchom lokalny serwer HTTP:

```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (jeśli zainstalowano http-server)
npx http-server -p 8000
```

3. Otwórz przeglądarkę i przejdź do `http://localhost:8000`

### Integracja z LMS

Projekt wspiera następujące tryby uruchomienia:
- `raw` - tryb podstawowy (domyślny)
- `review` - tryb przeglądu
- `tincan` - integracja z Tin Can API
- `xapi` - integracja z xAPI (Experience API)

## Funkcjonalności

- Dynamiczne ładowanie modułów z wykorzystaniem Module Federation
- Kompresja i dekompresja danych kursu
- Wsparcie dla różnych czcionek (Inter, Lato, Poppins)
- System ikon Icomoon
- Integracja z systemami LMS

## Tryby uruchomienia

Aplikacja sprawdza środowisko uruchomienia i dostosowuje się do niego:
- Tryb standalone (plik lokalny)
- Tryb iframe (osadzony w LMS)
- Tryb z wykrywaniem LMS

## Technologie

- HTML5
- JavaScript (ES6+)
- CSS3
- Module Federation (Webpack)
- LZW Compression

## Licencja

Projekt edukacyjny.

## Autor

MatPomGit
