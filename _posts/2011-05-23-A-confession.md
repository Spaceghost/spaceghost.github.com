---
layout: post
title: A confession
subtitle: Don't hate me.
category: Monoceros
comments: true
---

{{ page.title }} - {{ page.subtitle }}
================
<p class="meta">23 May 2011 - Eugene, Oregon</p>

[Yesterday][] was a productive day. I feel so good about it, I even broke down a wall that I've had for a long time. For the first time in Spaceghost history, I open sourced a project before it was even fit for human consumption.

Why would this matter in the least? To quote an old adage, "Commit early, commit often" I'm usually pretty good at keeping to my deadlines, but when I start a project that belongs solely to me, I tend to let it flounder after a while.

Now that I've given a small backstory to the confession, I'll spill the beans. I started [Monoceros][] a couple weeks ago. Oh those were the days. I was hacking along, making great progress and really just exploding out onto the repository with code. What deterred me from this path was an unwelcome guest. Or rather, quite a few. Since I tossed testing to the wayside in order to fully express myself, I introduced a large gaping hole into my project. Things were breaking left and right. You might say, "That's not a problem, just track down your bugs." and I agree with you, you should track down bugs. But when those bugs exist purely because you failed to keep code that you've already written working, that becomes an issue for me.

I still have the code I wrote in haste. It has a working dashboard panel and automagically detects the models in your application. Although I couldn't quite get it to work with models in engines. I learned a lot from the time I spent employing as many metaprogramming spells as I could wield, and properly namespacing my engine by hand. I was so silly, I even wrote it inside a plain rails application! Not a shiny new rails 3.1 engine. How ignorant I was!

Long story short (tl;dr), that code won't ever be open sourced and I will never release something meant to help the Ruby on Rails community without <a name="tests"> </a>tests to ensure that it works. This is just as much a promise to you as it is a promise to me. If you find that I'm lacking, please let me know. I'll also not accept code without tests. If you would like help testing your code, you should either be BDD'ing it along with me and whomever is playing with Monoceros, or you should make friends and get some help with your tests.

Thank you for being my silent partner in crime,

~Johnneylee

[Yesterday]: /Monoceros/2011/05/22/Monoceros-beginning.html "Monoceros-beginning"
[Monoceros]: https://github.com/Spaceghost/Monoceros "Monoceros@Github"

