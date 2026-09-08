# Sunly landing — tłumaczenia nowej treści (EN → ES / PL / DE)

Źródło: teksty z redesignu w Claude Design (wrzesień 2026).
Terminologia zgodna z aplikacją (`canaryweather/src/i18n/locales`): sun chance =
Probabilidad de sol / Szansa na słońce / Chance auf Sonne; station = estación
meteorológica / stacja pogodowa / Wetterstation; calima pozostaje „Calima".

Głos marki: prosto, ciepło, bez marketingowego szumu, zdania małą literą, „ty".
Nazwy własne miejsc zostają w pisowni hiszpańskiej we wszystkich językach.

Klucze zgodne z istniejącym wzorcem w `index.html`: `data-key="<klucz>_<lang>"`.

---

## Header / nawigacja

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| nav_destinations | Destinations | Destinos | Miejsca | Reiseziele |
| nav_measures | What it measures | Qué mide | Co mierzy | Was es misst |
| nav_data | The data | Los datos | Dane | Die Daten |
| nav_privacy | Privacy | Privacidad | Prywatność | Datenschutz |
| badge_notracking | No tracking | Sin rastreo | Bez śledzenia | Kein Tracking |
| btn_getapp | Get the app | Descargar la app | Pobierz aplikację | App holen |

---

## Hero

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| hero_badge | 27 AEMET STATIONS · 2016–2025 | 27 ESTACIONES AEMET · 2016–2025 | 27 STACJI AEMET · 2016–2025 | 27 AEMET-STATIONEN · 2016–2025 |
| hero_title | Will it be sunny when you go? | ¿Hará sol cuando vayas? | Czy będzie słonecznie, gdy przyjedziesz? | Wird es sonnig, wenn du fährst? |
| hero_sub | Search a place, pick a month, and Sunly shows the share of days that were actually sunny there — measured at the nearest AEMET station, not forecast. | Busca un lugar, elige un mes y Sunly te muestra el porcentaje de días que realmente fueron soleados allí — medido en la estación AEMET más cercana, no un pronóstico. | Wyszukaj miejsce, wybierz miesiąc, a Sunly pokaże odsetek dni, które naprawdę były słoneczne — zmierzony na najbliższej stacji AEMET, nie prognoza. | Suche einen Ort, wähle einen Monat, und Sunly zeigt dir den Anteil der Tage, die dort wirklich sonnig waren — gemessen an der nächsten AEMET-Station, keine Vorhersage. |
| hero_btn_play | Get it on Google Play | Disponible en Google Play | Pobierz z Google Play | Jetzt bei Google Play |
| hero_ios | iOS coming soon | iOS muy pronto | iOS wkrótce | iOS bald verfügbar |
| chip_free | Free | Gratis | Za darmo | Kostenlos |
| chip_noads | No ads | Sin anuncios | Bez reklam | Keine Werbung |
| chip_noaccounts | No accounts | Sin cuentas | Bez kont | Keine Konten |
| chip_notracking | No tracking | Sin rastreo | Bez śledzenia | Kein Tracking |

---

## How it works

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| how_eyebrow | HOW IT WORKS | CÓMO FUNCIONA | JAK TO DZIAŁA | SO FUNKTIONIERT'S |
| how_heading | Three taps between you and a sunny week | Tres toques entre tú y una semana soleada | Trzy dotknięcia dzielą Cię od słonecznego tygodnia | Drei Tipps zwischen dir und einer sonnigen Woche |
| how_s1_title | Search a place | Busca un lugar | Wyszukaj miejsce | Ort suchen |
| how_s1_body | Or tap "My location". Sunly finds the nearest of 27 AEMET stations. | O toca «Mi ubicación». Sunly encuentra la más cercana de las 27 estaciones AEMET. | Albo dotknij „Moja lokalizacja". Sunly znajdzie najbliższą z 27 stacji AEMET. | Oder tippe auf „Mein Standort". Sunly findet die nächste der 27 AEMET-Stationen. |
| how_s2_title | Pick a month | Elige un mes | Wybierz miesiąc | Monat wählen |
| how_s2_body | Twelve months of historical records — not a forecast. | Doce meses de registros históricos — no un pronóstico. | Dwanaście miesięcy danych historycznych — nie prognoza. | Zwölf Monate historischer Aufzeichnungen — keine Vorhersage. |
| how_s3_title | Read the numbers | Lee los números | Odczytaj liczby | Zahlen ablesen |
| how_s3_body | Sun chance, temperature, wind and rain, with the station named. | Probabilidad de sol, temperatura, viento y lluvia, con la estación indicada. | Szansa na słońce, temperatura, wiatr i deszcz — z podaną stacją. | Chance auf Sonne, Temperatur, Wind und Regen — mit angegebener Station. |

