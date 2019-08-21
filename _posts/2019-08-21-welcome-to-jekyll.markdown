---
layout: post
title:  "Hello World! From Jekyll on GitHub Pages"
date:   2019-08-21
---
# Hello World from Jekyll + GitHub Pages

In the next few weeks I will be rebuilding a few of my websites from the ground up. New hosts, new backends, and new frontends.

Lately I've been blogging a bit for my tutoring website (simontutors.com) so I figured I'd start a blog on something a bit more personally interesting i.e. not business related. The purpose of this blog is for me to document my thought process as I go through my build steps. I want to be able to reflect on my decision making. I normally do this in a notebook but I seem to be able to get more words out when I'm typing.

## Requirements:
- write in markdown
- be able to develop locally and also edit through a web browser
- cheap as possible
- decently fast without much, if any, configuration

## Solution:
Since this is going to be about my web development/coding/programming projects I figured GitHub Pages would be perfect. And since its all going to be code related a GitHub.io wouldn't seem out of place either. So free hosting, free domain. #free.99

GitHub Pages supports Jekyll and also builds/deploys it on their servers so I'm going to be using that as well. I used Jekyll a long time ago so I'm familiar with the file structure, so all I need is some boilerplate code to get started and customize after.

## Build steps:
1. Make sure dependencies are installed
    1. xcode-select --install
    2. 
2. Clone someones starter files because it's too much work to set it up all from scratch
3. Change the styles to something of my tastes
4. About page
5. Analytics


1. Install jekkyk
xcode-select --install

2. Ruby install
Ruby -v returns ruby 2.3.7p456 (2018-03-28 revision 63024) [universal.x86_64-darwin18]

3. Install bundler sudo gem install bundler

4. Cd desktop
Mkdir simonhowlader.github.io
Cd there
Touch Gemfile









Lately I've been blogging habit for my tutoring
 rebuild a few of my websites from the ground up.
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


Ruby version 2.4.0 or above, including all development headers (ruby version can be checked by running ruby -v)
RubyGems (which you can check by running gem -v)
GCC and Make (in case your system doesn’t have them installed, which you can check by running gcc -v,g++ -v and make -v in your system’s command line interface)

/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install Homebrew
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# Install rbenv and ruby-build
brew install rbenv

# Setup rbenv integration to your shell
rbenv init

# Check your install
curl -fsSL https://github.com/rbenv/rbenv-installer/raw/master/bin/rbenv-doctor | bash

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
