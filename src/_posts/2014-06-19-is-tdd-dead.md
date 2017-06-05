---
layout: post
title: "Is TDD dead?"
date: 2014-06-19 11:14:00 -0500
categories: uncategorized
---
Spoiler alert: Hell no.

If you haven't noticed, there's been a pretty major nerd-spat playing out in certain corners of the internet. On the one side, Rails creator David Heinemeier Hansson believes that TDD is a waste of time and energy, and encourages poorly designed software. On the other side, many people of consequence disagree. Some respectfully (Kent Beck and Martin Fowler). Others not so much (Rob C. Martin).

Find DHH's incindiary post [here][1]. Note his use of clever rhetoric like, "This is not better." Also note that most of his arguments rest on his point that module isolation is a Bad Thing - a point that runs contrary to most modern software development (and a fair bit of not-so-modern stuff too). See also: Object Oriented Analysis and Design, Object Oriented Programming, SOLID principles, and pretty much everything else that isn't high-school grade code.

Find a 5-part debate between DHH, Kent Beck, and Martin Fowler [here][2]. Enjoy 3 hours of Beck and Fowler politely patting DHH's head as he repeats over and over what I summarize as: "TDD is bad because I don't like it!" and "TDD is bad because it produces code that I think is bad!"

Rob C. Martin weighs in [several][3] [times][4], but my favorite is [here][5]. His conclusion uses the word "professional". That particular word struck a chord with enough folks that he had to [clarify and almost retract] what he had said. Too bad.

Fun!

For the record, when possible, Small Army Of Nerds Corp. practices _professional_ TDD. And though I find the word a little goofy, I fall squarely in the "mockist" camp. Unit tests test units - little to nothing else.

[1]: http://david.heinemeierhansson.com/2014/test-induced-design-damage.html
[2]: http://martinfowler.com/articles/is-tdd-dead/
[3]: http://blog.cleancoder.com/uncle-bob/2014/04/25/MonogamousTDD.html
[4]: http://blog.cleancoder.com/uncle-bob/2014/04/30/When-tdd-does-not-work.html
[5]: http://blog.cleancoder.com/uncle-bob/2014/05/01/Design-Damage.html
[6]: http://blog.cleancoder.com/uncle-bob/2014/05/02/ProfessionalismAndTDD.html