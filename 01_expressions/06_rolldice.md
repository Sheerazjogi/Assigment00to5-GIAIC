"""
Simulate rolling two dice and print results of each
roll as well as the total.
"""
import random  # Importing the random module to simulate dice rolls

# Defining the number of sides on each die
NUM_SIDES = 6

def main():
    # Simulating dice rolls
    die1 = random.randint(1, NUM_SIDES)  # Rolling first die
    die2 = random.randint(1, NUM_SIDES)  # Rolling second die

    # Calculating the total
    total = die1 + die2  

    # Printing the results
    print("Dice have", NUM_SIDES, "sides each.")
    print("First die:", die1)
    print("Second die:", die2)
    print("Total of two dice:", total)

# Ensuring the main() function runs when the script is executed
if _name_ == '_main_':
    main()