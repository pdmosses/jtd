source 'https://rubygems.org'

if ENV["JEKYLL_VERSION"]
  gem "jekyll", ENV["JEKYLL_VERSION"]
elsif ENV["JEKYLL_LOCAL"]
  gem "jekyll", path: '../jekyll'
else
  gem "jekyll"
end

gem "just-the-docs"

# Optional. For serving with default config.
gem "jekyll-remote-theme"
