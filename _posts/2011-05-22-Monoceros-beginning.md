---
layout: post
title: Monoceros beginning - A BDD love story
category: Projects
---

{{ page.title }}
================
<p class="meta">22 May 2011 - Eugene, Oregon</p>

It's 6 am.

So here is where I start my journey. Right now, I'm sitting in my living room, listening to the menu music from a movie that's been playing for hours on end on my media center computer.

Perhaps you've been there. Furious coding, stopping to fix some errant code (Not mine. I swear) and then mashing away at your keyboard in attempt to pick up the slack and get that velocity back. All the while, the movie you started to 'watch' has been left on, desperate for your attention.

Again I say, here is where I start my journey. Working with edge [Rails](https://github.com/rails/rails), fresh from the github repository. [@dhh](http://twitter.com/dhh) has just pushed the bump for the rails 3.1 release candidate moments before I start the long-winded bundle install that will be the first step towards building a better and brighter rails future. What's the target, you ask? [Monoceros](https://github.com/Spaceghost/Monoceros). The name means [Unicorn](http://en.wikipedia.org/wiki/Monoceros) in <strike>geek</strike>^W Greek. What Monoceros does (will do), would be best explained in parts.

1. Engine

    Monoceros is first and foremost a Rails 3.1 engine. That is to say, a mountable application for your rails 3.1 applications.
    My philosophy about engines is that they should be easy to use and easy to customize. When I arrive at the point where Monoceros  works reasonably as intended, I will be including rake tasks for different types of installations of the engine should you want to modify anything.

    * Full install - Completely installing the engine inside your application. This is meant for those who want to drastically modify Monoceros in their application.

    * Partial install - I'm thinking, probably views, maybe some controllers, this will have to be explored more. I'll make a note to let you know what I come up with.

    * Install - Should there be anything that simply *must* be generated for you, this will likely be the task it will go in.

2. Authentication

    I'm going to include authentication into the engine. Why? Because I can, it takes so little time to actually code, and if I'm clever enough, I'm going to make it work with your whole application if you let me. I'm thinking it'll be held in a config file, you can specify the options for with the 'install' rake task. The goal is to have this be a fallback, and have Monoceros (That clever bastard™) check for [Devise](https://github.com/plataformatec/devise) and maybe other authentication gems and use those as a priority. Sounds nifty, right?

3. Authorization

    Now here's the big one folks. This is the word that I have dreaded in every rails application, nay, every application I have ever made. Basically, I'm going to attempt to have authorization on both model and controller levels. Some prefer one over the other, some prefer both, and God save the ones who prefer none at all. (Totally kidding, applications without permissions are cool too.)

    To start, Monceros is going to be dependent on Active Record. But don't let that fool you, my goal is to be completely database agnostic in a future release. Yes, the ability to drop this little gem into your Gemfile and use it with any rails application is possible. I hate hard work, so I might enlist some of my friends to help me with achieving that goal. But anyways, it's going to be dependent on Active Record, and pull some witty tricks through the magic of metaprogramming to grab all your tables and your controllers and (hopefully) present a nice interface for you to start working with.

    When you arrive at your monoceros dashboard, you'll be able to start defining roles. These roles consist of permissions on controllers and models. I'm going to start with controllers since that's what most people get all giddy for anyways, and they seem the easiest to implement. After you define a role, you would select which table(s) contain users. You can then select one or more users and give them one of the roles you made.

    Along these lines, I've been tossing around the idea of groups, which is kind of like a role, except it doesn't have any specific permissions applied yet. Logic will get the better of me and reveal the best approach later. Long live Agile. (Best cop out for not having any idea what the plan is to date)

