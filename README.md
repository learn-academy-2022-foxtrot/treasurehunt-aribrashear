# 💰 React Treasure Hunt Game

As a developer, you are tasked with creating a treasure hunt game. The user will see a game board on the page and be able to select various squares on the board. Hidden behind one square is a treasure that will win the game and hidden behind another square is a bomb that will lose the game. All other squares will reveal a neutral image. The user will be given a particular number of clicks to find the treasure that will win the game.

### 🤔 Remember

- Pseudocode!!
- Ask clarifying questions

### 📚 User Stories

- As a user, I can see a page with a three by three grid board game with a question mark in each square.
  -- Branch: board-game
  -- mapped over array in state to dynamically render 9 squares
  -- used flexbox to position the squares
  -- passed the value of the array in state to square
  -- styled the square
- As a user, when I click on one of the question marks an alert appears with the index position of that question mark in the array.
  -- Branch: index-position
  -- added an onClick to the square div
  -- added a handleClick method to square
  -- passed index to square and to the handleClick
  -- created handleGamePlay in App.js
  -- passed handleGamePlay to square to get the index through functional props
- As a user, when I click on one of the question marks instead of the alert the question mark turns into a tree emoji.
  -- Branch: tree-emoji
  -- made a copy of the board with the spread operator
  -- updated the value at the particular index to be a tree emoji
  -- emoji keyboard is: ctrl + cmd + space
- As a user, if I select the winning square the question mark will become a treasure emoji and if I select the losing square the question mark will become a bomb emoji.
  -- Branch: treasure-bomb
  -- added random location for bomb and treasure into state
  -- added a conditional in the handleGamePlay method to produce different outcomes
- As a user, I can click on a “Play Again” button that will restart the game.
  -- Branch: game-reset
  -- added a button which will reset the state of setBoard to its original value, and set the state of both treasureLocation and bombLocation to new random numbers.
- As a user, I can see a counter that shows how many guesses I have left. The counter starts at five and decrements one every time I click on a square that is not the treasure nor the bomb.
- As a user, I can see a message informing me that I won the game if I select the square that contains the treasure.
- As a user, I can see a message informing me that I lost the game if I select the square that contains the bomb.
- As a user, I cannot continue to play the game after I win or lose.
- As a user, I can see a message informing me that I lost the game when I run out of turns (the counter reaches zero).

### 🏔 Stretch Goals

- Consider how to handle a situation where the bomb and the treasure are at the same index.

### 👩‍💻 Developer Stretch Goals

- As a developer, I have a well commented application.
- As a developer, I have well written README file with instructions on how to access my repository.
- As a developer, my variables are all named semantically.
- As a developer, I have refactored and efficient code.
- As a developer, I have my application [deployed as a live website](https://render.com/docs/deploy-create-react-app).
