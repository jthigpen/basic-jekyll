task :default => :server

task :server do 
  sh 'jekyll --auto --safe --server'
end

task :build do
  sh 'jekyll'
end

task :deploy => :build do
  sh 'rsync -avze ssh --delete _site/ username@hostname.com:path'
end
