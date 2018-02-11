require 'html-proofer'

task :clean do
  system "rm -rf _site"
end

task :check do
  system "bundle exec htmlproofer ./_site --check-html --disable-external"
end

task :build => [:clean] do
  system "bundle exec jekyll build"
end

task :build_dev => [:clean] do
  system "JEKYLL_ENV=development bundle exec jekyll build"
end

task :build_prod => [:clean] do
  system "JEKYLL_ENV=production bundle exec jekyll build"
end

task :watch do
  system "bundle exec jekyll build --watch"
end

task :serve do
  system "bundle exec jekyll serve"
end
