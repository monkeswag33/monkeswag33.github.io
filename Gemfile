require "uri"
require "net/http"
require "json"
source "https://rubygems.org"

plugins = [
    "jekyll-feed",
    "jekyll-remote-theme",
    "jekyll-paginate",
    "jekyll-sitemap",
    "jekyll-gist",
    "jekyll-include-cache"
]
versions = JSON.parse(Net::HTTP.get_response(URI("https://pages.github.com/versions.json")).body)
puts "Retrieved Github Pages versions..."
# Hello! This is where you manage which Jekyll version is used to run.
# When you want to use a different version, change it below, save the
# file and run `bundle install`. Run Jekyll with `bundle exec`, like so:
#
#     bundle exec jekyll serve
#
# This will help ensure the proper Jekyll version is running.
# Happy Jekylling!
# gem "jekyll", "~> 4.3.3"
# This is the default theme for new Jekyll sites. You may change this to anything you like.
# gem "minima", "~> 2.5"
# If you want to use GitHub Pages, remove the "gem "jekyll"" above and
# uncomment the line below. To upgrade, run `bundle update github-pages`.
gem "github-pages", versions["github-pages"]

group :jekyll_plugins do
    plugins.each { |plugin| gem plugin, versions[plugin] }
end
# gem "faraday-retry", "~> 2.2"
