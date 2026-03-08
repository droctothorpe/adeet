# Agentic Development Environment Extension Taxonomy

There has been a proliferation of agentic development environment extensions from competing vendors. As a result, the market has profoundly inconsistent nomenclature and standards that make the domain space seem unecessarily complex. This page is an attempt to simplify and disambiguate the available offerings.

https://droctothorpe.github.io/adeet/

## Content Framework (GitHub Pages build-time)

This site uses Jekyll's built-in `_data` pipeline so content is rendered at build time on GitHub Pages.

- Edit `/_data/taxonomy.yml` to change:
- Box titles and descriptions (`nodes`)
- Item labels and descriptions (`nodes`)
- Which items appear in each list (`lists`)
- Page heading/subtitle/footer link (`page`)

`index.html` reads this YAML through Liquid (`site.data.taxonomy`) and receives static JSON in the final generated HTML. No runtime YAML parsing is used in the browser.

### Local Preview (optional)

If you want to preview the GitHub Pages build locally:

```bash
bundle install
bundle exec jekyll serve
```

If `bundle` is missing, install Bundler first:

```bash
gem install bundler
```