---

## Where Sunly works (destinations)

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| dest_eyebrow | WHERE SUNLY WORKS | DÓNDE FUNCIONA SUNLY | GDZIE DZIAŁA SUNLY | WO SUNLY FUNKTIONIERT |
| dest_heading | The Canaries, the Balearics and the south-east coast | Las Canarias, las Baleares y la costa sureste | Kanary, Baleary i wybrzeże południowo-wschodnie | Die Kanaren, die Balearen und die Südostküste |
| dest_intro | 247 searchable places across the Canaries, the Balearics and the Spanish south-east coast. | 247 lugares que puedes buscar en las Canarias, las Baleares y la costa sureste de España. | 247 miejsc do wyszukania na Kanarach, Balearach i południowo-wschodnim wybrzeżu Hiszpanii. | 247 durchsuchbare Orte auf den Kanaren, den Balearen und an der spanischen Südostküste. |
| group_canary | Canary Islands | Islas Canarias | Wyspy Kanaryjskie | Kanarische Inseln |
| group_balearic | Balearic Islands | Islas Baleares | Baleary | Balearen |
| group_coast | Spanish south-east coast | Costa sureste de España | Południowo-wschodnie wybrzeże Hiszpanii | Spanische Südostküste |
| tile_places | {n} popular places | {n} lugares populares | {n} popularnych miejsc (patrz uwaga PL) | {n} beliebte Orte |

