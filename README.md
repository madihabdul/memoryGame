Pre-work - Memory Game
Memory Game is a Light & Sound Memory game to apply for CodePath's SITE Program.

Submitted by: Madiha Abdul Maajid

Time spent: 6 hours spent in total

Link to project: (insert your link here, should start with https://glitch.com...)

Required Functionality
The following required functionality is complete:

[✓] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
[✓] "Start" button toggles between "Start" and "Stop" when clicked.
[✓] Game buttons each light up and play a sound when clicked.
[✓] Computer plays back sequence of clues including sound and visual cue for each button
[✓] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess.
[✓] User wins the game after guessing a complete pattern
[✓] User loses the game after an incorrect guess
The following optional features are implemented:

[✓] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
[ ] Buttons use a pitch (frequency) other than the ones in the tutorial
[✓] More than 4 functional game buttons
[✓] Playback speeds up on each turn
[✓] Computer picks a different pattern each time the game is played
[✓] Player only loses after 3 mistakes (instead of on the first mistake)
[✓] Game button appearance change goes beyond color (e.g. add an image)
[ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
[✓] User has a limited amount of time to enter their guess on each turn
The following additional features are implemented:

[✓] Color Blind Mode: Enters the word 'click' inside the button to whichever button is being selected by the random array, and can be used at the beginning or the middle of the game
Video Walkthrough
Here's a walkthrough of implemented user stories:

Reflection Questions
If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. https://stackoverflow.com/questions/31106189/create-a-simple-10-second-countdown https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random

What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) [One challenge was getting the additional game buttons to not stay lit after being chosen in the array or after being clicked, which was fixed by adding the buttons to the freqMap. By realizing that the buttons were tied together by the playTone function due to the playSingleClue function, it would be impossible to add another working button since the .lit function and the sound were intertwined. Another challenge was getting the timer to restart, which was fixed by placing timeleft=0 in order to reset the timer. Instead of complicating it with a initialized true or false global variable, by setting the if statement to <= 0 it allowed for the timer to restart itself given that in certain conditions such as losing (either through running out of time or strikes, winning, or pressing the stop button) that the timer resets itself without it having a problem with counting down again. A similar method was used for the strikes. Another challenge with color blind mode was the buttons moving down after showing the 'click' keyword which was fixed by adding specific decorators to the button master class by adding vertical-align: top so that the element that is added to the button doesn't move what is inside the div. The function was also not starting initially, so by adding the !colorBlindMode it was able to start by revering the button.]

What questions about web development do you have after completing your submission? (recommended 100 - 300 words) [Questions that I have about web development is how to make the code more efficient. By minimizing my functions and variables to only necessities for functions, as well as assignment certain functions to variables it was easier to bind certain properties together. With that in mind, learning about how each of the elements, properties, etc. can be used in different strategies in order to make code as efficient and as customizable as possible is something that I would be interested in learning.]

If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) [I would add a difficulty selector like Easy, Medium, or Hard Mode. As well as buttons where users are allowed to customize their own game with as many buttons as the want as well as setting up the speed interval. I would also add specific color blind modes such as red-green color blind.]

License
Copyright [Madiha Abdul Maajid]

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.