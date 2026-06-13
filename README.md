# Yunfei Tian personal homepage

This repository contains the source for `https://robbie194.github.io/`.

The site is built with [Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio) academic homepage theme.

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000/`.

## Main content files

- `_pages/about.md`: homepage biography
- `_bibliography/papers.bib`: publications
- `_projects/`: project pages
- `_news/`: homepage news items
- `_data/cv.yml`: rendered CV content
- `_data/socials.yml`: contact and social links
- `assets/img/prof_pic.jpg`: profile photo
- `assets/pdf/Yunfei_Tian_CV.pdf`: downloadable CV

## Deployment

Push to the `main` branch. GitHub Actions builds the Jekyll site and deploys it with GitHub Pages.
