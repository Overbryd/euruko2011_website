desc "Create a new post"
task :post do
  if ENV['title'].nil? || ENV['title'].strip.empty?
    puts 'usage: rake post title="YOUR TITLE"'
    exit(1) 
  end
  
  title = ENV['title']
  filename = Time.now.strftime('%Y-%m-%d') + '-' + title.scan(/\w+/).join('-').downcase + '.md'
  post = <<-POST
---
layout: post
title: #{title}
---

POST
  
  File.open("_posts/#{filename}", 'w') { |f| f.write(post) }
  sh "mate _posts/#{filename}"
end