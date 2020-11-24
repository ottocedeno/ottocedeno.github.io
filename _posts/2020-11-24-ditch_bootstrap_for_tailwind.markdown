---
layout: post
title:      "Ditch Bootstrap for Tailwind"
date:       2020-11-24 15:59:02 -0500
permalink:  ditch_bootstrap_for_tailwind
---

## Start with Bootstrap

When I first started learning to code, I was all about [BootStrap](https://getbootstrap.com/).  Why wouldn't you be?  It was a fast shortcut to getting projects to look a bit more 'designed' without having to write any CSS.  Browsing through the many components they offer off-the-shelf, you can build almost anything and it will have that modern touch.  Personally, I think solid design and UX goes hand in hand with solid code.  Imagine putting in a ton of hours on a complex API and front end application, only for it to look, well ugly and uninviting to the user... no bueno.

Once you get started with BootStrap you'll see it's super easy to follow thier design pattern and add components to your site as needed without writting any CSS.  See their [documentation here.](https://getbootstrap.com/docs/4.0/getting-started/introduction/)

If you don't have a design system in place and just need a quick solution to create a somewhat polished protoype, then BootStrap is a great solution.  But what if you want something more custom / need to follow a given design system?  Sure you can still use BootStrap and also add your own CSS styles, but now your project is a bit messy.  Some CSS lives in your stylesheets, and others are just inherited from the BootStrap CSS files.  There's got be a better way to build a fast protoype with more wiggle room on customization.

Enter Tailwind.

## Intro to Tailwind

At first when I was introduced to [tailwind css](https://tailwindcss.com/) by a colleague, I was very MEH.  But at that point in my devepment roadmap, I wasn't in need of customizing design systems. (aka Bootstrap was the smarter tool).  When you first look at Tailwind and see that it's a Utility First design system, it's a bit overwhelming.  Also it feels a lot like writting inline styles for HTML elements but with class names.  Which turns a lot of people away.  But before we get into the pros and cons, let's go through the basics.

### Using Tailwind

After going through the tailwind installation, which you can find [here in their docs](https://tailwindcss.com/docs/installation), getting started is insanely easy.  Simply add class names of component features you want to give to that HTML element.

For example, let's say we wanted to create a style for our H1 Page titles, we can center the text, make it large and give it a color with the following Tailwind utility classes:

```
<h1 class="text-center font-bold text-lg color-red-600">Welcome to my cool App</h1>
```

This would result in an h1 styled similarly like this in a custom CSS stylesheet:

```
h1 {
   text-align: center;
	 color: #FF0000;
	 font-weight: bold;
	 font-size: 2rem;
```

At first it seems six to one half dozen to the other, but the power of Tailwind comes in the details.  Since it's a CSS system built with utilities first, you can build an almost ENDLESS amount of custom components with high reusability, especially if you're using React, without writting a single line of custom CSS.

Once you get into the realm of needing custom design, Tailwind will increase your work speed tremendously as you'll have most of the key classes memorized, and you'll have ZERO context switching going from your React JS files to a stylesheet file.

To learn more about Tailwind and its benefits, I highly recommend reading their docs and watching their support videos.  Once you get a taste for it, you'll never build a front end without it!

