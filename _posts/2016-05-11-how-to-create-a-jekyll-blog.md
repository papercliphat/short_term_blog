---
layout: post
title: How to Create a Jekyll Blog
category: Blog
tags: Jekyll StaticApp HowTo
---

* content
{:toc}

This is less of a How to, and more of a let me point you in the right direction. Then I\'ll throw in a couple pointers on how you can make an identical site to mine. It\'s going to be light on content, mosty full of links, but if you\'ve never built anything in Jekyll it\'s helpful to have instructions on how to proceed.




#### Install Ruby

The first step to building a Jekyll Blog is to install Ruby!

Ruby has a some decent instructions at the [Ruby official site](https://www.ruby-lang.org/en/documentation/installation/).

I used RVM (Ruby Version Manager) to both manage and install Ruby. I\'ve never actually needed to use a specific Ruby version, but it was the easiest way to install Ruby on my system. We can visit [RVM's official site](https://rvm.io/rvm/install) for detailed instructions.

For additional help do a google search - something like "install ruby windows 10" or "install ruby fedora"

#### Install Jekyll

Jekyll installation is insanely quick once you get Ruby installed properly. With a quick trip to the [Jekyll official site](https://jekyllrb.com/) we can find all the info to get started.

Once Ruby is installed it, it\'s just opening up the console and typing: 

>$gem install Jekyll

The Jekyll website has all the information you need to get started writing posts, additional pages, linking, etc., so it\'s a worthwhile read.

#### A Few Pointers

Out of the box Jekyll comes with a simple some HTML and CSS included. If you don\'t like the appearance or want additional features consider exploring Jekyll Themes or Jekyll Templates with a quick google search. 

I use a [Jekyll theme](http://jekyllthemes.org/) from, which is pretty much just an aggregation site. I was a fan of both [Yellow Blue](http://jekyllthemes.org/themes/yellowblue/) and [WikiBlog](http://jekyllthemes.org/themes/wiki-blog/) . I wanted something with Categories and Tags included on the sidebar, and WikiBlog actually linked me to [Concise-high-end Theme](http://jekyllthemes.org/themes/cool-concise-high-end/). It\'s not in English, but I cleaned it up a little and removed some features to make it more to my liking. I have included what I used in my [github](https://github.com/papercliphat/concise_theme_jekyll) for English speakers.

##### Some Concise Theme Caveats

The tags feature requires at least two pages with different tags or it will through a divide by 0 error.

To utilize the excerpt of the full blog page, keep 3 empty rows between the excerpt and the main body of the content.

You\'ll have to install the Jekyll pagination gem or you will get an error for that too! Instructions can be found on [Jekyll's site](https://jekyllrb.com/)

Pagination limits the number of posts that appear on a page. If you want to add comments, your best bet is disquis, a quick google search of "disquis jekyll" will lead you on the right path.

Gaohaoyang does have a request for linking that the theme was created by him in the footer. I think that's asking a bit much for a Jekyll Theme. Additionally the general concensus is if it\'s out there for public use with an MIT license you can pretty much do what you want with it. Lastly, I\'m modifying and building on his work like all programmers do. At some point we have to draw a line between our work and our predecessors.
