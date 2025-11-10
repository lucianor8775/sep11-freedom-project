# Tool Learning Log

## Tool: **earsketch**

## Project: **music app**

---

### 10/5/25:
#### Links
[EarSketch](https://earsketch.gatech.edu/landing/#/)

[Youtube](https://www.youtube.com/watch?v=KpEKplkGWhg)

#### Tinkering
```js
// Setup
init();
setTempo(100); // Sets tempo to 100 BPM

// Select sounds
var kick = "HipHop:Kick03";
var snare = "HipHop:Snare03";
var synth = "Electronic:SynthLoop01";

// Add kick on every beat for 4 measures
fitMedia(kick, 1, 1, 5);

// Add snare on beats 2 and 4 (offset by 0.5 measure)
fitMedia(snare, 2, 1.5, 5);

// Add synth loop in the background
fitMedia(synth, 3, 1, 5);

// End script
finish();
```
This code sets the tempo to 100 beats per minute, makes a kick drum plays every beat from 1 to 5, a snare hits on every off beat, and theres a synth like loop that plays behind the beat.
* tempo is the speed at which music is played
* kick drum is a type of drum
* a snare is a type of drum that produces a rattling sound and
* a synth loop is a repeating sound created by a synthesizer which is played back to make it repeat
#### Challenge
```js
fitMedia(snare, 2, 1.5, 5);
```
This part of the code was a bit challenging because earsketch uses music time not seconds, so 1.5 means measure 1 beat 3(each measure has 4 beatsin 4/4 time) this was hard because i couldnt align sounds with beats good enough using the musical time instead of the actual time
#### Questions
not any at the moment but ill try to research deeper
#### Next Steps
For my next learning log i would like to try dive deeper into Earsketch and learn how to make music that i like so that i can develop my coding skills.


<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->

## Tool: **Kaboom.js**

## Project: **music/hangman game**

---

### 10/5/25:
#### Links
[Kaboom](Kaboom.js.com)

[Youtube](https://www.youtube.com/watch?v=iRXI6ThRJvM&list=PLNwtXgWIx3rgk68WwrykC7BIJ50kT6ZpS&index=1)

#### Tinkering
```
loadSound("bgm", "assets/music/bgm.mp3")

// Because browsers block autoplay, wait for a click first
onClick(() => {
  play("bgm", {
    loop: true,   // repeat forever
    volume: 0.5,  // half volume
  })
  add([
    text("Music is playing 🎵", { size: 24 }),
    pos(24, 24),
  ])
})

add([
  text("Click anywhere to play music", { size: 24 }),
  pos(24, 24),
])
</script>
```
This code plays background music when you click on the screen(used in my blog) This is one of the first things that I learned because it will be very useful to me in the future because the website i will make is going to include a lot on music
* Bgm.mp3 is the background music that will be played
* ``loop: true``makes the background music play forever
* ``add([...])``is what added the text on the screen
  
#### Questions
how do I make objects move in the game

#### Next Steps
For my next learning log I want to have a plan for my portion of the website because I am working with a partner. I would also love to have a general idea for the way that our website is gonna look/behave.


<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
