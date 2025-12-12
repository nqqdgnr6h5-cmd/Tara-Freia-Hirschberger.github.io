# Tara-Freia-Hirschberger.github.io

Dieses Repository enthält drei einfache Scaffolds, mit denen du lokal eine Website starten kannst:

- Jekyll (GitHub Pages-kompatibel)
- Einfache statische Site (plain HTML/CSS)
- Eleventy (Node-basiertes SSG)

Anleitung — lokale Nutzung

**Jekyll (Ruby / Bundler)**:

- Voraussetzungen: `ruby`, `bundler`.
- Im Repository-Root:

```bash
bundle install
bundle exec jekyll serve
```

Die Jekyll-Dateien befinden sich im Root (`_config.yml`, `index.md`, `_layouts/`, `assets/`).

**Einfache statische Site (plain HTML/CSS)**:

- Dateien unter `static/`.
- Starte einen einfachen HTTP-Server:

```bash
python3 -m http.server --directory static 8000
```

Öffne dann `http://localhost:8000`.

**Eleventy (Node / npm)**:

- Ein vollständiges Eleventy-Scaffold wurde unter `eleventy/` erstellt (Beispielseite, Layout, Styles, `package.json`).
- Einrichtung und Start (im Ordner `eleventy`):

```bash
cd eleventy
npm install
npx @11ty/eleventy --serve
```

Falls du `package.json` manuell neu erzeugen musst:

```bash
cd eleventy
npm init -y
npm install @11ty/eleventy --save-dev
npx @11ty/eleventy --serve
```

Weitere Hinweise

- Änderungen, die du lokal erstellst, kannst du committen und pushen:

```bash
git add .
git commit -m "Add site scaffold and README"
git push origin main
```

- Wenn du GitHub Pages verwenden willst, ist die Jekyll-Variante direkt kompatibel; alternativ kannst du das `static/`-Verzeichnis oder das Eleventy-Build-Output als GitHub Pages-Quelle deployen.

Wenn du möchtest, erstelle ich jetzt:
- das vollständige Eleventy-Scaffold (Layouts, Beispielseite)
- oder passe README weiter an (z. B. Deploy-Anweisungen für GitHub Actions).

