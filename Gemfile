# frozen_string_literal: true

source 'https://rubygems.org'
git_source(:github) { |repo_name| "https://github.com/#{repo_name}" }
gemspec

# only needed on older windowses actually
install_if -> { RUBY_PLATFORM =~ /mingw32/ } do
  gem 'win32console', '~> 1.3'
end

if ENV['CI'] == 'true'
  gem 'codecov'
  gem 'simplecov'
end
