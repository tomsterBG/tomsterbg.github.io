---
layout: post
title: "Programming, ai and making of this blog"
date: 2025-05-06
last_edit: 2025-05-06
critics: 0
sitemap: false
hidden: true
---

I have been making this website for the past few days and i have to admit, Gemini 2.5 has been VERY helpful!

Usually i am not an early adopter, i don't jump on beta versions nor look for the newest trends. I never pay online (did it once and it was a waste of money, never again) and i always look for free, stable software even if that means *looking for alternatives* 🏴‍☠️. Actually, ever since ditching Windows i haven't downloaded anything shady, well except GitHub Desktop (it's shady because GitHub is owned by Microsoft).

Also i've been on the skeptical side of the ai revolution. Not because i don't believe what is going on, i do see and use it, ai is great and useful! The skepticism is about how people wrongly interpret it, saying overly optimistic stuff because they heard the overpromised lies told by the giants who run these companies. Ai needs insane learning data and runtime, something only the giants can afford. Not to mention there are [stories](https://world.edu/long-hours-and-low-wages-the-human-labour-powering-ais-development/) of many people being used as very low wage workers to label data, that's... really dark. And i couldn't even find the one i remember so i linked to a different one.

{:.callout .callout-tip}
Pro tip: you can `middle-click` the scroll on your mouse for various things. I use it for opening links in a new tab.

Anyway, right now i'm not here to break down the darkness of ai. Starting `3 May 2025` i decided to learn how to make a website to host for free, prompted Gemini and i was unable to use the first output because it had requirements to use eleventy to generate the site. However when i told it to generate everything in a single `.html` file, it did so well that i wondered "What would the first output look like if i wasn't so inexperienced and could actually make it work?" Then i asked it to do a very simple version of what i wanted without any static site generators to build it. That worked too and it looked amazing for an ai output! Gemini 2.5 is so cracked, i'm absolutely sure ChatGPT was NEVER this good when i used it, even though i used it months ago for programming and it could somewhat help at first, then they refined it to do better, but still it made so many mistakes. The biggest thing about Gemini is its context comprehension. It can understand entire zip archives, enough for me to post my entire website and just ask directly how to do something. So i iterated on what it generated a bunch of times and liked it, but you know the drill. When an entire website is built by an ai, there's no way it's as good as a real website built by someone competent. And i was right.

I remembered that i had seen [this website](https://brainfucksec.github.io/) earlier to harden my Firefox and when i saw the `github.io` url i thought "You can do that?" It wasn't until `4 May 2025` that i decided to actually look at this website's [GitHub repo](https://github.com/brainfucksec/brainfucksec.github.io) and that turned out to be the best decision ever! Thank you gigachad, your work will be remembered and loved!

So i started messing with my own copy of his website and asking Gemini to make edits and explain some things. I now remember one of the most important programming lessons i had forgotten - the best way to learn coding past the basics is to read other people's code and try to understand and modify it. This is a very, *very* fast way to learn (once it clicks, it's usually really slow before it clicks, but when it does click it all comes together and is now worth it) especially when combined with years of past experience (that are currently grayed out because i'm rusty, haven't been coding for a while) and with an ai that can, *FINALLY*, code like a half-competent person.

Gemini is still not at the point of replacing programmers, but it's definitely at the point where a client could come in, ask for some software and you'd prompt the ai to quickly whip up drafts that you could show to your customer for an easier time later. We all know that type of person who thinks they know what they want, but when they actually see what you do, they say "no, i wanted it more like this". That problem will still exist, but you can really alleviate it now with quick ai generated drafts.

## Basic website structure
The website uses the simplest things possible: `.html`, `.scss`, `LiquidJS` (to be parsed in `.markdown`), `markdown` and i love this. Markdown is my favorite especially after using [Obsidian](https://obsidian.md/) for about a year now. I love how you can write `HTML` and `LiquidJS` inside the same `markdown` file, as you can see in [posts.md](https://github.com/tomsterBG/tomsterbg.github.io/blob/master/posts.md). Also that i can just overwrite `.scss` as much as i want, letting me ask Gemini to generate entire files that do complex stuff like [beige.scss](https://github.com/tomsterBG/tomsterbg.github.io/blob/master/_sass/base.scss) and [_callouts.scss](https://github.com/tomsterBG/tomsterbg.github.io/blob/master/_sass/_callouts.scss). They're basically overlapping some of the original [base.scss](https://github.com/tomsterBG/tomsterbg.github.io/blob/master/_sass/base.scss), but because [main.scss](https://github.com/tomsterBG/tomsterbg.github.io/blob/master/css/main.scss) imports them later, they make sure that if there are conflicts, the later imported files have the last word. I could also use this to quickly jump between themes for the site.

One main complaint: i am using the default Linux Mint text editor with dark mode which makes most colored text a nightmare to read. I really don't want to use VSCode again, i found it really hard to understand what's going on and it feels sluggish.
