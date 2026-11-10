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

## Voraussetzungen

Node.js **>= 22.12.0** ist erforderlich (Astro 7 unterstützt kein Node 20).
Debian 13 „Trixie" liefert nur Node 20.19 per apt — installiere Node 22 z. B. so:

```bash
# Variante A: NodeSource (apt-integriert)
curl -fsSL https://deb.nodesource.com/setup_22.x | sudo bash -
sudo apt install -y nodejs

# Variante B: offizielles Tarball
wget https://nodejs.org/dist/v22.12.0/node-v22.12.0-linux-x64.tar.xz -P ~
tar -xf ~/node-v22.12.0-linux-x64.tar.xz -C ~
echo 'export PATH="$HOME/node-v22.12.0-linux-x64/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

## Lokal starten

```bash
npm install --legacy-peer-deps   # --legacy-peer-deps ist nötig
npm run dev     # http://localhost:4321/psychotherapie-praxis/
npm run build   # statischer Build nach dist/
```

## Deployment (GitHub Pages)

- Repo: `gehacreate/psychotherapie-praxis`
- `src/config/config.json` → `site.base_url` / `site.base_path` an die Pages-URL anpassen
- Build per GitHub Actions und Upload von `dist/` (Pages from branch `gh-pages` oder Actions)

## Hinweise

Alle Inhalte (Name, Adresse, Telefon, E-Mail) sind Platzhalter und vor Veröffentlichung
anzupassen. Datenschutz- und Impressumstext sind Beispiele und sollten anwaltlich geprüft werden.
