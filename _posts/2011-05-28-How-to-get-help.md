---
layout: post
title: How to get help
subtitle: Teaching people how to fish.
category: Thoughts
comments: true
meta: 29 May 2011 - Eugene, Oregon
---

Notice:
<span class="meta">This blargpost was <span class="strike">stolen</span>^W adapted from</span> <a href="http://diveintomark.org/archives/2003/05/05/why_we_wont_help_you">Why we won't help you.</a>

TL;DR Read the cucumber feature.

<div class="require"><a href="http://cukes.info" title="cukes.info">cucumber</a></div>
<div class="feature">Get help<br />
<tab /><span>In order</span> to get help from my peers<br />
<tab /><span>As a</span> developer<br />
<tab /><span>I want</span> to do <a href="https://gist.github.com/" title="Gist">all</a> I can to <a href="https://gist.github.com/996779" title="How to ask questions">help</a> them <a href="http://www.catb.org/~esr/faqs/smart-questions.html" title="Smart questions">help</a> me</div>

Now here's a scenario you might be familiar with.
You might've seen it on IRC, forums, [Stack Overflow][], mailing lists, any number of places.

Let's pretend you're on IRC and someone new asks for help and you know they're new because you're a lurker like me and don't ever sleep.
They're asking for some help with their model validations, and by golly, someone beats you to helping. Or so it seems.

The conversation goes thusly.

Helper: "Please elaborate by showing us the code by making a gist of the issue. ([https://gist.github.com/][])

The new person promptly returns with a gist.
As you start to shift gears from being super extra velocitous (New word!) to trying to help explain validations to a newcomer, you take a peek at their gist.
No, I'm going to call it the gist from hell. To call that a gist is a detriment to all gisters everywhere... on github.
It's a veritable explosion of what might have resembled properly formatted code, had it not gone three rounds with the business end of a lawn mower.

Now with you being a smart cookie and all, you back away and pretend you were never here. (It's okay, I do it too.) No one responds to the poor guy who simply needed some help.
It's like everyone forgot he existed.

Luckily, there's one cheeky fellow in the channel (usually me) who pipes up and responds with "Hey, that is honestly some of the worst code I've seen in a while, you should go and format it, clean it up and make it easier for us to help you with it."

Okay, so if this isn't all that common a story it's likely because it all happened to me. There's still a lesson to learn!

Why can't this poor fellow get some help? Well, the snarky answer would be that we've helped him a great deal already.
If you're not as zen as I am about these things, here's a more detailed explanation why his pleas for help went unheard.

<ol class="inner">
  <li><strong>Formatting your code may reveal your problem.</strong><p>Many cases of "Ohmygawsh I have no idea what's wrong!" is caused by silly developer errors.
  Typos like putting the colon in the wrong place (especially when using that darned new-fangled hash syntax) can really be embarassing at times.
  Usually simple errors like this and many others are mitigated by formatting your code according to the best practices of the community.
  In ruby this means two spaces per tab, make sure they're inserted as spaces.</p>

  <p>Now, I'm not saying that your code will work after you've formatted it appropriately; it may or may not.
  I'm also not going to say that there aren't developers out there who can't scrape the insides of a garbage disposal and come out with a perfectly valid program out of it.
  But organising your code into a format that has been deemed readable by the community surrounding the language/framework/whatever you're trying to get help with is likely the best approach.</p>

  <p>Not to put too much work on you, but if you were willing to accept a friendly suggestion, I'd say to learn how to code in that very way we just covered.
  Write your code in the format that the community can read. You'll love you for it when you need help or want to show off your code.</p></li>

<li><strong>Formatting your code may solve your problem.</strong><p>One possibility that may happen as you make sure your code is readable, you might happen on the problematic code and find that it was just a missing comma. This is a Major Win&#8482;</p></li>

<li><strong>Knowing your communication tools.</strong><p>It's not only good enough that you make your code seemingly gorgeous, you've got to share it.
  My personal favorite tool for all things pastable, at least text-wise, is <a href="https://gist.github.com/" title="Gist@Github">Gist</a>.
  Now making a good gist of your code is crucial and may impinge heavily on whether you'll get help or not.</p>

  <p>If you'd like a good tutorial on using gist that's hosted on gist and likely written on it as well, <a href="https://github.com/radar/guides/blob/master/using-gist.md" title="Using Gist">this</a> is a great example.</p>

  <p>Knowing how to ask for help is also a very important skill. One that really is easier to learn by doing than reading. One thing you want to be aware of is both spotting and not being a 'help vampire'. Here's a <a href="http://slash7.com/2006/12/22/vampires/" title="Help Vampires: A spotter's guide">link</a>.</p></li>
</ol>

Now, please go forth and imbue the world with many such niceties as lovely gems, LOC's by the dozen (Hehe, joke about ruby not taking copious amounts lines to do trivial things), and instill a mindset of a curteous coder.

~Johnneylee

[https://gist.github.com/]: https://gist.github.com/ "Gist@Github"
[Stack Overflow]: http://stackoverflow.com/

