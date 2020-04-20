---
layout: post
title:      "Adobe XD: Wireframe and ideate portfolio projects"
date:       2020-04-20 01:02:14 +0000
permalink:  adobe_xd_wireframe_and_ideate_portfolio_projects
---


Building your first Sinatra app soup to nuts can be DAUNTING.  Like many students in this program, it was my first time developing a true "full stack" application.  And like many students, figuring out where to start can paralize your efforts before you even begin.

* What domain should I explore?  Can I build something unique?
* What are the models going to be?  Crap, do I even remember how to make all the migrations for this?
* So many views, so many controller actions...this is going to take forever, will I even finish this?

You get it, the list goes on and on.  BUT, here's a spoiler alert, you'll eventually figure it out and hopefully build an awesome app, one step at a time.

One tool/technique that helped me get my project off the ground was using [Adobe XD](https://www.adobe.com/products/xd.html) to wireframe out my app and think through my views (and the models it would need).  **This was an especially helpful process when it came to managing all the views/controller actions I'd need to create.**

**DISCLAIMER:**  I have a design background, so mocking things up in XD is nothing new to me.  But you don't need a design background whatsoever to make helpful wireframes.  For quick projects in the past, I've just simply sketched out ideas on a notepad.

Here's a quick rundown of my process of mocking things up in Adobe XD (I'll link some screenshots for each step so you can see what I did for my Sinatra App wireframes)

1.  The one pre-requisite I recommend before you start is figuring out what domain you want to explore.  In my case, I wanted to develop a simple fitness application built around quick 15 minute or less workouts.  (Becuase you know, I've been super bad at working out since the whole Corona virus thing...)

2.  [Start with the login and sign up process](https://raw.githubusercontent.com/ottocedeno/solocize/master/public/images/Screen%20Shot%202020-04-19%20at%208.21.54%20PM.png)  Follow the user's journey from start to finish.  Start with the signup form.  This is an easy one to help build momentum/confidence as theres only a few things you need from your users at this time.  **PRO TIP:**  Have fun with colors, typography here.  This is a good step to explore some design styles for your app if you're going to be adding in CSS to your project.

3. [ Your "main page" after a user logs in.](https://raw.githubusercontent.com/ottocedeno/solocize/master/public/images/Screen%20Shot%202020-04-19%20at%208.23.42%20PM.png)  In my case, the index view for the workout controllor was going to be the "central" place where my users would interact with the application.  This for me was one of the harder parts of my project because I had to really think about what data was most important for the user to see, what order and how to group it all.  Mocking it up in XD first helped me sort all that out before a single line of code was written.

4. Move on to some of your "show" views.  (see previous link in #3 to see a sample show view I made).  Once you get a sense of layout, typography, colors, etc, try to use the same design principles on a new page.  For me, setting up some "design rules" aka "design systems" helps me prototype faster too.  For example, once you establish what your links, buttons, headers, etc will look like for one page, you in theory should just repeat that for your other views.

5. [Forms.  Dreaded forms. ](https://raw.githubusercontent.com/ottocedeno/solocize/master/public/images/Screen%20Shot%202020-04-19%20at%208.24.02%20PM.png) I don't know about you, but I find forms (both designing and coding) very hard.  I get overwhelmed thinking about what data I want from my user, what order I want it in and what type of HTML inputs I want to use to get all that.  I think if there was only one view you used some wireframing techiniques for, use it for forms.

6. [Rinse and repeat for all your views.](https://raw.githubusercontent.com/ottocedeno/solocize/master/public/images/Screen%20Shot%202020-04-19%20at%208.28.02%20PM.png)  I know it's tedius, but trust me, it will help.  Mock up the rest of the views you think you're going to need.  Again, it's a great exercise to a) help you keep track of your views and routes but also b) stress test your models and database.  You might get to a wireframe and realize, "oh crap, I need to persist a new piece of data in order to achieve this."  Better to find out problems early and often

By the way, while I suggest doing wireframes in the beginning of your project, you should 100% still develop it from the ground up (database => models => controllor/views).  I don't recommend going from wireframes straight to coding your views.  You'll end up having to stub out / hard code in temporary values before your database is setup.  This just creates double work.

If you want to see my final product, you can find it here:  https://github.com/ottocedeno/solocize (**DISCLAIMER**:  My CSS is ALL OVER THE PLACE.  I'm still getting the hand of writting susinct styling rules.  Will most likley iterate over it and use a framework like Tailwind or Bootstrap)
