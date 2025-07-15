# Number Guessing Game in Python

A fun and interactive **Number Guessing Game** built with Python. The computer randomly selects a number between  **1 and 100** , and the player tries to guess it with helpful hints provided after each guess.

## Features

* Random number generation between 1 and 100
* User-friendly prompts and instructions
* Hint system: tells whether your guess is too high or too low
* Input validation: ensures only integers between 1 and 100 are accepted
* Keeps track of number of guesses
* Handles invalid inputs gracefully

## How It Works

1. The computer selects a random number between  **1 and 100** .
2. The user is prompted to guess the number.
3. After each guess, the program tells the user:
   * If the guess is too **high**
   * If the guess is too **low**
   * If the guess is **correct**
4. The game continues until the user guesses the correct number.
5. It displays the number of attempts used to guess correctly.

## How to Run

1. Make sure you have Python installed. You can download it from: [https://www.python.org/downloads/](https://www.python.org/downloads/)
2. Save the code into a Python file, for example: `guessing_game.py`
3. Run the game using the terminal or any Python IDE:

## Screenshots
## Code:
![image]()
## Output:
![image]()

## Video:
[Video on YouTube]()

## Explaination

1. import random

This imports Python’s built-in random module.
The random module is used for generating random numbers.
We use this module to generate a random number the player has to guess.

2. def guessing_number():

This defines a function named guessing_number.
All the code inside the function is indented and will run only when the function is called.

3. n = random.randint(1, 100)

random.randint(a, b) generates a random integer between a and b (inclusive).
So here, n will hold a number randomly chosen between 1 and 100.
This is the target number the user has to guess.

4. guesses = 0

Initializes a counter to track how many guesses the user takes.
Every time the user enters a guess, this counter increases by 1.

5. Printing Instructions

print("\n*** Number Guessing Game ***")
print("I have selected  number between 1 and 100.")
print("Can you guess what it is?")
This provides a friendly intro and instructions to the player.
The \n adds a blank line before the game title for cleaner output.

6. while True:

This creates an infinite loop — it will keep running until we break it.
Perfect for games where we want to keep asking until a correct guess is made.

7. try: ... except ValueError:

This block is used for exception handling.
It protects your program from crashing if the user enters something that isn’t an integer (like a word or symbol).

8. user_guess = int(input("Enter your guess: "))

The input() function takes user input as a string.
We convert it to an integer using int().
If the input isn't a number (e.g., "hello"), it raises a ValueError, which is caught in the except block.

9. guesses += 1

Increments the guess counter every time the user enters a valid guess.

10. Input Range Check

if user_guess < 1 or user_guess > 100:
    print("Please enter a number between 1 and 100.")
    continue
Ensures the user only enters numbers between 1 and 100.
If they don't, the loop continues without checking if the guess is correct.

11. Comparison Logic

if user_guess < n:
    print("Your Guess is Lower than My Guess! Try again.")
If the guess is lower than the correct number, we give a hint to try a higher number.

elif user_guess > n:
    print("Your Guess is Higher than My Guess! Try again.")
If the guess is higher, we tell the user to try a smaller number.

else:
    print(f"Congratulations You guessed the number {n} correctly in {guesses} guesses.")
    break
If the guess matches the correct number:
Congratulate the user.
Show the total number of attempts.
Use break to exit the loop and end the game.

12. except ValueError:

print("Something Wrong!!,Enter an Integer Number")
This is executed when the user enters non-integer input (like "hello", "4.5", etc.).
It avoids crashing and prompts the user to enter a valid number.

13. guessing_number()

This is the function call that starts the game.
Without this, nothing would run even though the function is defined.


Author
**Ashish Yadav**
GitHub: [@ashishyadav-1510](https://github.com/ashishyadav-1510)
