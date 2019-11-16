# frozen_string_literal: true

source 'https://rubygems.org'

solidus_branch = ENV.fetch('SOLIDUS_BRANCH', 'master')

gem 'solidus', github: 'solidusio/solidus', branch: solidus_branch
gem 'solidus_auth_devise'
gem 'avatax-ruby', git: 'git@github.com:boomerdigital/avatax.git', require: 'avatax', branch: 'crossborder'

case ENV['DB']
when 'postgres'
  gem 'pg'
when 'mysql'
  gem 'mysql2'
else
  gem 'sqlite3'
end

gemspec
