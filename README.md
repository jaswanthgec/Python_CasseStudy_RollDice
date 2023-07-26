# Python_CasseStudy_RollDice
we create a roll and dice game using a random module in Python

# Program:

import random

def roll():
    min_value = 1
    max_value = 6
    return random.randint(min_value, max_value)

def game():
    while True:
        print("Rolling the dice...")
        dice_value = roll()
        
        print("After rolling you get ", dice_value)
        
        roll_again = input("Do you want to roll the dice again? (yes/no): ")
        if roll_again.lower() not in ['yes', 'y']:
            print("Thanks for playing! Goodbye!")
            break
game()

# Output:

Rolling the dice...
After rolling you get  6
Do you want to roll the dice again? (yes/no): y
Rolling the dice...
After rolling you get  3
Do you want to roll the dice again? (yes/no): y
Rolling the dice...
After rolling you get  4
Do you want to roll the dice again? (yes/no): n
Thanks for playing! Goodbye!
