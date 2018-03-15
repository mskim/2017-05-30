task :default => :pdf
task :pdf => Rake::FileList["**/output.pdf"]
files = Rake::FileList["**/output.pdf"]
puts files
rule "output.pdf" => "story.md" do |t|
  # folder = File.diranme("#{t.source}")
  # puts File.diranme("#{t.source}")
  # sh "cd #{folder} && newsman article .)"
  sh "newsman article #{t.source})"
end
