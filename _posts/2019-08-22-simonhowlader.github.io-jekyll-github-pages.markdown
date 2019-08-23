---
layout: post
title:  "SimonHowlader.github.io: Jekyll + GitHub Pages"
date:   2019-08-22
---

## Background:
I need a blog where I can document my progress for various web development projects. I've used WordPress and Ghost for a couple of other projects. They both have more features than I need. I've used hosting solutions such as nosupportlinuxhosting.com, FlyWheel, InMotionHosting, and Digital Ocean. I don't want to deal with hosting if I can avoid it. I just need a solution that let's me easily write blog posts, preferabbly in Markdown, has styling support via CSS, secure, and is relatively quick to load. Cheaper the better. The design of the overall website doesn not matter as long as the content is legible. After I have something like 30 posts I will work on the look of the website, for now something minimalist with Syntax highlighting would be sufficient. 


## Requirements:
- be able to write in markdown
- be able to develop locally and also edit through a web browser
- cheap as possible
- relatively fast

## Solution:
Since this is going to be about my web development/coding/programming projects I figured GitHub Pages would be perfect. And since its all going to be code related a GitHub.io url wouldn't seem out of place either. So free hosting, free domain. #free.99

GitHub Pages supports Jekyll and also builds/deploys it on their servers so I'm going to be using that as well. I used Jekyll a long time ago so I'm familiar with the file structure, so all I need is some boilerplate code to get started and customize after.

## Build steps:
1. Make a GitHub repository named simonhowlader.github.io
2. create a "\_config.yaml" file.
3. ``` YML
title: SimonHowlader.github.io
email: simon@simonhowlader.com
description: >- # this means to ignore newlines until "baseurl:"
  A blog for me to document my progress as I work on various web projects.
baseurl: "" # the subpath of your site, e.g. /blog
url: "https://simonhowlader.github.io" # the base hostname & protocol for your site, e.g. http://example.com
github_username:  simonhowlader


# Build settings
markdown: kramdown
theme: minima
plugins:
  - jekyll-feed
```


4. About page
5. Analytics

##Background
I currently have two websites that are both a work in progress. One is for an online course built on Wordpress and the LearnDash plugin and hosted on Flywheel. Another is a blog built on Ghost, which also used to be built on WordPress. I'm going back to WordPress but I will be combining both with a multisite configuration. One of them will also be using Gatsby.js and Netlify for the frontend. The past couple of weeks I have been researching to figure out the best webstack and I've had to do a lot of thinking about each project's requirements. The configuration is going to be complicated.

I've also been meaning to relaunch my personal website simonhowlader.com for a few months and start working on some web applications. All to say, I am going to need a way to document my build steps and my reasoning for different webstacks when I ineviotably start asking myself why I went with one technology over another. Lately I've been keeping that kind of info in a physical notebook, but now I want to write about it and keep that info online. So another blog.

##Requirements
>for blogging
>markdown suport
>syntax highlighting support
>static
>browser interface for uploading content and editing
>cheap

##The stack
The cheap part had me considering a simple ghost installation on Digitial Ocean, or a wordpress.com website, or blogger. But then I remembered Github Pages. It's static, uses Jekyll which I have some experience with, and it uses markdown. It's free (minus the domain name), but then I considered just keeping it free and going with a github.io domain. I'll like back to it from my simonhowlader.com website, but I don't need my coding projects to take the center stage of what people know about me. They can find it of course as I'm not trying to be anonymous. But this can always be changed.

I want to devvelop the site locally and then push it Github, but if I ever need to make small adjustments I want to be able to do that through the web interface. I want to use Jekyll because it's what Github pages recommends and has the best support for. I could use Hugo or a number of the other static site managers but with Jekyll I also have sass support and for the most part they all do the same main things and I'm just trying to launch a simple blog.

Step 1: Read the Jekyll docs
https://jekyllrb.com/docs/installation/macos/
Step 2: Install Jekyll locally



, one built with wordpress, and another built with Ghost. For the next few weeks I am planning on rebuilding two different tutoring websites with a headless cms approach, and restarting my personal website. There's going to be a lot of custom configuring and I want to create some sort of documentation for it incase I ever need to go through it again. I don't want to repeat my research and I want to know
I'm refactoring a lot of my code and restarting a bunch of web development projects. As I build/rebuild them from "scratch" I want to document my decisions and the structure of my projects.
I want to start blogging about my various projects as I begin working with them. I want to document my thought



{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}
