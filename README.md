# Hangman-Game-in-Python Credits to tacarpe(github)
A game designed for anyone who likes hangman
For a game where user is unable to guess:

![image](https://user-images.githubusercontent.com/70060391/176085167-c043ac04-7c4b-4696-9c86-387a4a608689.png)
![image](https://user-images.githubusercontent.com/70060391/176085174-630287c3-55e6-4efe-9dc5-ebc525c161cf.png)
![image](https://user-images.githubusercontent.com/70060391/176085254-cdcd7d9d-8e46-4b5a-a07a-4abfa9cb02cd.png)

For a game where user guesses the word:
![image](https://user-images.githubusercontent.com/70060391/176085358-a84f5374-841d-4cdc-9461-0f9d73775539.png)
![image](https://user-images.githubusercontent.com/70060391/176085378-6ca09295-e88c-43f6-9540-5e0995df20f1.png)
![image](https://user-images.githubusercontent.com/70060391/176085404-ecfcd74b-154b-4407-8658-19344f9835de.png)

Get word list
def get_word:
Get random word from the word list file as a variable and convert it to uppercase using .UPPER()
We convert to uppercase so that all user input that is mapped may be verified w the uppercase letters in the word
Def play:
This will be used for interactive play by updating several variables created after each turn the user takes
VARIABLES for Word Completion:
-Display word during each turn
-Represent unguessed letters as underscores and show the letters as correct guesses are made( This will be the same length as the chosen word)
-A variable guess is created and initialized to false
-Create 2 lists: one to hold the letters the users guess and the other to hold the words the user guesses
-A variable tries that corresponds to the number of body parts left to be drawn on the hangman before the user loses [initialised to 6 Counting Both arms, both legs, head and body]

WHILE LOOP:
If the user still has tries, asks for:
-User input
3 conditional cases:
Guessing a letter
If-else: Guessing the same letter, is not in the word, or is in the word Then subtract tries by 1
Guessing a word
Typing something other than a single letter or word of the correct length
IF?ELSE:
To check if the user guessed the word or ran out of tries
If the user guessed, congrats
If the user lost, you lost, the word was “word variable”
Def display_hangman:
This list contains the visual stages of hangman. Each stage corresponds to the number of tries the user has left

Def Main:
Get the word and pass it to play() for running it once
Option for user to PLAY AGAIN:
While loop
