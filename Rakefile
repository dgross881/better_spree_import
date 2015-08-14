require 'bundler'
Bundler::GemHelper.install_tasks

require 'rspec/core/rake_task'
require 'spree/testing_support/common_rake'

task default: :spec

RSpec::Core::RakeTask.new 

APP_RAKEFILE = File.expand_path("../spec/dummy/Rakefile", __FILE__)
load 'rails/tasks/engine.rake'


desc 'Generates a dummy app for testing'
task :test_app do
  ENV['LIB_NAME'] = 'spree_import'
  Rake::Task['common:test_app'].invoke
end



