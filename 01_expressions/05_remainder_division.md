"""
Program: Division Calculator
----------------------------
This program asks the user for two numbers and then prints
the quotient (result of division) and remainder.
"""

def main():
    # Taking input for the two numbers
    dividend = int(input("Please enter an integer to be divided: "))
    divisor = int(input("Please enter an integer to divide by: "))

    # Calculating quotient and remainder
    quotient = dividend // divisor  # Integer division (no decimal)
    remainder = dividend % divisor  # Modulus (gives remainder)

    # Displaying the result
    print("The result of this division is " + str(quotient) + " with a remainder of " + str(remainder))

# Ensuring the main() function runs when the script is executed
if _name_ == '_main_':
    main()