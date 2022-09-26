# Hangman-project

[![forthebadge made-with-python](http://ForTheBadge.com/images/badges/made-with-python.svg)](https://www.python.org/)

This repository uses Python3 to create a game of hangman. The random library is imported to generate a list of words, which the program randomly chooses from each time the game is run. The program then asks the user to enter characters and determines whether they are contained in the unknown word. This process is repeated until the user guesses the full word, or when the user runs out of lives. 

To run this project you can clone the Github repository and use the command ```git pull https://github.com/christabelgilmour/Hangman-project.git``` in your terminal or clone the file in an application such as VS Code.

<img width="614" alt="image" src="https://user-images.githubusercontent.com/113252944/191964157-518f6bc4-41c6-496e-b781-079430239d0f.png">

Once you have opened this you are able to run the whole program and play the hangman game for yourself.

## Milestone 1 

To begin, we set up the environment and create a Github repository. 

<img width="999" alt="image" src="https://user-images.githubusercontent.com/113252944/191947298-b2b7c39f-64b0-4b96-a534-40a8b9deda63.png">


## Milestone 2

First, the program needs to ask the user for an input, the ask_letter method is used to ensure the user is entering a single character. Furthermore, this character can not have already been tried by the user.

<img width="644" alt="image" src="https://user-images.githubusercontent.com/113252944/191934596-a49d5abe-394a-4edf-a713-dfbda0c0abe8.png">


## Milestone 3

Here, we need to initialise all the attributes of the game. With this we can present the number of characters and the spaces that need to be filled of the mystery word. 

<img width="685" alt="image" src="https://user-images.githubusercontent.com/113252944/191932742-eec3fe29-4d13-4038-a3e9-fcc6166a4fc3.png">

Sets are used for the number of letters in the word and the list of letters that the user has tried to avoid issues with unique letters.

## Milestone 4

Once the conditions for the ask_letter method are satisfied, the program uses the check_letter method to determine whether the letter given is in the word. If so, the corresponding empty spaces in the word must be replaced by the letter. If the letter is not in the word, one of the users lives is lost. In each case, the letter is added to the list of letters so the user cannot retry their input.

<img width="579" alt="image" src="https://user-images.githubusercontent.com/113252944/191932977-b51d2082-299e-4181-affe-106b81c76b71.png">

We can iterate over the length of the word using a for loop. This makes sure that if the word contains the same letter multiple times, all the spaces corresponding to the specific indices are replaced by the letter.

## Milestone 5

The final step to complete this game is to make sure the game ends when either the user has guessed all the letters in the word, or when the user has run out of lives and lost the game.
It is important to make sure there is a break after the while loop in the ask_letter method otherwise the while loop in the play_game method will not be called and the program will keep asking for an input, even if the user has guessed the word or run out of lives.

<img width="657" alt="image" src="https://user-images.githubusercontent.com/113252944/191938037-e95bd952-2f20-440b-8ada-7b23a575b071.png">

For visualisation, hangman images have been added, which shows the stages after a new input is given, and a full hangman image is shown if the game is lost. Below is an example of the result if the game is lost.

<img width="158" alt="image" src="https://user-images.githubusercontent.com/113252944/191946175-bcd922a2-037c-4e99-a28c-34396b003a31.png">


