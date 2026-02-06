---
title: "🧑🏻‍🍳 Here's what I've made :)"
permalink: /projects/
collection: projects
---

---
# Make your own TTS

What if you were VCing with friends, and you couldn't talk, but you could type? <br>
Jumpscare them with a voice that sounds *almost* like you (but still isn't quite there)?

That's the idea I've had now for a few years.
Specifically, making a text-to-speech based on your own voice.
This isn't a task I want to abstract to a single deep learning model,
because even though that yields better results,
it removes all of the linguistics involved, and what's the fun in that? <br>
Now I can leverage a bunch of knowledge from phonetics, phonology, prosody, and more! <br>
Here's how it works:
- Record your voice saying a bunch of curated sentences (the more, the better)
- Wait a few minutes for [MFA](https://montreal-forced-aligner.readthedocs.io/en/latest/){:target="_blank"}
to segment into phonemes and store their data
- Run the program, and type what you want your new TTS to say (in questionable quality), and you'll get an audio file :)

Currently, I've gotten the base version working locally, and am in the process of fine-tuning the [algorithm](https://en.wikipedia.org/wiki/Viterbi_algorithm){:target="_blank"} that decides which segments to concatenate.

---
<!-- All this inline code is for the sake of a wrap-text-style position for the video -->
<div style="display: flex; flex-direction: row; align-items: flex-start; justify-content: space-between; gap: 20px; width: 100%; margin-bottom: 20px;">
    <div style="display: flex; flex-direction: column; flex: 1;">
        <h1 style="margin-top: 0; margin-bottom: 5px; line-height: 1.2;">
            1v1 me in Word Hunt 
        </h1>
        <small style="color: #666; font-size: 0.9em; line-height: 1.4;">
            (I'll play you back) <br>
            (my wins as of 2/5/26 -->)
        </small>
    </div>
    <div style="flex-shrink: 0; width: 15%; max-width: 400px;">
        <video width="100px" autoplay loop muted style="display: block; border-radius: 4px;">
            <source src="/files/wins.mov" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>
</div>

I think I speak for everyone when I say there *has* to be a better way of improving at this game than just playing more.
What if you want to see which of the possible words you missed? GamePigeon makes you pay for that stuff...
That's why I implemented the game in Godot, so you don't have to pay,
and so I could fully customize the game to my heart's content :) <br>

The alpha release is playable [here](https://1ary.itch.io/laryhunt){:target="_blank"}. <br>
I didn't worry so much about graphics.
Instead, I was more interested in what words I was missing the most,
and definitely what they meant so I could actually remember them. <br>
Give it a shot! I recommend keyboard input if playing on your computer and touch/"mouse" input for mobile devices.
Your stats will be stored in your cookies, as per games on itch.io that save data.

---
# Course projects at CMU
- 15440: Distributed Systems
    - Stub library for remote file operations (C) <!-- consider adding tags for programming languages? -->
    - File-caching proxy (Java)
- 15213: Introduction to Computer Systems
    - Malloc lab: Dynamic memory allocator 
    - Cache lab: ...
    - Attack lab: ...


