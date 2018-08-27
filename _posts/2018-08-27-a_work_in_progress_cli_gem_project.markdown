---
layout: post
title:      "A Work in Progress... CLI Gem Project"
date:       2018-08-27 23:04:35 +0000
permalink:  a_work_in_progress_cli_gem_project
---


Well I made it to the CLI Gem Project and to say I was completely ready for it wouldn't be an understatement but possibly a bit close. I will do my best to chronicle my good acheivements and major mistakes during the process below. 

**Picking a site to scrape:**

I'll have to say, sometimes my heart moves much faster than my mind. I originally picked SoundCloud.com. The site and idea of what I wanted to do had meaning to me. But I then ran into a slight snag. My idea would have been to scrape my personal feed and reorganize tracks by likes and/or plays. So the key phrase is "personal feed." To do such a task, I would have to know how to utilize Oauth2 framework at which I have not learned as of yet. So that idea had to be tabled for a later date. Point of this information, make sure you read all documentation given before starting project. If I had done so, I would have realized sites that require authorization are most likely not the best sites to scrape for your first project. 

I then decide to go with a second favorite of movie trailers. I picked IMDB.com/trailers. Keep in mind, I lost about 2 1/2 days attempting to make the SoundCloud work so once I moved on to IMDB, I had a lot of catching up to do. 

**Starting the project:**

Be sure to review all suggested videos before starting this project. Don't let the heart move faster than the mind as I did. Those words are probably the best advice I can give concerning this or any project in programming. 

When you follow the videos/instructions, things progress at a good pace. Started working on just writing some code based around the simplest part of my idea which would be the CLI file. I liked how Avi states in those videos, "begin writing the code for what you want your program to do" or something like that. 

Once I got a basic CLI working, I moved on to scraping the IMDB page. There were a few hurdles in that when I went to scrape the trailer page, a lot of the information wasn't bundled in containers but imbedded in an image file. Really didn't know how to immediately fix but through PRY and remember some simple ruby methods I was able to get to the movie titles. `titles = doc.css(".trailer-caption").children.text.split("\n ").reject{|t| t.empty? || t == "   "}` This pulled all of the titles on the page as one long string that I had to split and then still remove extra character spaces. It is not pretty but the code does work. As I progress through more scraping I know there is a way that it could be refractored now. I have not attempted to do as of yet. I'll update blog once I do. 

**Bringing it all home**

Once i had my scraper class working, things just started flowing together. Added more to my CLI file to have it print out what I wanted which was the list of movie titles. Once that list printed, you could select one by corresponding number and it would then print out: movie title, year, director, genre, brief summary and the link to the trailer. 

One of the hardest parts was getting my second scrape of the individual movie's page to line up with my movie objects that were already created. the movie objects were being initialized with the title, trailer url and the url to the individual movie's page. To add that info from the movie url, I had to create a doc method and methods for each of the elements i wanted to scrape. The doc method had an instance variable set equal to Nokogiri and Open-Uri pulling on the self of the movie url. All the other methods were also instance variables set equal to the scraping code to find those items. I then have a find method that when invoked in my CLI class will pull the specific movie info. Probably not explaining in the best way but it works. Had to add the find method. At first I didn't have a find method so it was randomly pulling info. I would have the movie Meg but the summary for Crazy Rich Asians. That was blowing my mind for a bit. 

Now that it was fixed, the project was basically done. I attempted to refractor some of the code and cleaned it up a bit to look nice and uniform. Just have to put some final touches in README.md and gemspec file and I believe I'm done. 

**Best thing I learned**

As I stated above, the best thing you can do when starting this project, go through all materials and references given. Read it all!! Go back to old labs and brush up on any area you're unsure about. Sometimes it's hard to see that you have been given 90% of the information and tools you will need, but it's there. 


