---
layout: post
title:      "Adding Colorize to your Gem will make it POP"
date:       2020-01-24 00:01:52 -0500
permalink:  adding_colorize_to_your_gem_will_make_it_pop
---


I'm a visual person.  And if you are too, you might find making terminal based apps a bit on the simple side when it comes to color and creativity.

Enter: Colorize

Colorize is a Ruby Gem that extends methods to String objects that are output to the terminal.

For my CLI Gem project, it was a game changer.  I built an app called SnowReport that show's users data about the best ski resorts in the world.

To install this Gem, to an existing Ruby Gem project, you can add it as a dependency in your gemfile (if you setup your project via Bundler).

Type in ```ruby spec.add_dependency "colorize"``` with in the block scope of ```ruby Gem::Specification.new```

To use Colorize in your code, you must require it at the top of each page.  Type ```ruby require 'colorize'

Visit: https://github.com/fazibear/colorize to see the documentation on how to use methods within Colorize.

Now that it's up and running, let me show you how I used it to add some POP to my project...

Initially, I was struggling to find a meaningful way to make my information that the user was reading stand out in the monochrome world of terminal.  So I did some Googling, and found Colorize.  My initial application of it was to solve for 2 problems:

1. I wanted my section headers to stand out so the user knew clearly where they were in the application.
2. I wanted my data values to POP from it's data label.

Here are two places in my code that I was able to successfully leverage Colorize:

Example 1:  Printing the top level list of mountains.

```ruby
  def self.print_top_mountains
      puts "\nHere are the top #{self.all.size} mountains by 5 day snowfall".upcase.colorize(:blue).bold
      self.all.each.with_index(1) do |mountain, index|
        puts "#{index}. #{mountain.name} - #{mountain.five_day_snowfall.colorize(:red)}"
      end
      puts ""
    end
```

This resulted in a very user friendly print out of:

![Ex1 image](https://raw.githubusercontent.com/ottocedeno/snowreport/master/Screen%20Shot%202020-01-23%20at%2011.36.11%20PM.png)

Example 2:  Printing an individual mountain's data.

```ruby
  def print_mountain_info
      puts "\n#{self.name}".upcase.colorize(:blue).bold
      puts "Located in #{self.region}".upcase if self.region
      puts "5 Day Snowfall: " + "#{self.five_day_snowfall}".colorize(:red) if self.five_day_snowfall
      puts "Tomorrow's Snow Fall: " + "#{self.tomorrows_snowfall}".colorize(:red) if self.tomorrows_snowfall
      puts "Conditions: " + "#{self.conditions}".colorize(:red) if self.conditions
      puts "Base Depth: " + "#{self.base_depth}".colorize(:red) if self.base_depth
      puts "Trails Open: " + "#{self.trails_open}".colorize(:red) if self.trails_open
      puts "Lifts Open: " + "#{self.lifts_open}\n".colorize(:red) if self.lifts_open
    end
```

This resulted in another user friendly print out:

![Ex2 image](https://raw.githubusercontent.com/ottocedeno/snowreport/master/Screen%20Shot%202020-01-23%20at%2011.36.30%20PM.png)

As you can see in both examples, I can simply call ```.colorize``` on a string and pass in an argument.  In my application, I kept it simple and used the symbols ```:red``` and ```:blue``` to make my data values and headers pop.

Again, if you are more of a front-end visual person, Colorize helps your application stand out.  I hope this simple tutorial helps!



