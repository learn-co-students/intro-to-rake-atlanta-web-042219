
namespace :greeting do 
desc 'outputs hello to the terminal'
task :hello do
  puts "hello from Rake!"
end

desc 'output hola to the terminal'
task :hola do 
  puts "hola de Rake!"
end

end


task :console do
  puts "Make sure you have a 'console' rake task"
end 

namespace :db do 

desc "migrate"
task :migrate => :environment do
  Student.create_table
end

task :environment do
  require_relative './config/environment'
end

task :seed do 
  require_relative './db/seeds.rb'
end

end

