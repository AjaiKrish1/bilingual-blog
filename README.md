# AJ — Science × Philosophy (Bilingual Jekyll Blog)

This is a ready‑to‑use **bilingual (EN/DE)** Jekyll blog designed for GitHub Pages. It uses the `jekyll-polyglot` plugin and a minimal science‑and‑philosophy‑inspired theme.

## Quick Start (GitHub Pages with Actions)

1. **Create a new repo** on GitHub and push these files.
2. In **Settings → Pages** set **Build and deployment → Source** to **GitHub Actions**.
3. The included workflow in `.github/workflows/pages.yml` will build with `jekyll-polyglot` and deploy to Pages.
4. Your site will be served at: `https://<your-username>.github.io/<repo-name>/` (or at your user site if you use `<your-username>.github.io`).

## Local Development

```bash
bundle install
bundle exec jekyll serve
```
Then visit http://localhost:4000

## Change Languages

- Edit `_config.yml` `languages` array (e.g., `["en","de","ta"]`) and add translations in `_data/i18n/<lang>.yml`.
- Use `site.data.i18n[site.active_lang]` keys in templates to localize strings.

## Where to Edit

- **Home page intro:** `_data/i18n/en.yml` & `_data/i18n/de.yml` under `home.intro`.
- **Navigation labels:** `_data/i18n/*` under `nav.*`.
- **Styles:** `assets/css/main.css`.
- **Posts:** `_posts/en/*` and `_posts/de/*`.
- **Static pages:** `about.en.md`, `about.de.md`.

## Credits

- i18n by [jekyll‑polyglot](https://github.com/untra/polyglot)
- GitHub Pages build via Actions.
