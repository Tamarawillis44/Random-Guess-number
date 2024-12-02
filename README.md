# Random-Guess-number

## Description

This Python program is a simple Number Guessing Game. The computer generates a random number within a specified range, and the player tries to guess it. The program provides feedback on whether the guess is too high or too low, encouraging the player to keep trying until they get it right.

## Code

A randomly generated number to guess.
Feedback on whether the player's guess is too high or too low.
A congratulatory message when the correct number is guessed.

```Python
import random

def guess(x):
    random_number = random.randint(1, x)
    guess = 0
    while guess != random_number:
        guess = int(input(f'Guess a number between 1 and {x}: '))
        if guess < random_number:
            print('Sorry, guess again. Too low.')
        elif guess > random_number:
            print('Sorry, guess again. Too high')

    print(f'Yay you have guess the number {random_number}')


guess(20)
```
## How to use

1. Run the program
   
Execute the script in your preferred Python environment.

2. Provide inputs
   
When prompted, enter your guess as an integer between 1 and the specified range (default is 20 in this code).

3. Receive feedback
   
If your guess is too high or too low, the program will inform you so you can adjust your next guess.

4. Win the game
   
The game ends when you correctly guess the random number. A success message will display the correct number.




## Example Output

If the random number is 15 and you guess as follows:
```Python
Guess a number between 1 and 20: 10  
Sorry, guess again. Too low.  
Guess a number between 1 and 20: 18  
Sorry, guess again. Too high.  
Guess a number between 1 and 20: 15  
Yay, you have guessed the number 15!  
```

## Requirments 

* Python
