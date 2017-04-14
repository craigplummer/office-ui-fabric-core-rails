require "bundler/gem_tasks"
require "rspec/core/rake_task"

RSpec::Core::RakeTask.new(:spec)

task :default => :spec

namespace :assets do
  desc 'Update Office UI Fabric Core assets'
  task update: :clean do
    sh 'yarn install'
    sh 'cp -r node_modules/office-ui-fabric-core/dist/sass/* vendor/assets/scss'
    sh 'cp -r node_modules/office-ui-fabric-core/dist/css/* vendor/assets/css'

    puts "Updated to the latest version of Office UI Fabric Core"
  end

  desc 'Remove old office-ui-fabric-core assets'
  task :clean do
    sh 'rm -rf vendor'
    sh 'mkdir -p vendor/assets/scss/ vendor/assets/css'
  end
end
