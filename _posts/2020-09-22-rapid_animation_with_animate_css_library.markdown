---
layout: post
title:      "Rapid animation with Animate.css Library"
date:       2020-09-22 15:07:01 -0400
permalink:  rapid_animation_with_animate_css_library
---

Modern front end UIs (at least the good ones) always feel SMOOTH to me.  Nothing is jarring.  Elements transition nicely in and out, on and off screen.  It’s an important piece of the puzzle that most take for granted.  BUT if you take those simple animations and transitions away, not only is it apparently there, it can completely pull you out of the experience.

Developing with raw HTML/CSS/JS leaves something to be desired when it comes to animation and transitions.  While the functions, features and layouts all might be there.  Nothing is worse when you have a hover feature or a button click and the change happens instantaneously or abruptly.

That said, there’s already so much to focus on with respect to our projects, especially when you get to the JS project (Frontend JS and backend Rails!! EEK!).  Who has time for animations!?  Exactly where an amazing framework like Animate.css comes in.

[Animate.css website
](https://animate.style/)

Animate.css is a CSS framework that’s easy as pie to bake into almost any front end projects.  Follow the simple instructions on their website to include the library.  But the gist is you can either install it with NPM, Yarn, or just include it in the head of your HTML page.

## How to use
Usage is a simple two step process

### Step One
Give your HTML element a class name of `"animate__animated"`.  This class primes the HTML element. Read the actual documentation to see what specific CSS this adds to your element.  But it does NOT do any animations, yet.

```
<div class="animate__animated" id="card">
   <p>Text inside a card</p>
</div>
```

### Step Two

Select one of the many built in animations and add its name to the class list of the HTML element.  Animate.css comes with a ton of built in ready to go animations that can be found on the right side bar.  Browse through the effects, pick one and simply add it to the same HTML element.  Let’s say we wanted our `<div>` to bounce in on load...

```
<div class="animate__animated animate__bounceIn" id="card">
   <p>Text inside a card</p>
</div>
```

Give it a refresh and bam, you have world class animation without any of the hassle.

## Summary

Recap of Why you should add in animations:
* Less jarring experience for the user
* Its what should be expected from a world class UI
* It makes our projects feel alive and real
* Its that extra attention to detail that will hopefully impress potential job interviewers

For my JS-Rails project I used a lot of the Animate.css library to give the UI components some character.
[Check out my video walk through here to see it in action.](https://youtu.be/CDvMKIVG1y0)

