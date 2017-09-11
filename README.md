# Ray Website

## Development instructions

With Ruby >= 2.1 installed, run:

```
gem install jekyll bundler
bundle install
```

To view the site, run:

```
bundle exec jekyll serve
```

Note that images included under `site/assets/` should be referred to with
`<img src="{{ site.base-url }}/ray/assets/...">`. They will not render properly
when serving the site locally, but this is required for getting the paths to
work out on GitHub.

## Deployment

To deploy the site, run

```
cd ~
git clone https://github.com/ray-project/ray-project.github.io.git
cd ray-project.github.io
cp -r ~/ray/site/* .
```

and commit as well as push the desired changes.
