---
layout: post
title:      "OMG... Finally Finished Rails Project!"
date:       2019-06-23 16:34:22 +0000
permalink:  omg_finally_finished_rails_project
---


**The Project:** Cura10 is a Top Ten list app. Users create top ten lists of images (currently) of varying categories from art to vehicles. Users can favorite their favorite lists and also up/down vote lists. 

**The Process:** Not sure where to begin but this took me way longer than I should have let it. Things started of well. I had the list idea and just started making it but I had yet to have my meeting with the Rails Project Section Lead. So I'm trucking along, checking off requirements and then realize I should probably have this meeting before I get too involved. I was already too involved. At this point I had working database, multiple views, facebook login, etc. So there was no turning back. 

Move forward to having my meeting at which I was on the right track but had 2 main requirements to complete. Was given good direction on how I could complete but still had to figure out on my own. These are the 2 requirements that knocked me down some terribly, I didn't think I would get up:
* The "through" part of the has_many through includes at least one user submittable attribute, that is to say, some attribute other than its foreign keys that can be submitted by the app's user (attribute_name e.g. ingredients.quantity)
* Include a class level ActiveRecord scope method (model object & class method name and URL to see the working feature e.g. User.most_recipes URL: /users/most_recipes)

Figuring these two requirements out was probably the hardest thing I had to do so far in the cirriculum. They don't look or seem that difficult but in how I had already begun my project, the user submittable attribute proved to be difficult. I decided to make my own voting system so user could up/down vote list. Sounds easy enough but truly was not. Not going to give away my secrets on how I got there but it was a lot of trial and error, Google, Stack Overflow, and coaches. Finally solved the issue of reaching attribute of join model and created up/down vote methods making it possible to do so and I was ecstatic! Mind you, this had taken weeks... well, not actual weeks because I'm self-pace and have a full-time career, but definitely all of the spare time out of my life and a bit of my soul. Haha. 

Now I have reached the second hurdle which was good ole Scope. I know why I had difficulty with this one though. Not of the bat but I realized shortly in that I probably shouldn't have rushed through SQL and/or things could have been more in-depth during ActiveRecord to give myself more of a base. This one was won in Rails Console. A lot of writing methods and testing immediately. One of my problems is that I was trying to write the end method without writing the smaller ones that would lead to it. Ended up doing a deep dive and learning more than I had about it all at that point. Learned some things that weren't in cirriculum like how you can chain scope methods on top of scope methods on top of more scope methods. Which was basically how I solved that problem. Yet again, taking way longer that I would have hoped but some humility was learned and it needed to happen in that way. 

All in all, though being my own toughest critic, I have checked all the boxes and am at a point of submittal. Yes, there is plently more I'd love to do to this and most likely will but it will have to wait because this guy is stepping away for at least a good weekend. 

If you like, you can check my repo [here](https://github.com/JustReggie2/cura10).

Special shoutout to: Mariam, Kev, and Dwayne! The support was very much appreciated. 


