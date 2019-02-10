require 'html-proofer'
require 'dotenv/tasks'

desc 'it provides a short alias for dev_serve'
task :s do
  Rake::Task['serve'].invoke
end

desc 'it runs a dev server with a sensible base URL'
task :serve do
  sh 'env LIVE_BRANCH=$(git rev-parse --abbrev-ref HEAD) hugo -d /var/www/msitb -w --baseURL="//go.grz.li/msitb"'
end

# Deploy. Depends on the build and s3_push tasks
desc 'it deploys the site with current posts'
task :deploy do
  Rake::Task['build'].invoke
  Rake::Task['s3_push'].invoke
end

### BUILD
desc 'it builds the site with current posts'
task :build do
  sh 'hugo'
end

### S3_PUSH
desc 'it pushes the generated site to s3 and Cloudfront'
task s3_push: :dotenv do
  sh 'bundle exec s3_website push'
end

### HTML_PROOF
desc 'it checks validity of the generated HTML'
task :html_proof do
  Rake::Task['build'].invoke
  options = { assume_extension: true,
              http_status_ignore: [999],
              internal_domains: ['flyinggrizzly.net',
                                 'www.flyinggrizzly.net'] }
  HTMLProofer.check_directory('./public', options).run
end
