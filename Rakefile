require_relative "lib/student.rb"
require "pry"

task :environment
require_relative "config/environment.rb"

namespace "greeting" do

	desc 'outputs hello to the terminal'
	task :hello do
	  puts "hello from Rake!"
	end

	task :hola do
		puts 'hola de Rake!'
	end
end

desc "console"
task :console do
	#
end

namespace :db do
  desc 'migrate changes to your database'
  task :migrate => :environment do
    Student.create_table
  end

  task :seed do
 
	Student.create(name: "Melissa", grade: "10th")
	Student.create(name: "April", grade: "10th")
	Student.create(name: "Luke", grade: "9th")
	Student.create(name: "Devon", grade: "11th")
	Student.create(name: "Sarah", grade: "10th")
  end
end
