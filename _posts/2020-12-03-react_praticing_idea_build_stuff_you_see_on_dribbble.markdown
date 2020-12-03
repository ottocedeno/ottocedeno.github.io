---
layout: post
title:      "React Praticing Idea:  Build stuff you see on Dribbble"
date:       2020-12-03 22:29:42 +0000
permalink:  react_praticing_idea_build_stuff_you_see_on_dribbble
---


I was having a hard time trying to dial in my CSS skills, specifically with layouts, containers, responsiveness etc.  I watched YouTube videos / read random articles on Flexbox and Grid, but I usually find that the intro "easy projects" are not that compelling / real world examples you'd encounter at a proper tech start up.

For me, design is everything. It's the first impression the user has with the application.  So making sure I can build applications that look and feel like what you'd expect out of Google, UberEats, or AirBnB is mega important.

But this puts a lot of pressure to design something world class from scratch, and then implement it with your code.  It's also mega time consuming.  If your sole goal is to learn more CSS and practice building commercial looking front ends, here's your hack:

Go on Dribble, find some great looking UI from world class designers, pick one, and try to build it.

I've found this approach to be super fun and you can usually build the "above the fold" content fairly quickly.

I load out with the following tools:

* Gatsby (so I can take advantage of any Gatsby plugins that could help)
* React
* Tailwind (CSS Framework)
* Google Fonts plugin for Gatsby
* A random image generator (or use your own if you have dummy images in case the layout calls for pics)

Then I head over to [Dribbble](https://dribbble.com/) and start searching around.  Usually I start with "mobile UI", or "front-end UI".

I'm usually looking for something that has a great use of color, typography and a layout that looks moderately difficult.

*Note: for your first time trying this.  Go for a really simple layout just to get a win under your belt.  But after that find something that forces you to use at least Flexbox. (hard mode = Flexbox AND grid)*

## Getting Started

Ok so let's say we wanted to go with this layout idea for a [cool finance app](https://dribbble.com/shots/14210557-Finance-Mobile-Application-UX-UI-Design). 

I would probably practice just the first two views in this case as the third has some complex artwork which of course, we're not privy to.

IMPORTANT:  The goal isn't to make it pixel perfect.  The goal is to get it as close to the design as possible, while improving on CSS understanding AND speed.  So skip things or views that make sense.

Next, I would break the view down before laying down any code.

What I'm looking for in this example:
* Typography.  Should I look for any fonts that are similar to get the same vibe?
* Colors.  I'll take a screenshot and inspect colors in Illustrator and start a list of all the hexcodes used.
* Icons.  Can i use an off the shelf library like fontawesome or do I need to find something else?
* Images.  Can I google around to find images that fit the requirement?

Once I have my assets all sorted, I can move onto the next part, breaking down the layout.

Let's walk through the first view which is an elegant login page. 

On first glace it looks like we only need a single column of content (easy enough) and most elements are centered, also easy enough (somewhat).  

Knowing what I know, I think this is a prefect candidate for flexbox.  We can use it to center the logo it's logo container, and also have the form elements organized.

Another good place to practice flexbox is the subtle text "signup" and "forgot password".  Perhaps these are in a flex row using space-inbetween.

Again the goal here is to break down each design element, piece by piece and build it.  When you know a way to do it, do it.  When you don't now you get to research but at least you have something you can apply that learning to right away as opposed to learning flexbox just to learn flexbox.

In the end you'll rinse and repeat until the page is done.

Bonus:  Add interactivity.  These mock ups don't usually include any animation. But if you want, it's great practice to make some creative assumptions and style the hover states or focus states of a form input.

I've been trying to do 1 to 2 of these exercises a month just to "stay warm".  What's nice about these is. you can start/stop as needed in between projects.

Anyways, I hope this method is helpful to others.  Have fun!
