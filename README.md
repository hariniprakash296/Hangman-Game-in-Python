# Hangman-Game-in-Python Credits to tacarpe(github)
A game designed for anyone who likes hangman
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
