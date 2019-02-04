---
layout: post
title:      "Sinatra Project - Kinda getting the hang of it"
date:       2019-02-04 01:14:35 +0000
permalink:  sinatra_project_-_kinda_getting_the_hang_of_it
---


So I've just completed my Sinatra project. Well, it's done outside of all the other stuff I'd still like to do with it. Saying that simply because once you start coding and making headway, you really just don't want to stop. At least I don't. 

Like my first project (CLI), I started with one idea and had to change it. Last time, I had to change because my idea required more knowledge than I had yet to receive. This time around, it wasn't due to my lack of knowledge but more to the guidelines of the project. My original idea, which I'm not going to divulge, would have likely fallen into something close to a blog. At which guidelines stated to not create something similar to a blog. Had the idea way before I saw guidelines but what are ya gonna do!?! Nonetheless, I scrapped that for later and came up with The Cannabis Cabinet. 

The Cannabis Cabinet is an MVC app that is basically your cannabis strain organizer. Users are able to create different cabinets to store their favorite strains. It follows CRUD for the cabinet objects. Not much else in description. Just your basic Content Management System. 

**Process:** So I struggled a bit at the start on where to start. Since, I'm a bit old school, I broke out my notebook and started writing out what I wanted this app to be. I knew it would have Users, Cabinets and Strains. But how was I to connect it all? The associations almost exploded my brain until I finally put together the need of a Join table. 

* A User has many Cabinets and many Strains through Cabinets
* A Cabinet belongs to a User and has many Strains through Cabinet_Strains
* A Strain has many Cabinet_Strains, has many Cabinets through Cabinet_Strains and many Users through Cabinet_Strains
* Cabinet_Strains belongs to Cabinets and Strains

Once I figured all that out, the coding began. I started with my database and getting my many migrations correct. There were about 10 or so because of some minor mistakes and corrections. Then once I had those up, I used Tux to verify that all my associations were correct. What a feeling that was when they were. On to the MVC of my MVC. 

I found this part of the project, not easy, but easier since I had just finish that section of the curriculum. Starting with my basic controller and index page, I just continued adding each piece. I do think I could have had a more direct approach as I was bouncing back and forth between my different views and controllers. I just felt my process on which view I was working on and then moving to could have been better thought out. 

All in all, I managed to get the app as a whole working with only a few hiccups. Like, forgetting to push up about 4 commits to Github and losing the work because my computer decided to crash at that perfect time. That was a fun lesson but I learned because of it. Add, commit, push (immediately)!!! I did do a lot of Googling, use many of references that I've collected along the way and referenced code from old labs. 

Being able to utilize all that I've learned so far and create a working and useful application is giving me the confidence in realizing that I am at this point I am a programmer. Yes, there is much more for me to learn and some areas that I know need improving (writing about my code comes to mind) but I'm pleased with my progress. 
