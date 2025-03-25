"""
Program: Pythagorean Theorem Calculator
----------------------------------------
This program calculates the hypotenuse (BC) of a right triangle
using the Pythagorean theorem: BC^2 = AB^2 + AC^2
"""

# Importing math library to use sqrt function
import math  

def main():
    # Taking input for the two perpendicular sides
    ab = float(input("Enter the length of AB: "))
    ac = float(input("Enter the length of AC: "))

    # Calculating the hypotenuse using Pythagorean theorem
    bc = math.sqrt(ab*2 + ac*2)

    # Displaying the result
    print("The length of BC (the hypotenuse) is: " + str(bc))

# Ensuring the main() function runs when the script is executed
if _name_ == '_main_':
    main()