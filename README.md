# lizzonsh.github.io

Elizabeth Zonshtein's personal site — a single-page portfolio covering resume, projects, and hobbies. Hand-written HTML and CSS, no frameworks and no JavaScript; dark mode, the responsive nav, and the scroll animations are all done in CSS alone. Hosted on GitHub Pages.

## Structure

```
index.html              All page content (hero, resume, projects, hobbies)
assets/css/style.css     Styles, including dark mode and the mobile nav
assets/images/           Photos referenced by index.html
assets/docs/             Resume PDF (gitignored, not tracked in this repo)
```

## Local preview

No build step — open [index.html](index.html) directly in a browser, or serve the directory with any static file server.

## Linting

HTML and CSS are linted via [html-validate](.htmlvalidate.json) and [stylelint](.stylelintrc.json). CI runs both on pull requests into `dev` (see [.github/workflows/lint.yaml](.github/workflows/lint.yaml)):

```
npx html-validate "**/*.html"
npx stylelint "**/*.css"
```
