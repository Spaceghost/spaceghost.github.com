---
layout: post
title: Feature share
subtitle: Where you learn that there are way too many ideas in my head.
category: Monoceros
comments: true
---

<p class="meta">24 May 2011 - Eugene, Oregon</p>
> "We would rather have you contribute and mess something up than not contribute. So please go ahead and mess around." &dash; [Sarah Mei][]
---
Alright, here's the latest. I'm going to start tossing out ideas for you to discuss, critique, scoff at and generally offer feedback on. I'm not looking for the "best way", but I do love input. If you can fix anything or make some cool changes beyond the helpful hint, please submit a pull request. Take note though, in my [second post][] I mentioned that all pull requests have to include tests for code changes. Without further ado, my ideas.

#1. Idea number the first: Branching

I'm creating a few branches in [Monoceros][]. The first being "Web" where I'll start with some cucumber view specs. This branch will deal directly with the web interface. I'm feeling out just how much cucumber I can handle with these view specs, I don't want them to be too brittle, because if someone wants to step in and fiddle around to customise Monoceros for their application using the rake tasks I mentioned in my [first post][] they'll have a lot of failing features.

I'm going to continue with this, creating branches for each part of Monoceros, such as "DSL" for the role defining DSL when I get there. Another for the dsl for views and so on.

#2. Idea number the next one: Encouraging BDD & CT practices

My good friend [workmad3][] pointed out that my [Gemfile][] is silly, among other things. His reasoning is that I shouldn't include [Watchr][] and [ZenTest][] inside my Gemfile. Those really do belong in a gemset, but it should be the choice of the developer if they do or do not want to use them. While this all made perfect sense, I was clever enough to state that I was including them to help build a community environment that embraced BDD and CT in their development (Read: Play) with Monoceros.

Assuming the idea isn't hated by too many, I'll get the Gemfile in order and allow people to use --without when they bundle if they don't want it. It's like [Rubygems][] not using a sensible default. **cough**[notgeneratingdocumentationbydefault][]**cough** I also may be coming down with a cold.

**~/.gemrc**

        --no-ri
        --no-rdoc

So, that's that. I'm using cucumber and rspec right now. A great book to learn BDD and how to use these tools is the [RSpec book][] by [David Chelimsky][]. You can look at the Gemfile for the rest of the tools I use.

I'm also going to be using [aruba][] to test the monoceros executable for the generators and any other CLI goodness.

#3 Concept the III: Those rails generate tasks

[Earlier][], when I talked about Rake tasks, I mentioned three types of tasks. These are the generation commands for the engine itself. The `rails g monoceros:install:full` task will fully install Monoceros into your application. Now it is easy to modify and customise.

The `rails g monoceros:install:partial` task is probably going to generate controllers and views for monoceros. Just in case all they want to change is the views and how they want to present data in the controller and the such. I'm thinking of having the files generate to their respective directories, and putting any images or assets that Monoceros uses in the proper directory.

`rails g monoceros:install:minimal` will only generate the bare minimum of config files and whatever else it needs into your application. I'm expecting to include the usual opts for forcing it, not over-writing, etc.

#4 Manifestation number four: Building usable and cogent DSL's for Monoceros

There will be two [DSL][]'s in Monoceros. The first is the Roles DSL. The goal with this DSL is to be as expressive as possible, but easy to use with the web panel. Since I'm going to be using it for storing Roles and the such, I need to make the web panel work with it, loading and saving to the config in that DSL. This I might need a bit of help on.

The second DSL is the for the view. I'd love to work with developers who know what they'd like to see in this DSL. My goal is to build a DSL that's fun to use and easy to manage. I already got some feedback from a few good friends working on the [Rubunity][] web application and community. Here's what one of the guys there suggested for passing blocks with roles (In Haml). <script src="https://gist.github.com/958822.js?file=show.html.haml"> </script>


Won't you be my neighbor? Comment, discuss and let me know what your thoughts are, or questions. If the question is one I think would deserve a blogpost, I'll write one on your question.

[Sarah Mei]: http://twitter.com/SarahMei "@SarahMei"
[Monoceros]: https://github.com/Spaceghost/Monoceros "Monoceros@Github"
[first post]: /Monoceros/2011/05/22/Monoceros-beginning.html#rake "Monoceros beginning - Rake tasks"
[second post]: /Monoceros/2011/05/23/A-confession.html#tests "A confession - Tests"
[workmad3]: https://github.com/workmad3 "Workmad3"
[Gemfile]: https://github.com/Spaceghost/Monoceros/blob/72f72f3eb8743685921c67c0cc17383c38029b74/Gemfile "Gemfile@Github"
[Watchr]: https://github.com/mynyml/watchr "Watchr@Github"
[ZenTest]: https://github.com/seattlerb/zentest "ZenTest@Github"
[Rubygems]: http://rubygems.org/
[notgeneratingdocumentationbydefault]: https://github.com/rubygems/rubygems/pull/42 "Pull request number 42"
[Rspec book]: http://pragprog.com/titles/achbd/the-rspec-book "The RSpec Book @ Pragprog"
[David Chelimsky]: https://github.com/dchelimsky "dchelimsky@Github"
[aruba]: https://github.com/cucumber/aruba "Aruba@Github"
[Earlier]: /Monoceros/2011/05/22/Monoceros-beginning.html#rake "Monoceros beginning - Rake tasks"
[Rubunity]: http://rubunity.com/ "Rubunity"
[DSL]: http://en.wikipedia.org/wiki/Domain-specific_language "DSL@Wikipedia

