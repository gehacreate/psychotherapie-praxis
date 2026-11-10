# Praxis für Psychotherapie – Astro SSG Beispielseite

Statische Webseite (Astro) für eine psychotherapeutische Praxis, basierend auf dem Theme
[themefisher/bigspring-light-astro](https://github.com/themefisher/bigspring-light-astro).

## Seiten

- Start (Hero, Schwerpunkte, Leistungen, Ablauf, CTA)
- Über mich (`/about`)
- Leistungen & Kosten – GKV / PKV / Selbstzahler (`/pricing`)
- Ratgeber mit 5 Artikeln (`/blog`)
- FAQ (`/faq`)
- Kontakt & Terminanfrage (`/contact`)
- Impressum, Datenschutzerklärung, Terminbedingungen

## Lokal starten

```bash
npm install
npm run dev     # http://localhost:4321
npm run build   # statischer Build nach dist/
```

## Deployment (GitHub Pages)

- Repo: `gehacreate/psychotherapie-praxis`
- `src/config/config.json` → `site.base_url` / `site.base_path` an die Pages-URL anpassen
- Build per GitHub Actions und Upload von `dist/` (Pages from branch `gh-pages` oder Actions)

## Hinweise

Alle Inhalte (Name, Adresse, Telefon, E-Mail) sind Platzhalter und vor Veröffentlichung
anzupassen. Datenschutz- und Impressumstext sind Beispiele und sollten anwaltlich geprüft werden.
