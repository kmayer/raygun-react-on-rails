source "https://rubygems.org"
git_source(:github) { |repo| "https://github.com/#{repo}.git" }

# Heroku uses the ruby version to configure your application"s runtime.
ruby "2.6.5"

# Back-endy
gem "bootsnap", require: false
gem "pg"
gem "puma"
gem "rack-canonical-host"
gem "rails", "~> 6.0.0"
gem "react_on_rails", "11.1.4" # Update to the current version

# Front-endy
gem "bootstrap", "~> 4.3.1"
gem "jquery-rails"
gem "mini_racer", platforms: :ruby
gem "sassc-rails"
gem "simple_form"
gem "slim-rails"
gem "uglifier"
gem "webpacker", "~> 4" # Newer versions might be supported

# Tools
gem "awesome_print"

# Env specific dependencies...

group :production, :acceptance do
  gem "rack-timeout"
end

group :development, :test do
  gem "factory_bot_rails"
  gem "rspec-rails", "~> 4.0.0.beta2" # For Rails 6 support.
  gem "rspec_junit_formatter"
  gem "rubocop", require: false
  gem "rubocop-performance", require: false
  gem "rubocop-rails", require: false
end

group :development do
  gem "annotate"
  gem "better_errors"
  gem "binding_of_caller"
  gem "dotenv-rails"
  gem "launchy"
  gem "listen"
  gem "spring"
  gem "spring-commands-rspec"
  gem "spring-watcher-listen"
  # gem "guard"
  # gem "guard-rspec", ">= 4.6.5" # Resolves to 1.x without a version constraint. :/
  # gem "guard-livereload"
end

group :test do
  gem "capybara"
  # gem "capybara-email"
  gem "selenium-webdriver"
  gem "simplecov"
  gem "webdrivers"
end
