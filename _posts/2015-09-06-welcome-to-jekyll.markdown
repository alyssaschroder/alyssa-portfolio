---
layout: post
title:  "Welcome to Jekyll!"
subtitle: "Feel home!"
date:   2015-09-06 23:34:01
categories: []
---
You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll’s dedicated Help repository][jekyll-help].

[jekyll]:      http://jekyllrb.com
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-help]: https://github.com/jekyll/jekyll-help



each post will be an image.
wich gallery does it go in? choose based on category.
setup category galleries
main "gallery" topnav links will filter posts by category

site.posts

if each image is a post... you have a lot of posts to upkeep... and you dont want to click into pages just containing an image... what if each gallery grabs the list of images from an associated post... then all she has to do is update the imageurl in the corresponding post to include it in the gallery

an image has a thumbnail, a full size, and a caption, and a title

since imaes have a bunch of metadata... just have her create a "post" for a single image in the gallery