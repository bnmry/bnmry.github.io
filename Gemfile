source 'https://rubygems.org'
gem 'font-awesome-less'

require 'json'
require 'open-uri'
versions = JSON.parse(open('https://pages.github.com/versions.json').read)

gem 'github-pages', versions['github-pages']

group :jekyll_plugins do
  gem "jekyll-youtube"
  gem "jekyll-app-engine"
end