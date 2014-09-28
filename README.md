... WORK IN PROGRESS ...

# Run locally

First, install `gem install github-pages` (might need to fix this: http://stackoverflow.com/questions/19643153/error-to-install-nokogiri-on-osx-10-9-maverick)

Then, in console run: `jekyll serve --watch`.

# Render with rmarkdown

```{r}
devtools::install_github("reinholdsson/jekyllr")
```

Either write the article/blog posts directly in markdown, or use rmarkdown and then render the page with `jekyllr`. See examples in the `_posts` directory.

# Structure

- `_data/`
  - `authors.yml`: list of contributors
  - `navigation.yml`: navigation pages
  - `packages.yml`: list of packages
- `_posts/`
  - `article`: put new articles here, make sure the filename of the *.md*-file is *YYYY-MM-DD-article-title*.
  - `blog`: blog posts
- `packages/index.md`: packages page
- `about/index.md`: about page
- `images`: all images

See also `_config.yml` which includes site wide configuration.

# Jekyll theme

See [**Minimal Mistakes**](http://mmistakes.github.io/minimal-mistakes/).
