"""
Program: add2numbers
--------------------
This program prompts the user to enter two integers,
calculates their sum, and prints the result.
"""

def main():
    # Display the purpose of the program
    print("This program adds two numbers.")
    
    # Prompt the user to enter the first number and convert it to an integer
    num1 = int(input("Enter first number: "))
    
    # Prompt the user to enter the second number and convert it to an integer
    num2 = int(input("Enter second number: "))
    
    # Calculate the sum of the two numbers
    total = num1 + num2
    
    # Print the result with a message
    print("The total is " + str(total) + ".")

# This line ensures the main() function is executed when the script runs
if _name_ == '_main_':
    main()