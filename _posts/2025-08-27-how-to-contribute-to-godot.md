---
layout: post
title: "How to contribute to Godot."
date: 2025-08-27
last_edit: 2025-08-27
critics: 0
sitemap: false
hidden: true
---

[George Marques](https://www.youtube.com/watch?v=xFaTV4xRwaU) already talked about this, some other videos did as well. However i want this to be a more personalized cheat sheet for what to do when i want to help. And maybe, you can find it useful too!

Here are some other videos already covering the topic:
- <https://www.youtube.com/watch?v=HEOt79up5LE>
- <https://www.youtube.com/watch?v=LeUDvHS9vtQ>

And a playlist by Mohsen Zare on GDExtension: <https://www.youtube.com/playlist?list=PLhixpuPeRv9aDdsZbhTpsXguYRvMgyVQ->

Mohsen's channel is, by far, one of the better ones when it comes to actually showing you how to do it. Not because of the quality, but because he actually does it and explains things while showing them. I personally believe that video tutorials are way better if the person just gives up on explaining things they can't explain, and show them instead. Showing can be worth 1000 words.

Let's list each way in which you can contribute, from simplest to more complex:

- Use the engine and say or show that you used it.
- Gain experience, join the [Godot Discord server](https://discord.gg/godotengine) and answer people's questions.
	- You can also answer people's questions on the [Godot forums](https://forum.godotengine.org/) or just share valuable resources with the world.
- Download unstable versions of the engine, such as dev, beta and release candidate from [here](https://godotengine.org/download/archive/) to test if your projects work correctly. Back up your projects first!
	- If you're not on a commonly used platform such as Windows, like i am on Linux, please do this. I found an [engine-breaking bug](https://github.com/godotengine/godot/issues/106433) that nobody had noticed and it was very bad.
- Report the bugs that you find on [Godot issues](https://github.com/godotengine/godot/issues).
	- If someone already found a bug you know, please visit their issue and explain how you experienced it. This will help narrow down the problem.
- Propose ideas that you have on [Godot proposals](https://github.com/godotengine/godot-proposals/discussions).
	- Also if you've got the full technical details on how to implement the idea, propose it in [Godot proposal issues](https://github.com/godotengine/godot-proposals/issues).
- Fork [Godot](https://github.com/godotengine/godot), make your own branches such as `test/some-test` and do some experiments.
	- I used AI here to point me in the right direction because it can be very overwhelming when you're new to a massive codebase like this. The AI can tell you which files to edit, explain what does what, explain why things are written the way they are, why Github builds fail and sometimes even half-ass code things for you. However don't do it recklessly. I already have a blog post covering that: <https://tomsterbg.github.io/programming-with-ai-correctly>.
- Read [good first issues](https://github.com/godotengine/godot/issues?q=is%3Aissue%20state%3Aopen%20label%3A%22good%20first%20issue%22) to see if you can implement a fix for any of these. A "good first issue" label means it's probably easier to implement.
	- Personally i recommend to name your branches something like `feat/some-feature` or `pr/some-feature`. I am still figuring it out, but for now i use `feat/` for features and then i clone the branch to a `pr/` branch when i'm absolutely ready to make a pull request.
	- Specifically for pull requests this is a good read: <https://docs.godotengine.org/en/stable/contributing/workflow/pr_workflow.html>.
	- There are a couple trackers, find them by searching `[TRACKER]` and use them for combined work such as fixing small typos in the documentation and adding unit tests.
	- Read the documentation and see if you can improve it.
- Read [Godot proposals](https://github.com/godotengine/godot-proposals/discussions) and try to make your own mock of the proposal, perhaps in a `feat/` branch. Then make a video of how it works and share it in the replies of that proposal.
	- Seeing is more powerful than talking, and when you've already implemented it, you can link to your branch so other people know how you did it. I did exactly that [here](https://github.com/godotengine/godot/pull/92039) because people just can't agree on a solution to the pull request, so i made my own solution, recorded a video of how it works and linked to my code if anyone would like to know how it works. I'm not trying to boast, but seeing an example in action helps.

As you can see, there are literally dozens of ways in which you can help the engine. However, there are also other things that you can do:

- Use addons and provide feedback to the author of the addon. Bugs, features, same deal as contributing to Godot, but for an addon this time.
- Make addons and share them.
- Make videos. Be it promotional, tutorials, showing an addon and explaining how to use it, explaining a feature of Godot, showing how you work with the engine normally, etc.
- Make forum posts that explain how to do this and that.
- Contribute to addons made for Godot, most have a Github repository. Find bugs, request features, add features, say thanks.

Now, let's dive into the specifics.

# I can't compile the engine

I can't too, don't worry. My laptop gets so hot that it simply crashes. Github has a solution for this.

Godot automatically builds `artifacts`. To find them, go to the Godot Github page and look at [the commits](https://github.com/godotengine/godot/commits/master/). Look for a colored dot or check with a number like `20/20`. Clicking that opens a menu saying "All checks have passed" or something else, depending on the status of the checks. From there you can click on details and in this new interface, click on summary. Scroll to the bottom and you'll see downloadable artifacts.

There are multiple types of artifacts. Some are editors, some are templates. The editors are the engine itself, and the templates are how you export your game to other people, for example on itch or Steam. I'm not familiar with how custom templates work, so i'll stick to editors.

I personally use the only downloadable editor on Linux as of now, which is the Mono (basically normal editor, but also supports C# with .NET). Other editors are compiled, but the Github automation file says something like `artifact = false` which means that build won't be downloadable. You can easily change that, but only if you find where it is.
