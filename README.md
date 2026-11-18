# ChatGPT Google Forms MCP - strony informacyjne (projekt)

**Status: do przeglądu. Nie włączać GitHub Pages przed zatwierdzeniem treści.**

Repozytorium ma zawierać wyłącznie publiczne pliki statyczne: `index.html`, `privacy.html` i `.nojekyll`.
Nie wolno zamieszczać tu kodu serwera MCP, tokenów OAuth, sekretów, kluczy ani danych formularzy.

## Zastosowanie

Witryna opisuje integrację Google Forms MCP przeznaczoną do obsługi konta
`rciittzut@gmail.com` na potrzeby RCIiTT ZUT. Nie należy przedstawiać jej jako prywatnej
aplikacji osobistej ani oficjalnej witryny uczelni.

## Przed publikacją

1. Potwierdzić, kto formalnie odpowiada za integrację, dane i wskazany kontakt; ustalić wymagane uprawnienia organizacyjne.
2. Zweryfikować opis przechowywania i usuwania danych uwierzytelniających w Cloudflare KV.
3. Zatwierdzić strony i upewnić się, że nie zawierają informacji poufnych.
4. Dopiero potem udostępnić repozytorium publicznie i włączyć GitHub Pages z `main` / `(root)`.
5. Zweryfikować adres strony w Google Search Console (URL-prefix); osobno sprawdzić wymogi OAuth dotyczące domeny strony i callbacku Workera.
6. Nie przełączać Google OAuth na `In production`, dopóki wymagania Google i kontrola ochrony danych nie zostaną spełnione.

Planowany adres po upublicznieniu repozytorium:
`https://wjedrzejewski-tech.github.io/google-forms-mcp-pages/`

Google może zażądać weryfikowalnej domeny także dla przekierowania OAuth w Cloudflare Workers.
Sama witryna na GitHub Pages nie gwarantuje akceptacji domeny.

## Hosting

Docelowo GitHub Pages: `Settings > Pages > Deploy from a branch > main > /(root) > Save`.
Nie trzeba tworzyć własnego workflow CI do budowania HTML.