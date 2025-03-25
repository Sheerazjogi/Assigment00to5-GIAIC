"""
Program: Dice Simulator
----------------------
Simulates rolling two dice three times and prints
the results of each roll. Demonstrates variable scope.
"""

# Importing the random library for dice simulation
import random

# Number of sides on each die
NUM_SIDES = 6

def roll_dice():
    """
    Simulates rolling two dice and prints their total
    """
    die1 = random.randint(1, NUM_SIDES)  # First die roll
    die2 = random.randint(1, NUM_SIDES)  # Second die roll
    total = die1 + die2  # Sum of both dice
    print("Total of two dice:", total)  # Printing the result

def main():
    die1 = 10  # Local variable in main()
    print("die1 in main() starts as: " + str(die1))  # Printing initial value of die1 in main()
    
    # Rolling the dice three times
    roll_dice()
    roll_dice()
    roll_dice()
    
    print("die1 in main() is: " + str(die1))  # Printing value of die1 in main() after function calls

# Ensuring the main() function runs when the script is executed
if _name_ == '_main_':
    main()