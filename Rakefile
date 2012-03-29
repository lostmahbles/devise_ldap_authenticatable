require File.expand_path('test/rails_app/config/environment', File.dirname(__FILE__))
require 'rake/testtask'
require 'rdoc/task'

desc 'Default: run test suite.'
task :default => :test

desc 'Generate documentation for the devise_ldap_authenticatable plugin.'
Rake::RDocTask.new(:rdoc) do |rdoc|
  rdoc.rdoc_dir = 'rdoc'
  rdoc.title    = 'DeviseLDAPAuthenticatable'
  rdoc.options << '--line-numbers' << '--inline-source'
  rdoc.rdoc_files.include('README.md')
  rdoc.rdoc_files.include('lib/**/*.rb')
end

RailsApp::Application.load_tasks
