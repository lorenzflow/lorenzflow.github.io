# lorenzflow.github.io

Personal website of Lorenz Wolf. Plain [Jekyll](https://jekyllrb.com/), built and hosted by GitHub Pages; no theme or build tooling to maintain.

## Editing

Everything lives in a handful of files:

| What | File |
| --- | --- |
| Name, role, photo, links | `_data/profile.yml` |
| About text | `_includes/about.md` |
| **News** | `_data/news.yml` |
| Publications | `_data/publications.yml` |
| Experience / Education | `_data/experience.yml`, `_data/education.yml` |
| Projects | `_data/projects.yml` |
| Styling | `assets/css/style.css` |

### Add a news item

Add an entry at the **top** of `_data/news.yml` (you can do this straight in the GitHub web editor):

```yaml
- date: Oct 2026
  text: >-
    Our paper [Title: Subtitle](https://arxiv.org/abs/...) was accepted at **NeurIPS 2026**!
```

The newest `news_shown` items (set in `_config.yml`, default 8) are shown; the rest sit behind "Show all news".

### Add a publication

Add an entry at the top of `_data/publications.yml`. `image` (put the file in `assets/img/`), `note` (e.g. "Spotlight") and `abstract` are optional; any `links` key becomes a `[name]` link.

## Local preview

```sh
gem install jekyll
jekyll serve      # http://localhost:4000
```

## Deploying

Settings → Pages → "Deploy from a branch", pick the branch and `/ (root)`. A repo named `lorenzflow.github.io` is served at https://lorenzflow.github.io.
