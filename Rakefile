namespace :greeting do
  desc 'outputs hello to the terminal'
  task :hello do
    puts "hello from Rake!"
  end

  task :hola do
    puts "hola de Rake!"
  end
end

task :environment do
  require_relative './config/environment'
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment  do
    Student.create_table
  end

  desc 'migrate changes to your database'
  task :seed => :environment  do
    require_relative './db/seeds'
  end
end
