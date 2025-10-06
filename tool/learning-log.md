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

#### Challenges

#### Questions

#### Next Steps



<!-- 
* Links you used today (websites, videos, etc)
* Things you tried, progress you made, etc
* Challenges, a-ha moments, etc
* Questions you still have
* What you're going to try next
-->
