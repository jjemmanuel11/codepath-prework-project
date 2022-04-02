# codepath-prework
Codepath prework project

# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: Emmanuel Nidea

Time spent: 4 hours spent in total

Link to project: https://glitch.com/edit/#!/aquamarine-extreme-authority

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

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:

![]<img src="http://g.recordit.co/jlTKOfksJM.gif" width = 250><br> 
![]<img src="http://g.recordit.co/Rk0LwLgEn6.gif" width = 250><br>
![]<img src="http://g.recordit.co/T2BKALSAiS.gif" width = 250><br>
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
-https://www.rapidtables.com/web/color/RGB_Color.html

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
One challenge that I encountered was in debugging my code. After writing the code to play a single clue, I checked the preview panel and found that the game was only playing a tone withouting lighting up its corresponding button. Initially, I thought that the problem was in my lightButton function, and so to check that the function was even running, I added a print statement directly below the line in the playSingleClue function in which the lightButton function was called. After running my code again, I checked the console and found that the lightButton function was in fact running as indicated by the printed message to the console. Knowing this, I postulated that the problem must have to do with the connection of the computer playing a clue and the lighting up of the buttons. I began to investigate the body of the function by checking whether it was correctly modifying the document object model to add the lit class to the corresponding HTML element. After analyzing my JavaScript and CSS file, I realized that I had neglected to change the selector in my CSS file to include the lit class to its class list. In failing to include the lit class, the selector was unable to target buttons with the CSS class lit which prevented the buttons from being lit up when the lightButton function within playSingleClue was called. After isolating this bug, I proceeded to edit my code in my CSS file to include #buttonX.lit to the proper selectors. 


3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
This project was very engaging in that it provided me with a solid introduction to web development that left me wanting to learn more. On the front end side of things, I want to learn how to implement more complex visual elements to a project. For example, how do you implement an animation? And how can you integrate it into a website so that a user can interact with it? But beyond the visual aspects of web development, I want to know what steps web developers take to optimize their websites’ speeds. What tools or systems do web developers use to decrease website loading times? Furthermore, where does time complexity come into play? There are many factors that come into play when it comes to web development. I want to learn more about how front and back end code use these factors to come together to create seamless and elegant websites in hopes that I can one day make my own.


4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
If I had a few more hours to work on this project, I would add a mode to the game in which it can be reconfigured into an audio/tone game to help young or new musicians train their ears to differentiate between tones. In this mode, I would eliminate the use of the lightButton function which would prevent the player from observing which button’s tone was played aloud. To accomplish this, I would first  add four more buttons and change the tones of each button to create a musical scale of tones from left to right. I would then add a function that alerts the player, via a visual cue, that the sequence of tones is being played. The rest of this game mode’s functionality is similar to the original light and sound memory game. The computer would play a pattern of tones, and the player would have to repeat the pattern by clicking the correct sequence of buttons. Another change I would make if I had the time would be to add a “hard” mode that would increase the difficulty of the game. There are many ways to make the game more challenging for the player. For example, we could increase the length of the pattern array or add more buttons. Personally, I would randomize the clue sequence so that it doesn’t build on from the previous sequence but creates an entirely new one. This would make the game more difficult and perhaps more fun.



## Interview Recording URL Link

[My 5-minute Interview Recording]https://northwestern.zoom.us/rec/share/mWYflvEpwSSPMfJ3jaDRZpK7Y7KOrrcfX8S9zVGN4RPU6Uzh9Je7F54Ja8CKJW71.B3U3ZADwDPXKEXCE


## License

    Copyright [YOUR NAME]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.

