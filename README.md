# Wen-Hsi Kuo Academic Website

This site uses the [al-folio](https://github.com/alshedivat/al-folio) academic Jekyll theme.

## Local Preview

```bash
cd /Users/kuowenhsi/kuowenhsi.github.io
export PATH="$HOME/.rbenv/shims:$PATH"
bundle install
bundle exec jekyll serve
```

Then open `http://127.0.0.1:4000`.

## Main Files To Edit

- Site settings: `_config.yml`
- Homepage biography: `_pages/about.md`
- Publications: `_bibliography/papers.bib`
- Research/project pages: `_projects/`
- Teaching entries: `_teachings/`
- CV content: `_data/cv.yml`
- Social links: `_data/socials.yml`
- Header/profile image: `assets/img/research-header.png`

## Deployment

For this personal GitHub Pages repository, `_config.yml` uses:

```yml
url: https://kuowenhsi.github.io
baseurl:
```

Push changes to `main`, then use the repository's GitHub Pages/Actions settings to deploy the built site.
