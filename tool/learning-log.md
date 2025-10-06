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
