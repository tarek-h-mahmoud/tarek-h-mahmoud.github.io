# tarek-h-mahmoud.github.io

Personal academic website of Tarek Mahmoud — Applied AI Scientist, PhD in Natural Language Processing.

Live at **[tarek-h-mahmoud.github.io](https://tarek-h-mahmoud.github.io)**.

## Running locally

```bash
bundle install
bundle exec jekyll serve
```

The site is then at `http://localhost:4000`. Note that `_config.yml` is read once at startup, so restart the server after changing it — `--watch` will not pick it up.

## Layout

| Path             | Contents                                              |
| ---------------- | ----------------------------------------------------- |
| `_pages/`        | About, Selected Projects, Publications, News, CV       |
| `_projects/`     | One file per project; front matter drives the cards    |
| `_news/`         | One file per news item                                 |
| `_bibliography/` | `papers.bib` — publications, posters, slides, videos   |
| `_data/`         | Socials, co-authors, venues                            |
| `assets/pdf/`    | CV, conference posters and slides                      |

## Deployment

`.github/workflows/deploy.yml` builds on push to `main` and publishes the
result to the `gh-pages` branch, which is what GitHub Pages serves.

## Credits

Built on [al-folio](https://github.com/alshedivat/al-folio) by Maruan
Al-Shedivat and contributors, used under the MIT License. See
[`LICENSE`](LICENSE).
