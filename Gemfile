source 'https://rubygems.org'

git_source(:github) do |repo_name|
  repo_name = "#{repo_name}/#{repo_name}" unless repo_name.include?("/")
  "https://github.com/#{repo_name}.git"
end


# Bundle edge Rails instead: gem 'rails', github: 'rails/rails'
gem 'rails', '~> 5.0.7'

gem 'mysql2', '>= 0.3.18', '< 0.6.0'
# Use Puma as the app server
gem 'puma', '~> 3.0'
# Use SCSS for stylesheets
gem 'sass-rails', '~> 5.0'
# Use Uglifier as compressor for JavaScript assets
gem 'uglifier', '>= 1.3.0'
# Use CoffeeScript for .coffee assets and views
gem 'coffee-rails', '~> 4.2'
# See https://github.com/rails/execjs#readme for more supported runtimes
# gem 'therubyracer', platforms: :ruby

# Use jquery as the JavaScript library
gem 'jquery-rails'
# Turbolinks makes navigating your web application faster. Read more: https://github.com/turbolinks/turbolinks
gem 'turbolinks', '~> 5'
# Build JSON APIs with ease. Read more: https://github.com/rails/jbuilder
gem 'jbuilder', '~> 2.5'
# Use Redis adapter to run Action Cable in production
# gem 'redis', '~> 3.0'
# Use ActiveModel has_secure_password
# gem 'bcrypt', '~> 3.1.7'

# Use Capistrano for deployment
# gem 'capistrano-rails', group: :development


# gem 'bootstrap-sass'
# gem 'carrierwave'
# gem 'chart-js-rails'
# gem 'credit_card_validator'
# gem 'devise'
# gem 'devise-i18n'
# gem 'devise-i18n-views'
# gem 'dotenv-rails'
# gem 'gon'
# gem 'kakurenbo-puti'
# gem 'kaminari'
# gem 'less-rails'
# gem 'mini_magick'
# gem 'momentjs-rails'
# gem 'omniauth'
# gem 'omniauth-facebook'
# gem 'omniauth-google-oauth2'
# gem 'pagy'
# gem 'payjp'
# gem 'rails-i18n'
# gem 'ransack'
# gem 'squasher'
# gem 'whenever', require: false

group :development, :test do
  # Call 'byebug' anywhere in the code to stop execution and get a debugger console
  gem 'byebug', platform: :mri
  # gem 'capybara', '~> 2.13'
end

group :development do
  # Access an IRB console on exception pages or by using <%= console %> anywhere in the code.
  gem 'pry'
  gem 'listen', '~> 3.0.5'
  # Spring speeds up development by keeping your application running in the background. Read more: https://github.com/rails/spring
  gem 'spring'
  gem 'spring-watcher-listen', '~> 2.0.0'
  gem 'web-console', '>= 3.3.0'


  gem 'better_errors'
  gem 'binding_of_caller'
  gem 'bullet'
  # gem 'capistrano-rails'
  gem 'faker', require: false # for sample data in development
  gem 'letter_opener_web'
  # https://qiita.com/silmisilon/items/8e08435204d8d08d09ff
  # https://qiita.com/k0kubun/items/b118e9ccaef8707c4d9f
  gem 'pry-doc'
  gem 'pry-rails'
  gem 'pry-stack_explorer'
  # display params to explain simply in console
  gem 'rails-flog', require: 'flog'
  gem 'spring-commands-rspec'
end

group :production do
  gem 'rails_12factor'
end
# Windows does not include zoneinfo files, so bundle the tzinfo-data gem
# gem 'tzinfo-data', platforms: [:mingw, :mswin, :x64_mingw, :jruby]
