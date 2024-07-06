# Number Guessing Game

This project is a bash script that implements a number guessing game. It interacts with a PostgreSQL database to store user information and game statistics.

## Game Description

The Number Guessing Game is a simple, interactive game where:

1. The user is prompted to enter their username.
2. If it's a new user, they are welcomed to the game.
3. If it's a returning user, they are greeted with their game history.
4. The script generates a random number between 1 and 1000.
5. The user is asked to guess the number.
6. After each guess, the user is told if their guess was too high or too low.
7. The game continues until the user guesses the correct number.
8. Once the correct number is guessed, the user is told how many guesses it took.

## Script Details

The `number_guess.sh` script:

- Uses PostgreSQL to store and retrieve user data.
- Implements functions for creating users, finding users, and playing the game.
- Handles input validation to ensure only valid integer guesses are accepted.
- Updates the user's game statistics after each game.

## Database Structure

The game uses a PostgreSQL database named `number_guess` with a `users` table that stores:

- Username
- Number of games played
- Best game (lowest number of guesses)

## How to Run

1. Ensure you have PostgreSQL installed and the `number_guess` database set up.
2. Run the script using: `./number_guess.sh`

## Files in this Project

- `number_guess.sh`: The main bash script for the game.
- `number_guess.sql`: A SQL dump of the database structure and data.

## Note

This project was completed as part of the freeCodeCamp Relational Database certification.
