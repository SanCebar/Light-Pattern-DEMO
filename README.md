# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Robert Velasco

Time spent: 3 hours spent in total

Link to project: https://glitch.com/edit/#!/grey-hissing-opal

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough

Here's a walkthrough of implemented user stories:
![](https://cdn.glitch.com/47e1f8cc-b521-4c11-8499-2044975b4b5a%2FLIghtPatternDEMO.gif?v=1616360460793)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
  
  I mostly stuck to the tutorial provided, but I did reference the W3 Schools Website (https://grey-hissing-opal.glitch.me/) 
  for information on JavaScript and CSS styling.

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
  
  In the past, I’ve tended to avoid using global variables and constants. In fact, I have never utilized them at all. They were convenient 
  for this project, given how often the variables and constants appear across multiple functions; but, when I was implementing some of the 
  optional features, I ran into many bugs. For example, I tried to increase the game speed every turn, but after just one game, the buttons 
  were flashing far too quickly. At first, I thought I was decreasing clueHoldTime by too much, but no matter what value I chose the issue 
  persisted. I finally realized I had to reset the variable clueHoldTime within startGame(). A similar issue happened when I tried 
  implementing the random pattern feature. With every new game, the pattern size increased. I spent at least 20 minutes on W3 schools 
  relearning the syntax for arrays in javascript, believing that was my issue. However, once again, I needed to reset the pattern variable in startGame(). 

  It was constant trial and error when debugging. At some points I needed to take a break away from the screen and just think about the code 
  in my head. However, once I pinpointed global variables as my weakness, the rest quickly resolved itself.


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 

  Immediately, I’m curious about the pipeline for implementing new ideas within a larger group. What is the process from start to finish? 
  Furthermore, I’m curious about how web development work is divided. For this kind of project, would one person take charge of the JavaScript 
  while another focuses on the CSS and overall visuals of the web app? In this case, I think a front-end developer can accomplish all tasks, but 
  when working on a larger project, how is the work generally divided?

  I’m especially curious about security considerations for web development. Is it something to worry about at every step of development or just 
  for back-end developers maybe? What are some key characteristics of secure code that is resistant to hacking?


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 

  I have a number of features I would love to implement apart from the ones mentioned in the assignment. Players could have the option to 
  increase the size of the pattern array for a longer game. Players could toggle the increasing speed on and off. They could choose a different 
  set of audio options like animal noises or guitar strings. Building on this, the player could enter a creative mode where it’s possible to alter 
  the individual visuals and sounds of the buttons, including the ability to add or remove buttons. Within this creative mode, players could save 
  their own pattern to share with friends. An example implementation is to have enough buttons with hidden letters that print a secret 
  message (like “Prom?” or “Happy Bday”) as the game progresses.

  Beyond that, I think mapping the buttons to the keyboard would make the experience much more fun and interactive. 


## License

    Copyright Robert Velasco

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.