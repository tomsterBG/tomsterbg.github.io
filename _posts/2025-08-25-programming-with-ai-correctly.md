---
layout: post
title: "Programming with AI correctly."
date: 2025-08-25
last_edit: 2025-08-25
critics: 0
sitemap: false
hidden: true
---

This is a polarizing topic for some people. I hear "AI is great, it can do this and that". I hear "AI is terrible and it can't do anything, you should NOT use it for code".

Both are wrong, it's more nuanced than that.

The rules on how to use AI "correctly" exist because there are problems if you use it "incorrectly". Hence the labels, correct and incorrect.

Everyone comes up with their own rules and i can't give you the perfect set to follow, but i'm going to show my problems, problems i've seen and then solutions to these problems.
I'm also going to show benefits and strengths of correct AI usage.

# The problems

## Not actually learning

[Vibe coding](https://en.wikipedia.org/wiki/Vibe_coding) is the most well known wrong way to use AI so far. All you do is write normal sentences that ask for code, the AI gives you the code and you use that in your software without editing or looking into the logic behind it.

Do you know how the code works? Of course not, you didn't write it, you didn't review it!

When there's a bug you say *"I don't care"* and click the "fix bug" button.

This is fine when you aren't a programmer and just want something specific to work, but it's not fine otherwise. Even if you are a hobbyist, you are going to waste less time if you understand the code in the first place.
Trust me, programming is one of those things that isn't for everyone, but if you can think logically, once you get it, it clicks and now you can do it again, **much faster**.

Also, [Leetcode](https://leetcode.com/) exists for a reason. People knew that they need to practice and figure out solutions. Imagine being so down bad that you solve Leetcode problems with AI alone. They are **designed** for you to solve, if you want to learn the skills that each problem teaches. If you don't want to learn, keep on vibe coding.

## Overreliance

Some people like myself would actually review the code and try to understand how it works. However, sometimes without realizing, i would ask the AI things i could do myself. This is a problem.

With the years i have come to the conclusion that you take care of the brain in a similar way to how you take care of your muscles, by training. No training and both the muscles and the brain suffer atrophy.

Now imagine, instead of going outside and lifting a weight, i tell someone else to do it. Or, instead of solving a problem, i tell someone else to do it.

If that didn't make it obvious, the problem-solving skills are greatly diminished when someone relies too much on AI.

## Insufficient or flooded search results

Often times i would search for something and it would either not appear, or it would be buried in a wall of text that isn't straight to the point.

Other times it would be written in such confusing way, that you have to be the programmer who developed it, to understand. Or you need years of experience with the specific software. That isn't quite possible when new software comes out many times a day, and good, mature software grows in numbers, size and complexity.

This is when i sometimes decide to just use the AI instead of a search engine. Sometimes i would even copy a large document or page i found and ask it to explain, elaborate or summarize what this means, as well as find what i need.

## If you don't know the possibilities, you don't know what you can make

The best ideas i've had came from "aimlessly" experimenting with the features of a software. For example i wouldn't have made physical contraptions if i didn't know you can constrain them to behave in interesting and perhaps realistic ways.

More specific examples are kardan shafts (aka universal joints), engine pistons, cranks, gears, rope bridges, trains and more.

The best quote about possibilites i've heard is "if you can't make it perfect, make it adjustable". And you can't make it adjustable if you don't understand the parameters in the first place.

## Creativity

Even if AI might seem creative, i'm not the first person to say that it isn't. The reason it appears creative is because it has access to so much data, way more than we can ever hope to remember. Some human already did the creative solution that the AI is proposing, and if nobody did, the AI combined solutions from multiple places.

Combining solutions may be construed as creativity and in some cases it is, so i don't think this is what matters the most here. What truly matters is, again, your skill. Your experience, your creativity, your ability to come up with new things, to combine pieces of knowledge into something new.

Sometimes it may be useful to use AI as a search engine specifically in a way that gives you all the building blocks and lets you combine them, instead of asking it to do that for you. For example i remember asking it something among the lines of, how do other game engines do a specific thing, instead of "solve this problem, inspired by solutions in other game engines".

## Confidence

This one is more personalized. I am a perfectionist and i have always had to tell myself that things don't have to be perfect. However, code breaks and is very picky! Sometimes it's broken without even telling you. This is why over the years i developed a habit of proofreading my code multiple times over, which slows me down a lot.

There are two solutions to this. Testing your code with automated tests, and sending it to the AI by asking:

{:.callout .callout-note}
Criticize my code.
Are there any bugs, inconsistencies, unwanted behavior, typos, outdated comments, useless comments? How can i improve the code?
Is it all good? Do i even need to change anything? Am i following good coding practices?
Be concise and to the point.

I do both of these things as of writing this sentence, in the following Github project: <https://github.com/tomsterBG/godot-classes-unit-tested>

More often than not, it wouldn't give you a very good answer if your code is already good enough, but it's very good at catching things that need to be caught. So if your code has a flaw that's obvious and you missed it, the AI will probably find it.

# The rules

Now that i've given some reasoning, i think you won't just understand the **what** of a rule, but also the **why**.

## Never say that AI is bad

This is just not true. It can do some things, it can't do other things. Each model is different and nothing is this black and white.

## Never say that AI must be used for everything

Again, AI is not an "all in one" kind of tool, and nothing will ever be.

## Don't use AI if you can do the thing, except when you have to do it 490 times over

Training your skills is important, but what isn't important is repeating the same taks over, and over, and over, and...
Also don't count to 1000, that'd be stupid.

For such repetitive tasks, sometimes the solution would be AI, sometimes making a macro algorithm to edit everything in bulk.

## Don't use AI to finish your work

Ever since i started using it, i have been saying this, and for a good reason. The AI comes up with hallucinations.

You should always be the last one who judges what must be done. The human must be the one who reviews official changes.

## Don't let AI edit your project in an integrated environment

This rule goes very well together with the previous one.

This is vibe coding's worst pattern. Using the AI directly in your project for convenience, instead of letting it write on its own, and then learning from what it wrote, and writing it yourself. This is a big red flag that simply says "i am overreliant on this".

Instead do what i do, use AI in the browser.

Most AIs let you copy the code block they produced, so it's not a big hassle. Also if it's a big hassle, it would be much better for your future if you prompt it to make an algorithm that automates a repetitive task, as stated above, rather than prompting it to **do** the repetitive task.

## Don't pay for AI

There are so many free, to my surprise, models. Most of them are by big companies too. Paying for it, at least for me, doesn't give me nearly as much benefits as i would think it should. My own usage of AI is very contradictory with the pattern that if you pay for it, it should become more convenient and full of tools.

As i've said before, overreliance is dangerous, and one big red flag is too much convenience. It allows you to do destructive things such as accepting code changes without knowing what actually changed.

Another point is that, when you pay for it, you expect to gain something. Suddenly you're financially bound and if something happens, if a new model by another company comes out, now you're mentally stuck with the current model simply because you don't want to waste the money you paid. And using a different model than the one you paid for can be considered a waste of money.
Whatever else happens, the company fails, they become more greedy, raise prices, whatever. Not paying for it frees you up mentally from thinking that you got scammed or wasted money. And to be honest, i do think it's a waste of money when there are free alternatives.

The only exception i'd make is to pay for something free if i know that the person who made it is a good one, and usually large companies aren't.

On a side note, i would love to support the Factorio and BeamNG devs buy buying a copy of their games, simply because they've shown over the years that they deserve it. Good morals, consistent development, in fact, Factorio's blog posts are such an important piece of knowledge for any other developer. They write about search algorithms, sprite stacking techniques, music generation, noise generation, performance optimizations at big scales, the benefits of automated tests in your code, and best of all, read for yourself: <https://www.factorio.com/blog/post/fff-366>

# The strengths of AI

## Being a smarter search engine

Not always, but sometimes it can find stuff you never thought existed.

And best of all, it doesn't just search the web, it can search code too.

Often when you download code, there are so many unknowns, especially if it's a few megabytes big. A few megabytes of code is thousands upon thousands of lines. No way i'd know what all of that does!
Here comes the AI to help. I copy the code and ask, if i wanted to do this and that, where to go, which files to modify, what does what, etc.

You can think about this from a different perspective too. AI is basically an excellent way to "generate code comments" that elaborate what the code does.

## Explaining singular things

Each language has nuances, why does this use `::`, why is there a `#`, what is `#ifdef`, what is this function and many, many more questions.

Depending on how popular or open your codebase is, the AI will be able to explain the things you don't yet understand. You can apply human intelligence from there to use the newly acquired knowledge, or better, to experiment with it in an **informed** way.

Sometimes i absolutely hate the feel of being clueless in a new environment because even if i wanted to test stuff, everything suddenly breaks. Instead of searching for the exact tutorial on what i want to learn, AI can just explain it.

However, when the documentation is excellent and the tutorial is brilliant, AI is actually a downside. This is because humans can give you specific insight into why this works, when it doesn't work as good as something else, what are some less commonly known usecases, what are some cool examples, etc. You can still ask the AI to give you links to sources in order to deepen your understanding.

## Code review

As stated before in the confidence problem, i sometimes use AI to tell me whether something is off with my project, before i upload it to Github.

This may sound contradictory with me saying not to use AI to finish your work, but it isn't, because i am still the last judge. I decide what needs to happen and i always use AI in the browser, not in my coding environment.

Just today i was about to push to Github and decided to zip my code, ask the AI what may be wrong with it and guess what, it found a bug! I had an event being fired *after* clamping a value, causing the event to have an incorrect number as an argument, a number that could go outside of the clamping limits. I would have had to proofread my code for the 50th time by now to notice that.
