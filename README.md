# Sunly — strona-wizytówka (rekrutacja testerów)

Statyczna strona do zapraszania testerów apki mobilnej **Sunly**, wzorowana na sprawdzonym
`canaryeclipse` (`release/site`). Jasny motyw, 4 języki (EN/ES/PL/DE), formularz zapisu na test,
galeria zrzutów z lightboxem. Hostowana za darmo na **GitHub Pages** z własną domeną.

> To osobny projekt od apki (`../canaryweather`) i od SaaS (`../sunly-saas`). Trzy różne rzeczy:
> apka mobilna · strona-wizytówka (tu) · biznes B2B.

## Podgląd lokalny
Otwórz `index.html` w przeglądarce (dwuklik) — działa bez serwera.

## ⚠️ Do uzupełnienia PRZED publikacją (placeholdery w index.html)

Wyszukaj i podmień w `index.html`:

1. ~~`REPLACE_WEB3FORMS_ACCESS_KEY`~~ — ZROBIONE: klucz `22400fe2-…` (zgłoszenia → Gmail trzcinskib@).
2. ~~`REPLACE_PRIVACY_URL`~~ — ZROBIONE: wstawiony link Notion (×5).
3. ~~`REPLACE_DOMAIN`~~ — ZROBIONE: `og:url` = `https://app.sunly.live`, plik `CNAME` = `app.sunly.live`.
   E-mail „Contact" na stronie = `info@sunly.live` (⚠️ ustaw przekierowanie tej skrzynki, żeby działał).
4. *(opcjonalnie)* `REPLACE_GOATCOUNTER` — darmowa analityka bez ciasteczek; albo usuń ten blok.

## Architektura domen (jedna domena `sunly.live` + subdomeny)
- **`app.sunly.live`** → TA strona (pobieranie apki przez testerów). ← tu jesteśmy
- **`widget.sunly.live`** → projekt `sunly-saas` (widżet B2B), później.
- **`sunly.live`** (główna) → przyszła apka webowa Sunly + hub „pobierz", później.

Subdomeny są DARMOWE — kupujesz tylko jedną domenę `sunly.live` i tworzysz rekordy DNS.

## Zrzuty ekranu
- Placeholdery są w `screens/en/` (01-search … 06-rain). **Podmień na prawdziwe** zrzuty Sunly
  (te same nazwy plików). Masz 6 angielskich zrzutów z opisu sklepu — wystarczą na start.
- Języki: strona bierze `screens/<pl|es|de|en>/<nazwa>.png`, a gdy brak — **wraca do `screens/en/`**.
  Czyli wystarczy `screens/en/`; wersje pl/es/de dodasz kiedyś opcjonalnie.

## Wdrożenie (GitHub Pages, jak w canaryeclipse)
1. Utwórz repo na GitHub (np. `sunly-site`) i wypchnij tę zawartość (jest już plik `CNAME` = `app.sunly.live`).
2. Kup domenę **`sunly.live`** (sprawdź dostępność u rejestratora — whois było niepewne).
3. GitHub → Settings → Pages → Source = gałąź `main`, katalog `/`. Domena `app.sunly.live` podepnie się z `CNAME`; włącz „Enforce HTTPS".
4. W DNS domeny `sunly.live` dodaj rekord **CNAME**: host `app` → wartość `bartek666.github.io`.
   (Subdomena = tylko rekord CNAME, bez rekordów A/AAAA. Prościej niż domena główna.)
5. Później analogicznie: `widget` → hosting SaaS; domena główna `sunly.live` → apka webowa.

## Jak działa zapis testera (potok)
1. Osoba wpisuje swój **Gmail** w formularzu → web3forms wysyła Ci maila z tym adresem.
2. W **Play Console → Testowanie → Test zamknięty → Testerzy** dodajesz ten Gmail do listy.
3. Google/Ty wysyła jej **link opt-in** → instaluje Sunly z Google Play.
4. (Do zbierania zaangażowania: patrz `../canaryweather/docs/testers-engagement-plan.md`.)

## Uwaga
Strona = **nie** pełna apka webowa (ta jest odłożona do czasu produkcji). To lekka wizytówka,
którą wklejasz w postach na FB, żeby link wyglądał wiarygodnie i miał instrukcję w jednym miejscu.
Później stanie się stroną marketingową produktu.
