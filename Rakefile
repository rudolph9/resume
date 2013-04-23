gem 'highline'; require 'highline/import'
require 'fssm'
require 'pry'

task :default => [:compile]

task :compile do 
  file = ARGV.last
  puts file
=begin
  pid = Process.spawn( 'latex',
                      '-output-directory=bin/',
                      '-output-format=pdf',
                      file , out: STDOUT, err: STDOUT)
  #Process.kill(:QUIT, pid) && Process.wait
=end
  puts system( "latex -output-directory=bin/ -output-format=pdf #{file}")
  # to avoid error; creat a task with same name as last argument
  task file.to_sym do ; end 
end