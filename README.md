# ChatGPT Google Forms MCP — strony informacyjne

**Status:** publiczne, statyczne strony informacyjne hostowane w GitHub Pages.

- [Strona główna (PL)](https://wjedrzejewski-tech.github.io/google-forms-mcp-pages/)
- [Polityka prywatności (PL)](https://wjedrzejewski-tech.github.io/google-forms-mcp-pages/privacy.html)
- [About the integration (EN)](https://wjedrzejewski-tech.github.io/google-forms-mcp-pages/en/)
- [Privacy policy (EN)](https://wjedrzejewski-tech.github.io/google-forms-mcp-pages/en/privacy.html)

Witryna służy wyłącznie informowaniu o integracji konta `rciittzut@gmail.com` używanego na potrzeby RCIiTT ZUT. **Nie jest to oficjalna strona uczelni ani publiczna usługa Google Forms.**

Pliki: `index.html`, `privacy.html`, `en/index.html`, `en/privacy.html`, `assets/logo-google-forms-mcp-512.png`, `assets/logo-google-forms-mcp-120.png`, `.nojekyll`.

- Logo 512 × 512 jest wyświetlane na stronach; mały wariant 120 × 120 służy jako ikona witryny.
- Polska strona główna zachowuje znacznik Google Search Console. Właściciel potwierdził weryfikację witryny 18.11.2026 r.
- Google OAuth nadal wymaga odrębnej ponownej weryfikacji marki. Samo działanie GitHub Pages nie potwierdza statusu `In production`.
- Repozytorium **nie może** zawierać kodu chronionego Workera, danych formularzy, sekretów ani tokenów.
- Przetwarzanie rzeczywistych danych respondentów pozostaje poza zakresem obecnego pilotażu do czasu odrębnej oceny i zatwierdzenia.
- Wdrażanie: GitHub Pages z gałęzi `main`, katalog `/` (root), bez własnych workflow CI.

Utrzymanie: zmiany w HTML muszą zachować poprawne linki PL/EN oraz znacznik weryfikacyjny Google na stronie głównej.

## Ograniczenie indeksowania

Wszystkie cztery strony HTML (`index.html`, `privacy.html`, `en/index.html`, `en/privacy.html`) zawierają dyrektywę `<meta name="robots" content="noindex, noarchive, nosnippet, noimageindex">`. Ma ona ograniczać obecność stron w wynikach wyszukiwania Google, Bing i innych usług, które przestrzegają tej reguły. Nie stosować `Disallow` w `robots.txt` dla tych stron: wyszukiwarka musi móc odczytać dyrektywę `noindex`.

Witryna i kod strony nadal są publicznie dostępne przez bezpośredni adres, co jest potrzebne do Google OAuth. `noindex` nie jest ochroną dostępu, nie gwarantuje niewidoczności we wszystkich wyszukiwarkach i nie blokuje indeksowania publicznego repozytorium GitHub. Jeśli strony zostały już zindeksowane, usunięcie ich z wyników wymaga ponownego odwiedzenia przez wyszukiwarkę, ewentualnie zgłoszenia usunięcia przez narzędzie operatora wyszukiwarki.
