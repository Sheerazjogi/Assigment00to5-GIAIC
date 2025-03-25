"""
Program: Triangle Perimeter Calculator
--------------------------------------
This program prompts the user for three side lengths of a triangle,
calculates the perimeter, and prints the result.
"""

def main():
    # Prompt the user for the three side lengths
    side1 = float(input("What is the length of side 1? "))
    side2 = float(input("What is the length of side 2? "))
    side3 = float(input("What is the length of side 3? "))

    # Calculate the perimeter
    perimeter = side1 + side2 + side3

    # Print the perimeter of the triangle
    print("The perimeter of the triangle is " + str(perimeter))

# This ensures the main() function runs when the script is executed
if _name_ == '_main_':
    main()