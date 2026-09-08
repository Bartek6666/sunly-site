# Sunly — Design Brief for `app.sunly.live`

> Paste this into Claude Design (or any design tool) to kick off the redesign of the
> Sunly download page. It contains everything needed: product context, goal, brand,
> full page copy, available assets and technical constraints.

---

## 1. What we're redesigning

`app.sunly.live` — the public **product / download page** for the mobile app **Sunly**.
Single static page, hosted for free on GitHub Pages. It is **not** the app itself, and
**not** the B2B business (that's a separate widget/SaaS).

**Important context:** Sunly is now **live on Google Play** (published Sept 2026).
The current page was built earlier as a *tester-recruitment* page ("leave your Gmail to
join the closed test"). That framing is now obsolete — the new page is a normal
**"download Sunly" product page**. No more tester/testing language anywhere.

---

## 2. The product in one line

**Sunly shows the statistical chance of sun for a destination and month, based on
10 years of official AEMET weather data.** It answers a question ordinary weather apps
can't: *"In this place, in this month — how often has it actually been sunny over the
last 10 years?"* It also shows current live conditions, but it is **not a forecast**.

- Free, no ads, no account, no tracking.
- Android only (iOS "coming soon").
- Coverage: **Canary Islands, Balearic Islands, Spanish Mediterranean coast.**
- Data source: **AEMET** (Spanish national met service), 10 years of daily records.

## 3. Who visits this page

Mostly people **planning a trip** to the Canaries / Balearics / Spanish coast — deciding
*when* and *where* to go for the best chance of sun. Usually **not** on-site tourists.
They arrive from Facebook posts/links in travel groups. Multi-national audience →
the page ships in **4 languages: EN (default), ES, PL, DE**.

## 4. Goal & primary action

- **Primary CTA:** *Get it on Google Play* → `https://play.google.com/store/apps/details?id=com.canaryweather.app`
- Secondary: build trust (real data, free, private) and show the app via screenshots.
- Tertiary: a small **"For tourism businesses"** band linking to a B2B email enquiry.

Success = a visitor understands the value in ~5 seconds and taps *Get it on Google Play*.

---

## 5. Brand & visual language (keep consistent with the app)

The app is a **light**, airy, glassy theme with a **blue + sun** identity and the
**Manrope** typeface. The page should feel like the same product.

### Colors
| Token | Hex | Use |
|---|---|---|
| primary | `#0052D4` | brand blue, buttons, links |
| on-primary | `#FFFFFF` | text on blue |
| primary-soft | `#E7EFFC` | tinted panels |
| sun | `#FBBF24` | sun accent / badges |
| sun-strong | `#F59E0B` | stronger sun accent, kickers |
| background | `#F4F8FE` | page base |
| surface | `#FFFFFF` | cards |
| surface-soft | `#F5F8FD` | subtle fills |
| ink | `#0F2540` | primary text (dark navy) |
| muted | `#5B6B82` | secondary text |
| line | `#E2E9F3` | borders |

Body background gradient (sky): `linear-gradient(175deg, #E4EEFB, #CFDFF4 60%, #C6DAF2)`.

### Type & icons
- **Font:** Manrope (Google Fonts), weights 400–800. Headlines extrabold/bold, tight tracking.
- **Icons:** Material Symbols Outlined.

### Logo
Rounded blue tile (radial `#0052D4`→`#003EA6`), a sun circle (`#FFD700`→`#FF8C00`)
with a soft highlight, and **two layered jagged white waves** along the bottom (a faint
back wave + a solid front wave with a thin light-blue crest line `#A8D8F0`). Word-mark
"Sunly" in primary blue, extrabold Manrope.

**⚠️ Use the correct logo files (they match the real Google Play icon):**
- Mark: `sunly-logo.svg` (+ `sunly-logo-1024.png` / `-512.png`)
- Horizontal lockup: `sunly-lockup.svg` (light bg) / `sunly-lockup-dark.svg` (dark bg)
- Vertical lockup: `sunly-vertical.svg`

Do **not** copy the simplified single-wave logo that appears in the old page markup /
the `sunly-saas` project — that is an outdated variant. The files above are the canonical
brand mark, identical to the app icon on Google Play.

### Aesthetic direction (pick / explore in Claude Design)
Stay **light and on-brand**, but make it feel **premium and modern** — avoid the generic
"AI landing page" look (no default purple gradients, no clichéd stock layout). Possible
directions to explore:
- **Premium refresh** — same blue/sun identity, more whitespace, soft glass, smooth motion.
- **Bold / editorial** — big type, a large animated "sun-chance" gauge as hero centerpiece.
- **Warm / travel** — golden accents, vacation warmth, more emotional.
- **Product-led** — real app screenshots in a phone mockup as the hero focal point.

A signature idea worth using: the app's core visual is a **circular "sun chance %" gauge**
(e.g. "87% — Tenerife, July"). That gauge is a strong, ownable hero motif.

### ✅ CHOSEN direction (based on reference sites the owner likes)
Clean, light, **product-led** — inspired by modern app-landing templates (a fintech
"ProFinance / Invest for the Future"-style layout), adapted to Sunly's blue + sun identity.
**Replace the reference's lime-green accent with Sunly blue `#0052D4` + sun `#FBBF24/#F59E0B`
everywhere.** Base is white / very light blue.

Layout & structure to follow:
- **Split hero:** app value proposition + "Get it on Google Play" button on the LEFT; a
  **phone mockup on the RIGHT** showing the app. Optionally on a soft rounded color panel
  (sky-blue tint) with a subtle **sun-glow** accent (not a lime blob).
- **Alternating sections:** text on one side, a phone mockup or floating UI cards on the
  other. Feature the app's best screens in the mockups — especially the **sun-chance (%)
  screen** and the **wind screen**.
- **Floating UI snippets:** lift small real UI elements (e.g. a sun-chance gauge card, a
  month tile) out over the background for a lively, product-led feel.
- **Feature / "advantages" grid:** icon + short title + one line, clean 2-column grid.
- **Dark CTA banner** near the end: rounded **navy `#0F2540`** band — "Get Sunly free" +
  Google Play button + a phone mockup overlapping.
- **Big bold closing CTA** before the footer (centered, e.g. "Get the app for free").

Style: generous whitespace, rounded corners, soft shadows, **not overloaded**; bold, tight
headlines. **Keep Manrope** (it matches the app and gives the same clean, modern, geometric
feel the owner liked in the reference font). Subtle playful touches allowed (a thin
hand-drawn connecting line, a soft sun-glow) — but restrained and on-brand.

Screens to feature in mockups (`screens/en/`): `03-result` (sun chance + live weather),
`05-wind` (wind), `04-stats` (monthly stats), `06-rain`, `01-search`, `02-regions`.

---

## 6. Page content (English = source of truth)

Keep all of this content (reworded/restyled is fine). The page currently has these
sections, in order:

### Header
- Logo "Sunly" + language switch: **EN · ES · PL · DE**

### Hero
- **H1:** "Know your chance of sunshine before you book"
- **Sub:** "Sunly shows the statistical chance of sun for your destination and month — from 10 years of official AEMET weather data."

### Intro + trust chips
- **Kicker:** "Free Android app · 10 years of AEMET data · Canary Islands, Balearic Islands, Spanish coast"
- **H2:** "Not a forecast — statistical certainty"
- **Body:** "Weather apps forecast the weather for tomorrow, the day after, a few days ahead. Sunly answers a different question: in this place, in this month, how often has it actually been sunny over the last 10 years?"
- **Chips:** No ads · No tracking · Free · 10 years of AEMET data

### Screenshot gallery — "See the app in action"
Horizontal scroll of 6 phone screenshots, tap to enlarge (lightbox). Files/captions:
1. `01-search.png` — Search — pick your destination
2. `02-regions.png` — Canary Islands, Balearics and the Spanish coast
3. `03-result.png` — Sun chance and live weather
4. `04-stats.png` — Monthly statistics from 10 years of data
5. `05-wind.png` — Wind details
6. `06-rain.png` — Rain details

### Download card — primary CTA
- **Title:** "Get Sunly on Google Play"  · badge: "Free"
- **Body:** "Free, no ads, no account. Install Sunly from Google Play and check the chance of sun for any destination and month in seconds."
- **Benefits:** Automatic updates · Safe & official
- **Button:** "Get it on Google Play" → Google Play URL (below)
- **Note:** "iOS version coming soon." + link to privacy policy

### Key features (4)
- **Sun chance** — "The % of sunny days for your place and month, from 10 years of records."
- **Monthly stats** — "Average highs and lows, rainy days, and 10-year temperature charts."
- **Live weather** — "Current conditions from the nearest station, plus Calima and high-wave alerts."
- **Wide coverage** — "Canary Islands, Balearic Islands, Spanish Mediterranean coast."

### FAQ (4)
- **How do I install it?** — "Open the Google Play listing on your Android phone and tap Install — it's free, no account needed."
- **What data does it collect?** — "Nothing that identifies you. Your location is used only on request to find the nearest station. See the full privacy policy."
- **Is it really free?** — "Yes — free, no ads, no account needed."
- **Is it a weather forecast?** — "No. Sunly shows historical statistics — how often it was sunny in the past — to help you plan. It also shows current live conditions, but it is not a forecast."

### For tourism businesses (SaaS band) — KEEP
- **Kicker:** "For tourism businesses"
- **H3:** "Add 'chance of sun' to your website"
- **Body:** "Run a hotel, apartment rental or travel agency? Embed the Sunly sun-chance widget on your site — the same 10 years of AEMET data, on your own pages."
- **CTA:** "Get in touch" → `mailto:info@sunly.live?subject=Sunly for business`

### Footer — KEEP (legal requirement)
- Logo + "© 2026 Sunly · Android · **Data: AEMET (aemet.es) · Not affiliated with AEMET**"
- Links: Privacy · Contact

---

## 7. Must-keep (non-negotiable)

1. **Google Play button** → `https://play.google.com/store/apps/details?id=com.canaryweather.app`
2. **AEMET attribution + "Not affiliated with AEMET"** disclaimer in the footer (Google Play policy requirement).
3. **"For tourism businesses" SaaS band** with `mailto:info@sunly.live?subject=Sunly for business`.
4. **4 languages** EN/ES/PL/DE with an in-page switcher (no page reload).
5. **Cookieless analytics** (GoatCounter — no cookie banner needed).
6. **Privacy policy link:** `https://fishy-chili-431.notion.site/Privacy-Policy-Sunly-33fcf25df26a80ecba78deb415a373b6`
7. **Contact email:** `info@sunly.live`

## 8. Available assets

- **6 app screenshots** (English UI), portrait phone shots: `screens/en/01-search.png` … `06-rain.png`.
- **Logo** as inline SVG (in current `index.html`).
- Everything else is CSS/SVG (illustrated sun + waves hero) — no photography yet.

---

## 9. Technical constraints (important for implementation)

- **One static `index.html`**, no build step. Styling via **Tailwind (CDN)**. Fonts via
  Google Fonts. Deployed on **GitHub Pages** at `app.sunly.live` (a `CNAME` file pins the domain).
- **Must stay lightweight & fast** — inline SVG/CSS over heavy images; lazy-load screenshots.
- **Mobile-first** — most visitors are on phones coming from Facebook links.
- **4-language mechanism:** every translatable string is duplicated as 4 `<span>`s with a
  `data-key` suffix (`_en/_es/_pl/_de`); a tiny script toggles which is visible and remembers
  the choice in `localStorage`, defaulting to the browser language.
- **Analytics:** GoatCounter (`sunly.goatcounter.com`), cookieless — keep it, no consent banner.
- Accessibility: real `<a>`/`<button>`, `aria-*`, visible focus, alt text on screenshots.

### Suggested workflow with Claude Design
Design & build the **layout + visuals in English first** (one language, clean HTML/Tailwind).
The **4-language wiring, GoatCounter, lightbox and final translations** can be re-applied
afterward in the real repo (they already exist in the current page and are easy to port).
This keeps the design exploration fast and uncluttered.

---

## 10. Key facts (quick reference)

| Item | Value |
|---|---|
| Domain | `app.sunly.live` |
| Google Play | `https://play.google.com/store/apps/details?id=com.canaryweather.app` |
| Privacy policy | `https://fishy-chili-431.notion.site/Privacy-Policy-Sunly-33fcf25df26a80ecba78deb415a373b6` |
| Contact | `info@sunly.live` |
| Business enquiry | `mailto:info@sunly.live?subject=Sunly for business` |
| Analytics | GoatCounter `sunly.goatcounter.com` (cookieless) |
| Languages | EN (default), ES, PL, DE |
| Platform | Android (iOS "coming soon") |
| Data | AEMET, 10 years, daily records |
