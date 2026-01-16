# Entry 2
##### 1/15/26

### Context
Me and my parter Aaron have been doing more research for our game that incorporates both concepts of hangman and music into one. The tool that i am using is named [Kaboom.js](https://kaboomjs.com/). And i was able to make a sort of game menu with "music options" and i also made it able to swipe between options. My Research for the development of my game has been very slow but still very effortful nonetheless.
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
in summary my code tracks the wrong guesses that the player makes, stores drawing insturctions, and draws the parts that are supposed to be visual, and automatically updates. which to summerize it this code basically removes a part of the hang man everytime you make an incorrect guess.
in depth explaination:
* "let mistakes =0" stores the amount of wrong guesses a player made. it starts at 0 since no mistakes were made yet
* "const hangmanParts=[...]" is an array of functions were each function draws a specifc part of the body and the body part is only drawn when the function is called.
* "onDraw(() => {...})" in my opinion the most important part because Kaboom runs it in every frame
   which is usually 60 times per second and it clears the screen and redraws it every time.
* "for" is a loop and it starts at 0 and stops when "mistakes-1" and it calls each drawing function which basically creates the full hangman.
* 
### Egineering Design Process
This is a early version of my product that me and my partner am unsure of keeping/scraping just because we feel as if we could do better and change some things about the current code. Me and my partner still need to figure out how to incorperate music into the game and how music will take part creating the hangman. 

### Sources
A few sources that were useful to me include:
* [snakegame youtube video](https://www.youtube.com/watch?v=2pl7I16CkHs&t=99s) 
* [kaboom.js youtube video](https://www.youtube.com/watch?v=iRXI6ThRJvM)
* [awesome-kaboom](https://github.com/kaplayjs/awesome-kaboom?utm_source=chatgpt.com)

these resources gave me an introduction into creating a game with Kaboom.js without giving me full answers on what was required of me and my partner aaron to code a version of Hangman.

### Skills
* collaberation
* revising
* coding grammer
* time management
these are a few skills that i have gained throughout this process since i had to do teamwork with my partner aaron, manage school work/classwork, and revise my code for mad grammer since code wont run depending on captialization/typos(very simple but very complicated(imo).

[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)
