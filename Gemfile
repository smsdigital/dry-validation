source 'https://rubygems.org'

gemspec

group :test do
  gem 'i18n', require: false
  platform :mri do
    gem 'codeclimate-test-reporter', require: false
    gem 'simplecov', require: false
  end
  gem 'dry-monads', '< 1.0', require: false
  gem 'dry-struct', require: false
end

group :tools do
  gem 'byebug', platform: :mri
  gem 'pry'

  unless ENV['TRAVIS']
    gem 'mutant', github: 'mbj/mutant'
    gem 'mutant-rspec', github: 'mbj/mutant'
  end
end

group :benchmarks do
  gem 'hotch', platform: :mri
  gem 'activemodel', '~> 5.0.0.rc'
  gem 'actionpack', '~> 5.0.0.rc'
  gem 'benchmark-ips'
  gem 'virtus'
end

gem 'dry-logic', '~> 0.4.2', git: 'https://github.com/smsdigital/dry-logic', tag: 'v0.4.2.1'
gem 'dry-types', '~> 0.12.3', git: 'https://github.com/smsdigital/dry-types', tag: 'v0.12.3.1'
