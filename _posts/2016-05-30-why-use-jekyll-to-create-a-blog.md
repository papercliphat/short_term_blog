---
layout: post
title: Benefits of Jekyll in Static Apps
category: Jekyll
tags: Jekyll StaticApp
---

* content
{:toc}

Jekyll is a static site generator written in Ruby. That means you can use it for blogs, business websites and anything else you can imagine that mostly doesn\'t require a database. It takes dynamic content like templates and markdown and assembles that content into a static application. The assembled static application is what gets put on the web. Using this method we can take advantage of paradigms in programming<sup>1</sup> to easily and rapidly make changes to our application.





### The Pros

Jekyll is pitched and touted as being very minimalistic and very efficient. It has only what you need to generate a basic static site. Everything else you have add via plugins. The benefits to this approach are that Jekyll is very fast, very secure and very cheap right out of the box<sup>2</sup>. Additionally, because it\'s so simple, it\'s fairly easy to optimize code for speed and efficiency.

If you need log-in, extensive commenting, photo hosting or hosting any type of data you should definitely move out of Jekyll and into a webapp framework that supports databases like Ruby on Rails, PHP, or Python to name a new.

### The Cons

I consider these inconveniences inherent in the type of framework Jekyll is, but with enough inconveniences, we get a bit unhappy.

Photos and media have to be inserted manually. With some sites like Wordpress, there is a nice interface to easily add this kind of data. Jekyll doesn\'t have that, so if we\'ve got a dozen photos per post, it might be a good idea to consider switching.

SEO optimization generally has to be done manually. SEO optimization gets webapp pages hitting higher on unpaid search results. There are a lot of factors to take into consideration, but generally optimization relies on good keywords, inter-application cross-linking and easy social network sharing. There are some Jekyll plug ins that help, but I don\'t use them. For me, this is more of a personal body of work blog, and I don\'t think it would be an optimal use of my time.

Jekyll only works on computers where you are "set-up". So if you\'ve got a laptop you do most of your work on, and a light weight underpowered mini-laptop for traveling, you would likely find it difficult to update or edit your website on the road. 

### The Competition

#### Wordpress

Today, the biggest webapp framework is definitely Wordpress. A lot of folks knock it for it\'s resource use, but it\'s huge strength is in it\'s interface. Anyone can easily create a website on wordpress with virtually no programming knowledge. Additionally, the more difficult to do things like handling database log-ins and tarnsactions can be done with plugins. It\'s really easy to use and you can find a TON of sites that use Wordpress like The New York Times.

Wordpress works out of a browser and it has a simple editing system, but it is slower. It\'s also more prone to crashes and MUST be continuously updated. Security holes in plugins are constantly being found and updated. Because of these security holes, and popularity there is also got a malware situation. Malware might get inserted into your site if you aren\'t constantly updating, and then you might run into anti-viruses programs warning users of your site, loss of users trust and possibly SEO de-optimization<sup>3</sup>.


#### Alternative Popular Static Site Generators

Middleman - Also built in Ruby, but smaller than Jekyll. Some major websites use Middleman and if it works for them it can work for us.

Roots - Node.js based, built by Carrot which is a subsidiary of the Vice Media Group.

Hugo - Written in GO. I\'ve been hearing a lot of love for Hugo, but it might be because it\'s the new kid on the block.

If you are having trouble choosing a Static Site Generator and don\'t don\'t have any coding experience I\'d just pick Jekyll or Wordpress. It\'s more important to get started and work through the fundamentals, than spending significant time researching for very small gains. The larger frameworks also have more tutorials, guides, plug-ins and overall resources at your disposal.

If you do have skill in Node.js, GO or another language you should definitely use the static site generator in that language. With a quick google search you can find a framework that supports your language of choice. Additionally, you shouldn\'t have any trouble finding tutorials to get you started.

##### Footnotes:

1. Paradigms include things like DRY - Don\'t repeat yourself. If you are repeating yourself over several sections, and you decide to make a change, you now have to make this change over several sections. This is both error prone (typos) and time consuming.

2. Becuase we have no communication between databases we are fast. We are just pulling up already prepared data quickly. Jekyll comes out of the box without plugins, which may be a source of continuous updating to patch security holes. Additionally, because Jekyll is already prepared when it\'s hosted, there isn\'t much to change. It\'s often the ability to be dynamic that presents security holes. With no databse, Jekyll is small and light. That means cheap. It also means we aren\'t sending a lot of data. That also means cheap. Cheap on space and cheap on sending data = very cheap.

3. SEO optimization is sort of like a hidden black box. Search engines don't publicly say all the ways they use to choose site rankings, but they tell us some of them and we get an impression of others. It\'s a likely case that sites with security warnings, suffer de-ranks, but it\'s unclear how severe those security issues have to be or how long. 