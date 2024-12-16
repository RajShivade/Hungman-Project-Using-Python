# Hangman Project Using Python :-

# Project Structure:
The project consists of a single Python script that contains all the necessary code to run the Hangman game. The main components of the game logic include:

- **Word Selection:** Randomly selecting a word from a predefined list.
- **Game Loop:** Handling user inputs and updating the game state.
- **Display Functions:** Showing the current state of the game, including the word with guessed letters and remaining attempts.
- **Win/Loss Conditions:** Checking if the player has won or lost the game.

# Game Logic: 
# 1. Word Selection
The game starts by randomly selecting a word from a predefined list of words. This word will be the target that the player needs to guess.
import random

words_list = ['python', 'hangman', 'programming', 'data', 'science']
word = random.choice(words_list).upper()
# 2. Game Loop:
The main game loop handles user inputs and updates the game state accordingly. The player is prompted to guess a letter, and the game checks if the letter is in the word.
attempts = 6
guessed = False
guessed_letters = []
guessed_words = []
word_completion = "_" * len(word)

while not guessed and attempts > 0:
    guess = input("Please guess a letter or word: ").upper()
    # Logic to handle guesses
# 3. Display Functions:
Functions to display the current state of the game, including the word with guessed letters and remaining attempts, are used to provide feedback to the player.
def display_hangman(attempts):
    # Visual representation of hangman based on the number of attempts left
    pass

def display_word_completion(word_completion):
    print("Current word: " + " ".join(word_completion))
# 4. Win/Loss Conditions:
The game checks if the player has successfully guessed the word or if they have run out of attempts.
if "_" not in word_completion:
    guessed = True
    print("Congratulations, you guessed the word!")
elif attempts == 0:
    print("Sorry, you ran out of attempts. The word was " + word + ".")
# How to Play:
- The game will display a series of underscores representing the letters in the target word.

- You will be prompted to guess a letter or the entire word.

- If the guessed letter is in the word, it will be revealed in its correct position(s).

- If the guessed letter is not in the word, you will lose one attempt.

- The game continues until you either guess the word correctly or run out of attempts.

# Features:
- Random Word Selection: Words are randomly selected from a predefined list.

- Multiple Attempts: Players have a limited number of attempts to guess the word.

- Visual Feedback: The game provides visual feedback on the guessed letters and remaining attempts.

- Win/Loss Conditions: The game checks for win or loss conditions and displays appropriate messages.

  # Conclusion:
  This Hangman game project provides a simple yet engaging way to practice Python programming concepts such as loops, conditionals, functions, and user input handling. Feel free to explore and enhance the game with additional features and improvements. If you have any questions or suggestions, please don't hesitate to reach out!
