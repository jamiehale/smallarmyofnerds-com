---
layout: page
title: Tablescript
permalink: /software/tablescript/
---
Tablescript started as a hobby project to build a scripting language that could be used to quickly define and select from tables of random outcomes, as frequently used in roleplaying games.

The initial implementation was a complex C++ parser and interpreter. It worked fine until I broke it trying to add classes to the language. That was many years ago, before I learned how to use revision control properly. I have not gone back to fix it, but intend to.

In the intervening years, my need for the tool did not diminish.

Then I found the wonderful [Ruby programming language][1]. And with it, easy-to-define DSLs. I reimplemented most of the original functionality in a day using less than 250 lines of Ruby.

The tool is functional for now. It's packaged in an easy-to-install gem that can be downloaded [here][2].

It is Free Software. The source code is [here][3].

## Use

{% highlight ruby %}
#! /usr/bin/env ruby

require 'tablescript'

table :gems do
  f { "ruby" }
  f { "quartz" }
  f { "garnet" }
end

count = roll_dice( '3d6' )
gem = roll_on( :gems )
value = choose( [ 10, 100 ] ) * roll_dice( '2d6' )

puts "#{count} #{gem} gems (#{value} gp)"
{% endhighlight %}

[1]: http://ruby-lang.org
[2]: https://rubygems.org/gems/tablescript
[3]: https://github.com/jamiehale/tablescript.rb