---
layout: post
title: Coding dangerously
subtitle: Or why I would rather not use debuggers.
category: Thoughts
comments: true
meta: 28 May 2011 - Eugene, Oregon
---

I spend a lot of time in the #RubyonRails channel on Freenode.
Sometimes a certain subject comes up that I have problems refraining from answering, or attempting to.
That question goes invariably like, "... debugger ..."

I ommited the parts that aren't important right now, my mind is already making a sad face.
I start to wonder if it's conviction or something sinister that gives me such a distaste for debuggers.
The way I feel about debuggers is that you should be comfortable enough with the language to be able to write quick throw-away code to investigate the problem if you're able to use the debugger with any skill whatsoever.

Perhaps that's an unrealistic goal, but I digress. "Coding dangerously", besides sounding like the newest hip craze you hooligans are into,
is a practice of realizing it's perfectly fine to write code you intend to throw away once you've found the information you needed.

Why would I want to write code I intend on tossing out? Well, that's a good question.
It may boil down to personal taste, but right now I'm on the soapbox.
I find that I'm able to keep my present <a name="velocity" title="Velocity is an extremely simple, powerful method for accurately measuring the rate at which teams consistently deliver business value.">velocity</a>
when I take a moment to root around the program and get the data I need instead of dropping into ruby's debugger.

My preferred methods of getting to the juicy bits of my program will likely always be [#inspect][], [#instance_variables], and [#logger][] from the stdlib as well as [#debug][] in [Ruby on Rails][].
Examples of their uses can be found on the rails guide for [debugging][]. I'll check back in later for some more advanced techniques for coding dangerously.

This is where we part ways for a while, I hope you enjoyed my mind as much as I do. Live long and code dangerously.

[Make it sew][],

~Johnneylee

[#inspect]: http://www.ruby-doc.org/core/classes/Object.html#M001025 "#inspect@Rubydoc.info"
[#instance_variables]: http://rubydoc.info/stdlib/core/1.9.2/Object#instance_variables-instance_method "#instance_variables@Rubydoc.info"
[#debug]: http://rubydoc.info/docs/rails/3.0.0/ActionView/Helpers/DebugHelper#debug-instance_method "#debug@RubyonRails"
[#logger]: http://rubydoc.info/stdlib/logger/1.9.2/Logger/Application#logger-instance_method "#logger@Rubydoc.info"
[debugging]: http://guides.rubyonrails.org/debugging_rails_applications.html "Debugging Rails Applications@RubyonRails"
[Ruby on Rails]: http://rubyonrails.org/ "Ruby on Rails"
[Make it sew]: http://i.imgur.com/IBXFX.jpg "Make it sew"

