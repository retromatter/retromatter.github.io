# frozen_string_literal: true

source "https://rubygems.org"

# Core Jekyll dependency
gem "jekyll", "~> 4.3.3"

# Essential for Windows to prevent polling and reduce CPU usage
gem "wdm", ">= 0.1.1" if Gem.win_platform?

# Required for Ruby 3.0+ to run the local server
gem "webrick", "~> 1.8"

# Standard plugins for SEO and Feeds
group :jekyll_plugins do
  gem "jekyll-feed", "~> 0.17"
  gem "jekyll-sitemap"
  # If you want to use the README as your index as discussed earlier:
  # gem "jekyll-readme-index"
end

# Optional: If you plan to deploy to GitHub Pages specifically, 
# you can use this gem to align versions, but it can sometimes 
# conflict with Jekyll 4.x. For now, Jekyll 4.3 is better for local dev.
# gem "github-pages", group: :jekyll_plugins