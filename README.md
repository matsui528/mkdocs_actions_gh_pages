# Deploy mkdocs on github pages via github actions
- Render html files using mkdocs through GitHub actions. Upload the artifacts (html files) to GitHub pages automatically.
- No need to push html files to `gh-pages` branch or `docs` directory.


## Build
```console
pip install -r requirements.txt
mkdocs build   # Render html files on the `site` directory
```

## Configure
- Activate GitHub Pages by specifying `source` as `GitHub Actions`. See [this]((https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site#publishing-with-a-custom-github-actions-workflow)).
- Setup workflow like [this](.github/workflows/pages.yml)
- Done. See [the rendered page here](https://matsui528.github.io/mkdocs_actions_gh_pages/).