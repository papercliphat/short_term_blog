---
layout: post
title: How to Create a Jekyll Blog
category: Jekyll
tags: Jekyll HowTo
---

* content
{:toc}

This is less than an expansive How To, and more of a let me point you exactly to the resources you need and explain why or how that resource is important. I\'ll throw in ways you can make an identical site to mine. If you\'ve never built anything in Jekyll it\'s helpful to have a step-wise guide on how to proceed.




#### Install Ruby

The first step to building a Jekyll Blog is to install Ruby!

Ruby has a some great step-by-step instructions at the [Ruby official site](https://www.ruby-lang.org/en/documentation/installation/). Find your operating system and get started. 

Warning: Ruby runs best on Ubuntu(Linux) and Mac. I've played with it in Fedora(Linux) and it wasn't as easy to install for me. It will install in windows, but there are some issues with running Ruby on Rails and... I think Javascript frameworks. I actually use a Windows PC with a virtual machine set up through VMware.

I used RVM (Ruby Version Manager) to both manage and install Ruby. I\'ve never actually needed to use a specific Ruby version, which is their touted feature, but it was the easiest way to install Ruby on my system. We can visit [RVM's official site](https://rvm.io/rvm/install) for detailed instructions.

For additional help do a google search - something like "install ruby windows 10" or "install ruby fedora", but be ready to wrestle with set up technical issues.

#### Install Jekyll

Jekyll installation is insanely quick once you get Ruby installed properly. With a quick trip to the [Jekyll official site](https://jekyllrb.com/docs/installation/) we can have an extensive installation guide.

The quick installation is <sup>1<sup>

>$ gem install Jekyll

>$ jekyll new my-site

>$ cd my-site

>my-site$ jekyll serve


Then go to http://localhost:4000 in your browser

The Jekyll website has all the information you need to get started writing posts, additional pages, linking, etc., so it\'s a worthwhile read.

#### A Few Pointers

Out of the box Jekyll comes with a simple some HTML and CSS included. If you don\'t like the appearance or want additional features consider exploring Jekyll Themes or Jekyll Templates with a quick google search. 

I something from [Jekyll theme](http://jekyllthemes.org/), which is an aggregation site. I was a fan of both [Yellow Blue](http://jekyllthemes.org/themes/yellowblue/) and [WikiBlog](http://jekyllthemes.org/themes/wiki-blog/). I wanted something with Categories and Tags included on the sidebar, and WikiBlog actually linked me to [Concise-high-end Theme](https://github.com/Gaohaoyang/gaohaoyang.github.io). It\'s not in English, but I cleaned it up a little and removed some features to make it more to my liking. I have included a blank template in my [github](https://github.com/papercliphat/concise_theme_jekyll) for English speakers. But spend some time exploring on your own for ideas you can build on.

##### Caveats of Concise-high-end Theme

The Concise theme "tag" feature requires at least two pages with different tags or you will get a divide by 0 error.

To utilize the excerpt of the full blog page, keep 4 empty rows between the excerpt and the main body of the content.

You\'ll have to install the Jekyll pagination gem or you will get an error for that too! Instructions can be found on the [Jekyll site](https://jekyllrb.com/docs/pagination/)

Pagination limits the number of posts that appear on a page. If you want to add comments, your best bet is disquis, which requires registration and was a bit too much hassle for me. If you want comments, a "disquis jekyll" google search will send you to a ton of videos and guides to assist.

##### Footnotes:

1. The $ denotes using the terminal aka console to type this code. You'll see it a lot while your programming, but for me on day 1, I didn't understand it.