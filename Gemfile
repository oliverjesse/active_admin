source 'http://rubygems.org'

gemspec

ACTIVE_ADMIN_PATH = File.dirname(__FILE__) unless defined?(ACTIVE_ADMIN_PATH)

require File.expand_path('spec/support/detect_rails_version', ACTIVE_ADMIN_PATH)

rails_version = detect_rails_version
gem 'rails', rails_version
gem 'bourbon'

group :assets do
  gem 'sass-rails'
  gem 'uglifier'
end

group :development, :test do
  gem 'haml', '~> 3.1.7',  :require => false
  gem 'rake', '~> 10.0.2', :require => false
  gem 'rails-i18n' # Provides default i18n for many languages
  gem 'rdiscount'  # Markdown implementation (for yard)
  gem 'sprockets'
  gem 'yard'
end

group :test do
  gem 'cancan'
  gem 'capybara',        '1.1.2'
  gem 'cucumber-rails',  '1.3.0', :require => false
  gem 'database_cleaner'
  gem 'guard-coffeescript'
  gem 'guard-rspec'
  gem 'jasmine'
  gem 'jslint_on_rails', '~> 1.1.1'
  gem 'launchy'
  gem 'parallel_tests'
  gem 'rspec-rails',     '~> 2.9.0'
  gem 'shoulda-matchers', '1.5.0' # See active_admin#2004
  gem 'sqlite3'
end
