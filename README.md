# jtd

Test Just-the-Docs search data

To reproduce the results shown in `assets/jekyll-4.1.1/`:

1. Copy `assets/jekyll-4.1.1/Gemfile` to the `jtd` folder.
2. Run `bundle update`.
3. Run `bundle exec jekyll serve --config _config.yml,_config_local.yml`.
4. Check that `_site/assets/js/search-data.json` has the same contents as `assets/jekyll-4.1.1/search-data.json`.

Similarly for `assets/jekyll-4.2.0/`.
