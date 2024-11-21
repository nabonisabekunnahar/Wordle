Roll:2007034

# Wordle iOS Application

This is a simple Wordle game implemented in Swift as part of an iOS assignment. The app replicates the functionality of the popular word game,
where users attempt to guess a 5-letter word in six attempts. It was developed using Storyboard and Swift, based on a tutorial for beginners.

![image_alt](https://github.com/nabonisabekunnahar/Wordle/blob/main/image.png?raw=true)

## Features

### Game Board:

Displays the current guesses in a grid layout.
Each row represents a single guess.

### Colors indicate feedback:

#### Green: Correct letter in the correct position.

#### Orange: Correct letter in the wrong position.

#### Gray: Incorrect letter.

### On-Screen Keyboard:

A virtual keyboard for user input.
Automatically updates the grid based on user input.

### Interactive Gameplay:

Immediate feedback for each guess.

## Code Overview:

#### BoardViewController
   
Manages the game board display using a UICollectionView.
Dynamically updates cell colors based on the user's guesses.
Implements the BoardViewControllerDatasource protocol to interact with the main game logic.

#### KeyboardViewController

Displays the virtual keyboard using a UICollectionView.
Sends user input (letters) to the main game controller through the KeyboardViewControllerDelegate protocol.

#### ViewController

Main game logic controller.
Manages the interaction between the board and keyboard.
Tracks the current guesses and the correct answer.
Implements:
KeyboardViewControllerDelegate for handling keyboard inputs.
BoardViewControllerDatasource for providing data to the game board.

#### KeyCell

Represents individual keys in the keyboard and letters on the board.
Configures appearance dynamically based on the input or feedback.

##### This project was created by following a Wordle tutorial designed by Afraz Siddiqui, available on YouTube. 