**Uwaga PL (odmiana „miejsce"):** liczby stałe, więc wpiszemy je ręcznie na kaflach.
Zasada: końcówka 2–4 (poza 12–14) → „miejsca"; reszta → „miejsc".
Konkretnie: Teneryfa 61 → „61 popularnych miejsc"; Gran Canaria 41 → „41 popularnych miejsc";
Fuerteventura 27 → „27 popularnych miejsc"; **La Palma 22 → „22 popularne miejsca"**;
Lanzarote 18 → „18 popularnych miejsc"; La Gomera 11 → „11 popularnych miejsc";
El Hierro 10 → „10 popularnych miejsc"; Mallorca/Menorca/Ibiza 7 → „7 popularnych miejsc";
Formentera i każde wybrzeże 6 → „6 popularnych miejsc".
(ES i DE — jedna forma liczby mnogiej dla wszystkich.)

---

## What it measures

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| meas_eyebrow | WHAT IT MEASURES | QUÉ MIDE | CO MIERZY | WAS ES MISST |
| meas_heading | Six things worth knowing before you book | Seis cosas que conviene saber antes de reservar | Sześć rzeczy, które warto wiedzieć przed rezerwacją | Sechs Dinge, die du vor der Buchung wissen solltest |
| meas_intro | Every figure comes from the nearest AEMET station and is named as such in the app. | Cada dato viene de la estación AEMET más cercana, indicada en la app. | Każda liczba pochodzi z najbliższej stacji AEMET — jej nazwa jest podana w aplikacji. | Jede Zahl stammt von der nächsten AEMET-Station, die in der App genannt wird. |
| meas_sun_title | Sun chance | Probabilidad de sol | Szansa na słońce | Chance auf Sonne |
| meas_sun_body | The share of days that were sunny in that month, per station. | El porcentaje de días que fueron soleados ese mes, por estación. | Odsetek dni, które w danym miesiącu były słoneczne — dla każdej stacji. | Der Anteil der Tage, die in dem Monat sonnig waren, je Station. |
| meas_hours_title | Sun hours | Horas de sol | Godziny słońca | Sonnenstunden |
| meas_hours_body | Average hours of sunshine in a day. | Promedio de horas de sol al día. | Średnia liczba godzin słońca w ciągu dnia. | Durchschnittliche Sonnenstunden pro Tag. |
| meas_temp_title | Temperature | Temperatura | Temperatura | Temperatur |
| meas_temp_body | Average high and average low for the month. | Máxima y mínima promedio del mes. | Średnia temperatura maksymalna i minimalna w miesiącu. | Durchschnittliche Höchst- und Tiefstwerte des Monats. |
| meas_wind_title | Wind | Viento | Wiatr | Wind |
| meas_wind_body | Average speed, Beaufort scale and trade-wind stability. | Velocidad media, escala Beaufort y estabilidad de los vientos alisios. | Średnia prędkość, skala Beauforta i stabilność pasatów. | Durchschnittsgeschwindigkeit, Beaufort-Skala und Stabilität der Passatwinde. |
| meas_rain_title | Rain | Lluvia | Deszcz | Regen |
| meas_rain_body | Average precipitation and how many days it rained. | Precipitación media y cuántos días llovió. | Średnie opady i liczba dni z deszczem. | Durchschnittlicher Niederschlag und an wie vielen Tagen es regnete. |
| meas_calima_title | Calima | Calima | Calima | Calima |
| meas_calima_body | Saharan dust episodes recorded at the station. | Episodios de polvo sahariano registrados en la estación. | Epizody pyłu saharyjskiego zarejestrowane na stacji. | An der Station erfasste Saharastaub-Ereignisse. |

---

## The data

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| data_eyebrow | THE DATA | LOS DATOS | DANE | DIE DATEN |
| data_heading | Official records. Nothing invented. | Registros oficiales. Nada inventado. | Oficjalne dane. Nic zmyślonego. | Offizielle Aufzeichnungen. Nichts erfunden. |
| data_body | Every number in Sunly comes from AEMET, Spain's national meteorological agency. We count the days that were sunny and divide. That's the whole method — and you can read it in full. | Cada número de Sunly viene de AEMET, la agencia meteorológica nacional de España. Contamos los días que fueron soleados y dividimos. Ese es todo el método — y puedes leerlo entero. | Każda liczba w Sunly pochodzi z AEMET, hiszpańskiej krajowej agencji meteorologicznej. Liczymy dni, które były słoneczne, i dzielimy. To cała metoda — możesz przeczytać ją w całości. | Jede Zahl in Sunly stammt von AEMET, Spaniens nationalem Wetterdienst. Wir zählen die sonnigen Tage und teilen. Das ist die ganze Methode — und du kannst sie vollständig nachlesen. |
| data_btn_method | Read the method | Leer el método | Poznaj metodę | Methode lesen |
| data_link_stations | Station list | Lista de estaciones | Lista stacji | Stationsliste |
| data_stat_stations | AEMET stations | estaciones AEMET | stacji AEMET | AEMET-Stationen |
| data_stat_years | years of records | años de registros | lat danych | Jahre an Aufzeichnungen |
| data_stat_window | record window | periodo de registro | zakres danych | Erfassungszeitraum |
| data_stat_trackers | trackers | rastreadores | trackery | Tracker |
| data_disclaimer | Sunly is not affiliated with or endorsed by AEMET. | Sunly no está afiliada a AEMET ni cuenta con su respaldo. | Sunly nie jest powiązana z AEMET ani przez nią wspierana. | Sunly ist nicht mit AEMET verbunden und wird nicht von AEMET unterstützt. |

---

## Privacy

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| priv_badge | Privacy first | Privacidad primero | Prywatność przede wszystkim | Datenschutz zuerst |
| priv_heading | We don't want your data. We just have the weather's. | No queremos tus datos. Solo tenemos los del tiempo. | Nie chcemy Twoich danych. Mamy tylko dane o pogodzie. | Wir wollen deine Daten nicht. Wir haben nur die des Wetters. |
| priv_track_title | No tracking | Sin rastreo | Bez śledzenia | Kein Tracking |
| priv_track_body | No analytics SDKs, no ad IDs, no fingerprinting. | Sin SDKs de analítica, sin IDs de anuncios, sin fingerprinting. | Bez SDK analitycznych, bez identyfikatorów reklamowych, bez fingerprintingu. | Keine Analyse-SDKs, keine Werbe-IDs, kein Fingerprinting. |
| priv_acc_title | No account | Sin cuentas | Bez konta | Kein Konto |
| priv_acc_body | Nothing to sign up for. Nothing to delete. | Nada que registrar. Nada que borrar. | Nie ma się do czego rejestrować. Nie ma czego usuwać. | Nichts zum Anmelden. Nichts zum Löschen. |
| priv_ads_title | No ads | Sin anuncios | Bez reklam | Keine Werbung |
| priv_ads_body | Free, and not paid for by your attention. | Gratis, y no lo pagas con tu atención. | Za darmo — i nie płacisz swoją uwagą. | Kostenlos — und nicht mit deiner Aufmerksamkeit bezahlt. |
| priv_link | Read the privacy policy | Leer la política de privacidad | Przeczytaj politykę prywatności | Datenschutzerklärung lesen |

---

## Download CTA

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| cta_heading | Plan your next trip around the sun. | Planea tu próximo viaje alrededor del sol. | Zaplanuj następną podróż wokół słońca. | Plane deine nächste Reise rund um die Sonne. |
| cta_body | Free on Android. No ads, no accounts, no tracking. iOS coming soon. | Gratis en Android. Sin anuncios, sin cuentas, sin rastreo. iOS muy pronto. | Za darmo na Androida. Bez reklam, bez kont, bez śledzenia. iOS wkrótce. | Kostenlos für Android. Keine Werbung, keine Konten, kein Tracking. iOS bald verfügbar. |
| cta_link_privacy | Privacy policy | Política de privacidad | Polityka prywatności | Datenschutzerklärung |
| cta_footnote | Data: AEMET, 2016–2025. Sunly is not affiliated with or endorsed by AEMET. | Datos: AEMET, 2016–2025. Sunly no está afiliada a AEMET ni cuenta con su respaldo. | Dane: AEMET, 2016–2025. Sunly nie jest powiązana z AEMET ani przez nią wspierana. | Daten: AEMET, 2016–2025. Sunly ist nicht mit AEMET verbunden und wird nicht von AEMET unterstützt. |

---

## Footer

| key | EN | ES | PL | DE |
|---|---|---|---|---|
| foot_tagline | Ten years of official AEMET observations, turned into one honest number: your chance of sunshine. | Diez años de observaciones oficiales de AEMET, convertidos en un número honesto: tu probabilidad de sol. | Dziesięć lat oficjalnych obserwacji AEMET zamienionych w jedną uczciwą liczbę: Twoją szansę na słońce. | Zehn Jahre offizieller AEMET-Beobachtungen, verwandelt in eine ehrliche Zahl: deine Chance auf Sonne. |
| foot_free | Free. No ads. No accounts. | Gratis. Sin anuncios. Sin cuentas. | Za darmo. Bez reklam. Bez kont. | Kostenlos. Keine Werbung. Keine Konten. |
| foot_col_data | DATA | DATOS | DANE | DATEN |
| foot_col_legal | LEGAL | LEGAL | PRAWNE | RECHTLICHES |
| foot_getapp | Get the app | Descargar la app | Pobierz aplikację | App holen |
| foot_aemet_sources | AEMET sources | Fuentes de AEMET | Źródła AEMET | AEMET-Quellen |
| foot_how_count | How we count sunny days | Cómo contamos los días de sol | Jak liczymy słoneczne dni | Wie wir Sonnentage zählen |
| foot_coverage | Coverage: 27 stations | Cobertura: 27 estaciones | Zasięg: 27 stacji | Abdeckung: 27 Stationen |
| foot_terms | Terms | Términos | Regulamin | AGB |
| foot_contact | Contact | Contacto | Kontakt | Kontakt |
| foot_bottom_disclaimer | Data: AEMET (2016–2025). Sunly is not affiliated with or endorsed by AEMET. | Datos: AEMET (2016–2025). Sunly no está afiliada a AEMET ni cuenta con su respaldo. | Dane: AEMET (2016–2025). Sunly nie jest powiązana z AEMET ani przez nią wspierana. | Daten: AEMET (2016–2025). Sunly ist nicht mit AEMET verbunden und wird nicht von AEMET unterstützt. |

(Copyright „© 2026 Sunly · app.sunly.live" i nazwa marki „Sunly" — bez tłumaczenia.
Nagłówek kolumny „SUNLY" w stopce — bez tłumaczenia.)

---

## Do decyzji / uwagi

- **Teksty wewnątrz makiet telefonów** (np. „Search for a place", „My location",
  „SUN CHANCE IN JULY", „NOW", „LIVE", „Trade Wind", „Rainfall characteristics",
  skróty miesięcy) — to odwzorowanie ekranów aplikacji. Aplikacja MA już te teksty
  przetłumaczone (`canaryweather/src/i18n/locales`). Decyzja: albo (a) zostawić makiety
  po angielsku (proste), albo (b) przełączać je razem z językiem strony, używając
  gotowych stringów z aplikacji (więcej pracy). Rekomendacja: na start (a) — angielskie
  makiety, bo to grafika poglądowa; (b) później, jeśli będzie potrzeba.
- **„Terms"** — jeśli nie mamy strony regulaminu, link do usunięcia (nie tłumaczyć na darmo).
- **„Get it on Google Play"** — użyłem oficjalnego brzmienia przycisku sklepu w każdym języku.
