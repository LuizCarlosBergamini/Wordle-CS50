# Wordle Game
![Wordle working animation](https://github.com/LuizCarlosBergamini/Wordle-CS50/assets/109323370/d72cab6b-3976-41cf-813e-6a6fc9d33e07)

This is a simple command-line word-guessing game called Wordle50. The game challenges you to guess a word within a limited number of tries. You will receive feedback on each guess to help you narrow down the correct word.

## Prerequisites

To play Wordle50, you need to have the following installed:

- `gcc` compiler
- `cs50` library

## Getting Started

1. Clone the repository or download the source code files.
2. Compile the code using the `gcc` compiler with the following command:
```bash
gcc -o wordle wordle.c -lcs50
```
3. Run the game by executing the compiled binary:
```bash
./wordle <wordsize>
```
Replace `<wordsize>` with the desired size of the word to be guessed (5, 6, 7, or 8).

## How to Play

1. Upon starting the game, you will be provided with the number of tries you have to guess the word.
2. Enter a word of the specified length when prompted. Make sure to input a word with exactly the same number of characters as the word to be guessed.
3. After each guess, the game will provide feedback based on the correctness of the letters in your guess.
- Green letters indicate correct letters in the correct positions (EXACT).
- Yellow letters indicate correct letters in incorrect positions (CLOSE).
- Red letters indicate incorrect letters (WRONG).
4. Keep guessing and using the feedback to narrow down the word.
5. If you guess the word exactly within the given number of tries, you win! Otherwise, the game will reveal the target word.

## Custom Word Lists

The game uses word lists stored in text files (`5.txt`, `6.txt`, `7.txt`, `8.txt`) that contain 1000 words each. You can modify or replace these files to use your own word lists. Each word should be on a separate line, and the number of words in each file should remain the same.

## Note

The game uses ANSI color codes to provide a more visually appealing experience. Please ensure that your terminal supports ANSI escape sequences for proper color rendering.

## Acknowledgments

The Wordle50 game was developed using the C programming language and the CS50 library.

Enjoy the game and have fun guessing words!
