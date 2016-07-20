---
layout: post
title: Seeding a Database
category: OpenCourseWare
tags: Instruction Seeding Rails
---

* content
{:toc}

I wanted to make a series of posts detailing various types of tree structures to organize data logically, but thought it would be too early without an explanation on seeding your database. Seeding a database is a basic tool we can use to add data to a database. It would be nuts to build an application without seeing where data goes and how it fits. Gems like faker are great tools to populate data automatically. I will also go into a bit about fixtures and the rake command.




#### How Seeding Works

Seeding a database is a piece of cake. Just open up `db/seeds.rb` and treat it like a normal ruby program in the rails environment. I am going to use a tree to organize some phylogenetic biology data. If you do not remember, those are the trees used to organize living things. So for an amoeba, which is that funky blog like micro-organism we would have:

> Eukaryota > Amoebozoa > Tubulinea > Loboda > Tubulinda > Amoebidae > Amoeba > Proteus

This is complex, and hard for us to read, so I will just make up some simple data that goes one or two levels down. We'll have a broad category of Animals, Plants and Micro-organisms. Animals will be subdivided into Reptiles, Birds and Fish. Plants will be subdivided Flowering and Non-flowering, and Micro-organisms won't have any subdivisions at all. How you organize this data is the subject of the tree structure series, but we do have a bunch of names. So let's seed a database of names.

First we need to generate our model in Rails

> $ rails g model Tree name:string

> $ rake db:migrate

Then we add some data!

db/seeds.rb

	tree_list = [
	
	  "Animals",
	  "Plants",
	  "Micro-organisms",
	  "Reptiles",
	  "Birds",
	  "Fish",
	  "Gecko",
	  "Alligator",
	  "Iguana",
	  "Chicken",
	  "Blue Jay",
	  "Shark",
	  "Tuna",
	  "Dog Fish",
	  "Catfish",
	  "Amoeba",
	  "Algae",
	  "Phytoplankton",
	  ]

	tree_list.each do |phylum|
	  Tree.create( name: phylum )
	end

Then we seed the db with

> $ rails db:seed

Pretty simple, all we're doing is writing out some strings, and throwing them in a dot each do. But this took me a few mintues. I could not think of these all quickly, and did not want funky data. Like where would Whales go? I did not leave room for those. Micro-organisms was also Bacteria, until I realized I did not know any bacteria off the top of my head.

###### Faker

In many common instances should save ourself some trouble and use Faker. We cannot get the same logic we could in our made up data, but we can create all sorts of things like addresses, names and universities.

> $ gem install faker

> $ bundle install

Open up db/seeds.rb

	99.times do |n|
	  name  = Faker::Name.name
	  Tree.create!(name:  name)
	end


###### Fixtures

While we are on the subject of creating dummy data, fixtures are used to create dummy data for testing. One of the more prominent gems is factory_girl_rails.

