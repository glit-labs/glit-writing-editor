source "https://rubygems.org"

# Local build uses modern Jekyll 4 (Liquid 5), which is compatible with current
# Ruby. GitHub Pages builds the deployed site with its own environment via the
# `remote_theme` setting in _config.yml, so this Gemfile only affects local
# preview.
gem "jekyll", "~> 4.3"

group :jekyll_plugins do
  gem "jekyll-remote-theme"
  gem "jekyll-include-cache"
  gem "jekyll-feed"
  gem "jekyll-seo-tag"
  gem "jekyll-sitemap"
  # Provided automatically on GitHub Pages; added explicitly for local parity so
  # markdown files without front matter still render and get titles from their
  # first heading.
  gem "jekyll-optional-front-matter"
  gem "jekyll-titles-from-headings"
end

# Needed by `jekyll serve` on modern Ruby.
gem "webrick"

# Windows / JRuby do not include zoneinfo files, so bundle the tzinfo-data gem.
platforms :mingw, :x64_mingw, :mswin, :jruby do
  gem "tzinfo", ">= 1", "< 3"
  gem "tzinfo-data"
end
