# Entry 2
##### 1/15/26

### Context
me and my parter Aaron have been doing more research for our game that incorporates both concepts of hangman and music into one. The tool that i am using is named [Kaboom](https://kaboomjs.com/). and i was able to make a sort of game menu with "music options" and i also made it able to swipe between options. My Research for the development of my game has been very slow but still very effortful nonetheless.
code snippet:
```js
// number of wrong guesses (0–6)
let mistakes = 0;

// cute pink hangman parts (drawn step-by-step)
const hangmanParts = [
  // head
  () => {
    drawCircle(vec2(600, 200), 20, {
      color: rgb(255, 105, 180),
    });
  },

  // body
  () => {
    drawLine(
      vec2(600, 220),
      vec2(600, 280),
      {
        width: 4,
        color: rgb(255, 105, 180),
      }
    );
  },

  // left arm
  () => {
    drawLine(
      vec2(600, 240),
      vec2(570, 260),
      {
        width: 4,
        color: rgb(255, 105, 180),
      }
    );
  },

  // right arm
  () => {
    drawLine(
      vec2(600, 240),
      vec2(630, 260),
      {
        width: 4,
        color: rgb(255, 105, 180),
      }
    );
  },

  // left leg
  () => {
    drawLine(
      vec2(600, 280),
      vec2(580, 320),
      {
        width: 4,
        color: rgb(255, 105, 180),
      }
    );
  },

  // right leg
  () => {
    drawLine(
      vec2(600, 280),
      vec2(620, 320),
      {
        width: 4,
        color: rgb(255, 105, 180),
      }
    );
  },
];

// draw hangman based on mistakes
onDraw(() => {
  for (let i = 0; i < mistakes; i++) {
    hangmanParts[i]();
  }
});
```
The most important part of my code is
```
function createPinkHangman() {
  let mistakes = 0;

  const hangmanParts = [
    () => drawCircle(vec2(600, 200), 20, { color: rgb(255, 105, 180) }),
    () => drawLine(vec2(600, 220), vec2(600, 280), { width: 4, color: rgb(255, 105, 180) }),
    () => drawLine(vec2(600, 240), vec2(570, 260), { width: 4, color: rgb(255, 105, 180) }),
    () => drawLine(vec2(600, 240), vec2(630, 260), { width: 4, color: rgb(255, 105, 180) }),
    () => drawLine(vec2(600, 280), vec2(580, 320), { width: 4, color: rgb(255, 105, 180) }),
    () => drawLine(vec2(600, 280), vec2(620, 320), { width: 4, color: rgb(255, 105, 180) }),
  ];

  onDraw(() => {
    for (let i = 0; i < mistakes; i++) {
      hangmanParts[i]();
    }
  });

  return {
    addMistake() {
      if (mistakes < hangmanParts.length) mistakes++;
    },
    reset() {
      mistakes = 0;
    },
    getMistakes() {
      return mistakes;
    },
  };
```
### Egineering Design Process


### Sources
a few sources that were useful to me include:
*[

### Skills

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
