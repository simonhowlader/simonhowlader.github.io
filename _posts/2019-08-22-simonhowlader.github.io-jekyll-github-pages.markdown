---
layout: post
title:  "SimonHowlader.github.io: Jekyll + GitHub Pages"
date:   2019-08-22
---

## Background and requirements:
I need a blog where I can document my progress as I work on various web development projects.

I currently have two websites that are both a work in progress. One is for an online course built on Wordpress and the LearnDash plugin and hosted on Flywheel. Another is a blog built on Ghost, which also used to be built on WordPress. I'm going back to WordPress but I will be combining both with a multisite configuration. One of them will also be using Gatsby.js and Netlify for the frontend. The past couple of weeks I have been researching to figure out the best webstack and I've had to do a lot of thinking about each project's requirements. The configuration is going to be complicated.

I've also been meaning to relaunch my personal website simonhowlader.com for a few months and start working on some web applications. All to say, I am going to need a way to document my build steps and my reasoning for different webstacks when I ineviotably start asking myself why I went with one technology over another. Lately I've been keeping that kind of info in a physical notebook, but now I want to write about it and keep that info online. So another blog.

After I have a bunch of content I will look into a commenting system. Blog posts will need to display code snippets in an elegant way. I also need to be able to create content as simply as possible.

- blog support
- be able to write in markdown
- syntax highlighting
- static
- be able to develop locally and also edit through a web browser
- cheap as possible
- relatively fast

## Solution:
The cheap part of my brain had me considering a simple ghost installation on Digitial Ocean, or a wordpress.com website, or blogger. But then I remembered Github Pages. It's static, uses Jekyll which I have some experience with, and it uses markdown. It's free (minus the domain name), but then I considered just keeping it free and going with a github.io domain since it would be appropriate for the type of blog posts I will be writing. I'm also going to be more deligent about keeping my code version controlled and pushing to GitHub pages.

I've used WordPress and Ghost CMS for a couple of other projects. They both have more features than I need for a simple blog. I've used hosting solutions such as nosupportlinuxhosting.com, FlyWheel, InMotionHosting, Digital Ocean, and GitHub Pages. NSLH costs a dollar per month but its SSL support is sketchy, they don't have automated backups, and it is slow. FlyWheel is only for WordPress and I'm not a fan of their chat based customer support, but mainly I dont't need to use WordPress for this simple side project. InMotionHosting had awesome customer support, but I know I won't need any customer support for a simple blog. Digitial Ocean is great at around 5 dollars a month, but I don't need a dedicated vps for a simple blog. GitHub pages is great for static content (like a blog) but it doesn't have a built in comment system like WordPress. I can use Disqus or a similar service if/when I want to integrate comments but for now it's not a priority. For now I just need a place to generate content that I can access from anywhere. I also like the sound of a personal webdev blog on a github.io domain, and I plan on hosting all of my code on GitHub anyways so GitHub pages sounds great.


GitHub Pages officially supports Jekyll and also builds + deploys it on their servers so I'm going to be using that as well. I used Jekyll a few years ago so I'm familiar with the file structure, so all I need is some boilerplate code to get started and customize after. GitHub Pages supports Jekyll, markdown, and sass preprocessing. Their servers are reliable, and relatively quick to serve content. I can also edit and write posts through a browser. And of course it's all version controlled. After I have something like 30 posts I will work on the look of the website but now something minimalist with Syntax highlighting would be sufficient. When the blog has more content I will probably be more inclined to create a more personalized design. Until then, content is priority. When I need to do more complex development work I can pull the github repository and work on it locally with a local Jekyll install.

## Build steps:
1. First I made a GitHub repository and named it simonhowlader.github.io
> Naming a repository with your username followed by .github.io tells GitHub to process the respository through Jekyll and host it on GitHub pages

2. Next I created a "\_config.yaml" file in the root directory and set a theme variable to "minima"
> Minima is Jekyll's default theme. I like the minimalist design and it seems to almost exactly what I wanted my blog too look like. I will change the look of the website in the future, but for now this is sufficient. Since the theme is set to minima, Jekyll uses the default theme files (https://github.com/jekyll/minima). Any files or folders that I create will overwrite the minima files/folders of the same name.
 
``` YAML
title: SimonHowlader.github.io
email: simon@simonhowlader.com
description: A blog for me to document my progress as I work on various web projects.
url: "https://simonhowlader.github.io"
github_username:  simonhowlader


# Build settings
markdown: kramdown
theme: minima
plugins:
 - jekyll-feed
 - jekyll-seo-tag
```
3. Next I created an index.md file with the following piece of code
> GitHub Pages requires an index.html file in order to know that the repository is meant to be hosted as a website. Jekyll will convert the index.md file into index.html file after processing it through the "home" layout of the minima theme.
``` YAML
---
layout: home
---
```

4. I then created an about page by creating a file named about.md.
> Jekyll converts markdown files to html files through the use of kramdown.

5. Finally I created a "\_posts" folder to create my first post (this one).
> Jekyll uses the naming convention, YYYY-MM-DD-title-of-my-post.md, to generate the permalink and sort your posts.
This post is named "2019-08-24-simonhowlader.github.io-jekyll-github-pages.markdown"


{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}
