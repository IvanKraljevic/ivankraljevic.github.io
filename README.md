# Personal site

This is my personal site hosted on GH pages.

## Run locally

On macOS, install rbenv and Ruby 3.4 (see the `.ruby-version` for the exact version:

```sh
brew install rbenv
rbenv install 3.4
rbenv init

# whn upgrading Ruby just invoke this to update it in .ruby-version
# rbenv local <ruby-version>
```

```sh
gem install bundler -v 2.6.6
bundle install
bundle exec jekyll serve --livereload
```

- Open [http://127.0.0.1:4000/](http://127.0.0.1:4000/).
- Jekyll rebuilds and refreshes the preview when you edit source files.
- Restart the server after changing `_config.yml`.
- Press `Ctrl+C` to stop it.
- For more details see : [GitHub Pages local preview guide](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll)

## Debug locally

For build failures, run a build with verbose logging and a stack trace. Check the file and line number reported in the terminal. [Jekyll command options](https://jekyllrb.com/docs/configuration/options/)

```sh
bundle exec jekyll build --trace --verbose
```
