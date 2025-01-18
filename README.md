# Hangman Game

## Overview
This is a Python-based implementation of the classic Hangman game. Players attempt to guess a hidden word one letter at a time while avoiding incorrect guesses that reduce their remaining lives. The game continues until the player either guesses the entire word or runs out of lives.

---

## Features
1. **Random Word Selection**: Words are chosen randomly from a predefined list (`hangman_words.word_list`).
2. **Dynamic Word Display**: Displays underscores for unguessed letters and reveals correctly guessed letters as the game progresses.
3. **Lives System**: Players start with 6 lives, which decrease with each incorrect guess.
4. **Win/Lose Conditions**:
   - **Win**: Successfully guess all the letters in the word.
   - **Lose**: Run out of lives before guessing the word.
5. **Visual Feedback**: Includes ASCII art from `hangman_art` to enhance the gameplay experience.
6. **Input Validation**: Prevents players from guessing the same letter multiple times or entering invalid input.

---

## Requirements
- Python 3.x
- `hangman_words.py` containing a list of words.
- `hangman_art.py` containing ASCII art for the Hangman game.

---

## How to Play
1. Run the script in a Python environment.
2. The game will randomly select a word and display it as underscores.
3. Guess a letter by typing it when prompted.
4. If the letter is correct, it will be revealed in the word. If it is incorrect, you lose a life.
5. The game ends when you either guess the entire word or run out of lives.

---

## File Descriptions
### `main.py`
The main game logic, including word selection, player input, and win/lose conditions.

### `hangman_words.py`
A module containing a list of words from which the game randomly selects.

### `hangman_art.py`
A module containing ASCII art for the game logo and the Hangman stages.

---

## Example Gameplay
```
 _                                              
| |                                             
| |__   __ _ _ __   __ _ _ __ ___   __ _ _ __  
| '_ \ / _` | '_ \ / _` | '_ ` _ \ / _` | '_ \
| | | | (_| | | | | (_| | | | | | | (_| | | | |
|_| |_|\__,_|_| |_|\__, |_| |_| |_|\__,_|_| |_|
                    __/ |                      
                   |___/                       
Word to guess: ______
**************************** 6/6 LIVES LEFT ****************************
Guess a letter: a
Word to guess: ______
You guessed 'a'. This is not in the word. You lose a life.
```

---

## Customization
- **Adding Words**: Update `hangman_words.word_list` with new words to increase variety.
- **Adjusting Lives**: Change the `lives` variable in `main.py` to modify the difficulty.

---

## License
This project is free to use and distribute. No formal license applies.

