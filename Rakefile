# encoding: utf-8

require 'rubygems'
require 'bundler'
begin
  Bundler.setup(:default, :development)
rescue Bundler::BundlerError => e
  $stderr.puts e.message
  $stderr.puts "Run `bundle install` to install missing gems"
  exit e.status_code
end
require 'rake'

require 'jeweler'
Jeweler::Tasks.new do |gem|
  # gem is a Gem::Specification... see http://guides.rubygems.org/specification-reference/ for more options
  gem.name = "myob-essentials-api"
  gem.homepage = "http://github.com/BrunoChauvet/myob-essentials-api"
  gem.license = "MIT"
  gem.summary = %Q{Integrate with MYOB Essentials Accounting}
  gem.description = %Q{Integrate with MYOB Essentials Accounting}
  gem.email = "it@maestrano.com"
  gem.authors = ["BrunoChauvet"]
  # dependencies defined in Gemfile
end
Jeweler::RubygemsDotOrgTasks.new

begin
  require 'rspec/core/rake_task'
  RSpec::Core::RakeTask.new(:spec)
  task :default => :spec
rescue LoadError
  # no rspec available
end
