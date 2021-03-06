# Milestone Project 1

## UX

### Project Goals
The goal of Memory Master is to provide a fun card/pattern matching game that is easy to play. The game is suitable for children and adults

#### Player Goals
Player goals are
- A fun game to play
- Easy to understand controls
- Clearly recognisable cards/patterns
- Visual and audio feedback
- A "best score" counter
- Adjust difficulty to suit age and/or time available for play

Developer and Business goals
- A game that can entertain children and pass time for adults in waiting rooms
- Programming that will handle unexpected behaviour well, e.g. will double check before resetting user progress
- Add a javascript project to his portfolio

#### User stories
As an adult I want...
1. Different difficulty options to suit the amount of free time I currently have
2. To be able to set a high score and try to beat it
3. The number of matches made to be visible on screen
4. Visual feedback on which cards are already matched

#### As a child I want...
1. To change the difficulty to suit my age
2. Audio and visual feedback on my progress
3. Easily recognisable cards/patterns
4. Acknowledgement when I set a new high score or "good" score (i.e. close to high score)

![Changing difficulty and high score/number of matches made](assets/readme-screenshots/difficulty.png)
![Visually see which cards are matched](assets/readme-screenshots/matched-cards.png)
![Visual feedback when cards don't match](assets/readme-screenshots/feedback.png)
![High score messaging](assets/readme-screenshots/high-score.png)
![Confirmation required to restart game](assets/readme-screenshots/reset-confirmation.png)


### Design Choices
The game is designed to feel like it is being played on a real board with real cards to help immerse the player. The design choices were made around this theme.

#### Fonts
- The primary font chosen was Permanent Marker. This font appears in a handwritten style and adds to the feel of realism in the game
- The secondary font chosen was Handlee, again because its style is handwritten, but also because it's more compact and easier to read

#### Images
- The card images were chosen as they would be easy to recognise for both adults and children

#### Colours
- The primary colour chosen is green to simulate playing on a green felt board
- Black and red are also chosen as they are commonly used in card games. This will help to immerse the player further
- Text may be in white/black instead of the colours chosen for accessibility reasons

#### Styling
- When the player gets a match right, a green tick is briefly shown over each card to encourage the player
- Likewise when they make a mistake, an x is shown to let them know it wasn't a match

#### Icons
- The icons were chosen to be as simple as possible. This makes it intuitive for both adults and children to understand what they do and allows them to play the game without distraction

#### Audio
- A "buzz" sound is played when when two cards don't match
- A "ding" sound is used to give positive feedback when a match is found
- A small theme tune will play when the player beats their top score 

### Wireframes
Wireframes can be viewed [here](wireframes/ms2.pdf)

## Features

### Existing Features
- Audio and visual feedback given to player
- Current and best score shown
- Turn audio on and off
- Change difficulty
- Restart game
- Show/hide instructions for game

## Technologies Used
- [HTML](https://www.w3.org/)
    - The project uses **HTML** for the content of the site.
- [CSS](https://www.w3.org/)
    - The project uses **CSS** for the layout of the site.
- [Bootstrap](https://getbootstrap.com/)
    - The project uses **Bootstrap** to give a responsive layout.
- [Font Awesome](https://fontawesome.com/)
    - The project uses **Fontawesome** to add icons.
- [javascript](https://www.javascript.com/)
    - The project uses **Javascript** to make the site interactive
- [jquery](https://jquery.com/)
    - The project uses **jQuery** to simplify and improve the site's interactivity

## Testing
1. Ran LightHouse on the page
2. Checked all code in appropriate linters (jshint.com, jigsaw CSS validator, w3c HTML validator)
3. Verify sound doesn't play when muted
4. Checked that user would be prompted before resetting game/changing difficulty, but only if they've already made a move
5. Tried clicking 3 cards in quick succession
6. Checked that help and win screens both display correctly
7. Checked that high score is kept between resets, and that appropriate message is shown if new score beats/is close to old high score

### User Story Testing
#### Adult User Story
1. Difficulty can be changed without issue.
2. High score is maintained between games and messaging is given to encourage beating it.
3. When a match is made, the number shown in the score bar is updated.
4. Matched cards are shown face up.

#### Child User Story
1. The difficulty can be reduced to show fewer cards.
2. Audio and visual feedback are given when cards are matched, different feedback is given when they don't.
3. The cards are clear and familiar
4. Different messaging is shown based on the score I set

### Issues encountered
- Handling 3 fast clicks was originally done by removing event listeners and re-adding them. This was resulting in "undefined" errors in the console. Instead a timer is set, then this is checked in the turnCard function. If the timer hasn't run out, the code will be directed to a return statement instead of executing any functionality

## Deployment

### To contribute:
1. Clone the repository using [this guide](https://docs.github.com/en/github/creating-cloning-and-archiving-repositories/cloning-a-repository)
2. Add the [Gitpod browser extension](https://www.gitpod.io/docs/browser-extension/)
3. If prompted, log in to Gitpod using your Github account

### To deploy the site
1. Log into GitHub and select the project **JoeTuohy/milestone-project-2**
2. In the menu at the top, click on **Settings**
3. Scroll to **GitHub Pages**, change the source to **Master Branch** and click **Save**
4. The site is now deployed. Scroll to **GitHub Pages** again to retrieve the URL

## Credits

### Media
#### The images used in this site were obtained from ...
- opengameart.org
- https://kenney.nl
