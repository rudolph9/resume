
task :default => [:compile_resume]

task :compile_resume do 
  puts system("pdflatex -output-directory=bin/ resume-rudolph_kurt.tex")
end

task :compile do
  puts system("pdflatex -output-directory=bin/ #{ARGV[1]}")
end
