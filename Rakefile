namespace  :greeting do
desc "Display message on terminal"
task :hello do
  puts "hello it's Rake!"
end

desc "greet MIkey"
task :hola do
  puts "hola MIkey"
end

end

namespace :db do
  desc 'migrate changes to your database'
  task migrate::environment do
    Student.create_table
  end

desc 'seed database wih some data'
task seed::environment do
  require_relative '.db/seeds'
end

end

task :environment do
  require_relative './config/environment'
end

desc 'drop into pry console'
task console::environment do
  Pry.start
end
