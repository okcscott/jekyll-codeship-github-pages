require 'tmpdir'

desc "Generate jekyll site"
task :generate do
  puts "## Generating Site with Jekyll"
  system "jekyll build"
end

desc "Generate and publish blog to gh-pages"
task :publish do
  Dir.mktmpdir do |tmp|
    # system "mv _site/* #{tmp}"
    # system "git checkout -b gh-pages"
    # system "rm -rf *"
    # system "mkdir _deploy"
    # system "mv #{tmp}/* _deploy"
    # message = "Site updated at #{Time.now.utc}"
    # system "git add ."
    # system "git commit -am #{message.shellescape}"
    # system "git push origin gh-pages --force"
    # system "git checkout master"
    # system "echo yolo"
  end
end