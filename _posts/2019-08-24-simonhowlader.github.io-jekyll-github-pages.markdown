---
layout: post
title:  "SimonHowlader.github.io: Jekyll + GitHub Pages"
date:   2019-08-24
---

## Background and requirements:
I need a blog where I can document my progress as I work on various web development projects.

I currently have two websites that are both a work in progress. One is for an online course built on WordPress and the LearnDash plugin and hosted on FlyWheel. Another is a blog built on Ghost CMS and hosted on Digital Ocean. Both projects will be combined onto a WordPress multisite installation with seperate frontends. The past couple of weeks I have been researching to figure out the best webstack for each project's requirements. The configuration is going to be complicated.

I've also been meaning to relaunch my personal website simonhowlader.com for a few months and start working on some web applications. All to say, I am going to need a way to document my build steps and my reasoning for different webstacks when I ineviotably start asking myself why I went with one technology over another. For the past few years I've been keeping that kind of info in a physical notebook, but now I want to write about it and keep that info online. I think that keeping a "public" record of my projects and milestones will help me be more productive by keeping myself accountable.

After I have a bunch of content and projects completed I will start thinking more about the functionality and design of the website. For now I just need a simple way to publish content in a safe and reliable manner. Things sush as a commenting system, SEO, and a personalized theme are going to be tasks for a much later time. I still want my posts to be presentable, at the vvery least for myself. My posts will have snippets of code so Syntax Highlighting is a must. 

- blog support
- be able to write in markdown
- syntax highlighting
- static hosting
- be able to develop locally in the future when I need to 
- edit and post through a web browser
- cheap as possible
- relatively fast

## Solution:

### free.99
The cheap part of my brain had me considering a simple ghost installation on Digitial Ocean, or a wordpress.com website, or blogger.com, but then I remembered Github Pages. It's great for static sites, uses Jekyll on their backend (which I have some experience with) and it uses markdown. It's also free (minus the domain name), but then I considered just keeping it free and going with a subdomain on github.io domain since it would be appropriate for the type of blog posts I will be writing. I'm also going to be more deligent about keeping my code version controlled and pushing to GitHub Pages so it just makes a lot of sense.

### Other hosts/solutions
I've used WordPress and Ghost CMS for a couple of other projects. They both have more features than I need for a simple blog. I've used hosting solutions such as nosupportlinuxhosting.com, FlyWheel, InMotionHosting, Digital Ocean, and GitHub Pages. NSLH costs a dollar per month but its SSL support is sketchy, they don't have automated backups, and it is slow. FlyWheel is only for WordPress and I'm not a fan of their chat based customer support, but mainly I dont't need to use WordPress for this simple side project. InMotionHosting had awesome customer support, but I know I won't need any customer support for a simple blog. Digitial Ocean is great at around 5 dollars a month, but I don't need a dedicated vps for a simple blog. GitHub pages is great for static content (like a blog) but it doesn't have a built in comment system like WordPress. I can use Disqus or a similar service if/when I want to integrate comments but for now it's not a priority. For now I just need a place to generate content that I can access from anywhere. 

### Jekyll support
GitHub Pages officially supports Jekyll and also builds + deploys it on their servers so I'm going to be using that as well. I used Jekyll a few years ago so I'm familiar with the file structure, so all I need is some boilerplate code to get started and customize later. GitHub Pages supports Jekyll, markdown, and sass preprocessing. Their servers are reliable, and relatively quick to serve content. I can also edit and write posts through a browser. And of course it's all version controlled. After I have something like 30 posts I will work on the look of the website but now something minimalist with Syntax highlighting would be sufficient. When the blog has more content I will probably be more inclined to create a more personalized design. Until then, content is priority. When I need to do more complex development work I can pull the github repository and work on it locally with a local Jekyll install.

## Build steps:
\1. First I made a GitHub repository and named it simonhowlader.github.io
> Naming a repository with your username followed by .github.io tells GitHub to process the respository through Jekyll and host it on GitHub pages

\2. Next I created a "\_config.yaml" file in the root directory and set a theme variable to "minima"
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

\3. Next I created an index.md file with the following piece of code

``` YAML
---
layout: home
---
```

> GitHub Pages requires an index.html file in order to know that the repository is meant to be hosted as a website. Jekyll will convert the index.md file into index.html file after processing it through the "home" layout of the minima theme.

\4. I then created an about page by creating a file named about.md.
> Jekyll converts markdown files to html files through the use of kramdown.

\5. Finally I created a "\_posts" folder and my first post (this one) with the name "2019-08-24-simonhowlader.github.io-jekyll-github-pages.markdown".
> Jekyll uses the naming convention, YYYY-MM-DD-title-of-my-post.md, to generate the permalink and sort your posts.
This post is named "2019-08-24-simonhowlader.github.io-jekyll-github-pages.markdown"
