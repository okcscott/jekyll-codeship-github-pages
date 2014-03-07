require 'tmpdir'

desc "Generate jekyll site"
task :generate do
  puts "## Generating Site with Jekyll"
  system "jekyll build"
end

desc "Generate and publish blog to gh-pages"
task :publish do
  Dir.mktmpdir do |tmp|
    system "mv _site/* #{tmp}"
    system "rm -rf *"
    system "mv #{tmp}/* ."    
    system 'git config --global user.email "scottwlesser+codeship@gmail.com"'
    system 'git config --global user.name "Scott Lesser - Codeship"'
    system "git add ."
    puts "## Git Status"
    system "git status"
    # system "git commit -am 'Codeship Update'"
    # system "git remote add ghub git@github.com:okcscott/jekyll-codeship-github-pages.git"
    # system "git push -f ghub master:gh-pages"
  end
end