source 'https://rubygems.org'
ruby file: '.ruby-version'

gem 'bootsnap'
gem 'pg'
gem 'puma'
gem 'puma_worker_killer'
gem 'rails', '~> 8.0.0'

gem 'jbuilder'
gem 'jquery-rails'

gem 'bootstrap-sass'
gem 'font-awesome-rails'
gem 'rails-html-sanitizer'
gem 'sass-rails', '>= 5'

# Add bundled gems for Ruby 3.3+
# https://gihyo.jp/article/2024/01/ruby3.3-bundled-gems
gem 'csv'
gem 'ostruct' # Depended by 'koala' gem and shown at 'deploy' job in Actions (rake assets:precompile)

gem 'rambulance'         # Error handling pages: https://github.com/yuki24/rambulance
gem 'airbrake'           # Error Monitoring by Airbrake: https://github.com/airbrake/airbrake
gem 'rack-host-redirect' # Enable redirection
gem 'secure_headers'     # Enable SSL and CORS
gem 'rinku'              # Enable Auto Link for Podcasts
gem 'sitemap_generator'  # Sitemap: https://github.com/kjvarga/sitemap_generator
gem 'rss'                # Add RSS for Podcasts: https://coderdojo.jp/podcasts
gem 'ruby-mp3info', require: 'mp3info' # For RSS feed

# Rendering *.md documents: https://coderdojo.jp/docs
gem 'kramdown'
gem 'kramdown-parser-gfm'

# Need to fetch Stats & UpcomingEvents.
# https://coderdojo.jp/stats
# https://coderdojo.jp/events
gem 'faraday'
gem 'koala'
gem 'lazy_high_charts', '1.5.8'
gem 'connpass_api_v2' # https://github.com/sue445/connpass_api_v2-ruby

# Protect from attacks for Security
gem 'rack-attack'
gem 'rack-user_agent'

# For Pokemon Workshop v1. https://coderdojo.jp/pokemon
# But current v2 does not need this, so can be removed.
gem 'aws-sdk-s3', '~> 1'

group :development do
  gem 'letter_opener_web'
  gem 'listen'
  gem 'solargraph'
  gem 'spring'
  gem 'web-console'

  # Enable perf tools if needed (YAGNI).
  # https://ja.wikipedia.org/wiki/YAGNI
  gem 'stackprof',          require: false
  gem 'flamegraph',         require: false
  gem 'memory_profiler',    require: false
  gem 'rack-mini-profiler', require: false
end

group :development, :test do
  gem 'rake'
  gem 'rspec-rails', '~> 6.1.1'
  gem 'rspec-retry'

  gem 'capybara'
  gem 'factory_bot_rails'
  gem 'selenium-webdriver'

  gem 'rails-controller-testing'
  gem 'dotenv-rails'

  # NOTE: This enable GitHub Codespaces. Uncomment for YAGNI.
  # https://github.com/coderdojo-japan/coderdojo.jp/pull/1526
  #gem 'mini_racer'
end
