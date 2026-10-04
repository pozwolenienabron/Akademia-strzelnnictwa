AKADEMIA STRZELECTWA 8.0.0

Lekka aplikacja web/PWA do nauki teorii patentu strzeleckiego.

URUCHOMIENIE
1. Rozpakuj ZIP w całości.
2. Otwórz index.html.
3. Aplikacja nie wymaga lokalnego serwera do uruchomienia podstawowych funkcji.

ANDROID
- Możesz otworzyć index.html w przeglądarce lub uruchomić aplikację z serwera HTTPS.
- Przy HTTPS/PWA dostępna jest instalacja na ekranie głównym i działanie offline.

LAPTOP
- Dwuklik index.html jest obsługiwany.
- Nie jest wymagane python -m http.server.
- Jeśli uruchamiasz przez lokalny serwer, aplikacja również działa.

DANE
- Baza 205 pytań i lekcji jest wbudowana lokalnie w data.js.
- Aplikacja nie pobiera pytań ani lekcji przez fetch(), dzięki czemu zwykłe file:// nie blokuje startu.
- Postępy są zapisywane lokalnie w IndexedDB z fallbackiem do localStorage.

PWA
- Service Worker działa tylko w bezpiecznym kontekście HTTP/HTTPS.
- Przy zwykłym file:// funkcje PWA mogą być niedostępne, ale sama aplikacja działa.

AKTUALNOŚĆ
Regulamin patentowy PZSS obowiązujący od 1 lipca 2025 r. oraz tekst jednolity przyjęty uchwałą nr 47 z 26 września 2025 r. należy sprawdzać na oficjalnej stronie PZSS.
Pytania w aplikacji są materiałem treningowym i nie są przedstawiane jako kompletna oficjalna baza egzaminacyjna PZSS.

WERSJA
8.0.0 — 5 października 2026


FINAL 8.0: samodzielny index.html. CSS, JavaScript i baza pytań są wbudowane, więc dwuklik na index.html działa bez lokalnego serwera i bez fetch().


OSTATNI AUDYT 8.0: poprawiono Service Worker/PWA. Cache nie odwołuje się już do usuniętych plików, ma nową wersję cache i poprawnie czyści poprzednie cache przy aktualizacji.
