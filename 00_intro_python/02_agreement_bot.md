"""
Program: Favorite Animal
------------------------
This program asks the user for their favorite animal
and responds with the same favorite animal.
"""

def main():
    # Asking the user for their favorite animal
    favorite_animal = input("What's your favorite animal? ")

    # Printing the response with the user's input
    print("My favorite animal is also " + favorite_animal + "!")

# This line ensures the main() function runs when the script is executed
if _name_ == '_main_':
    main()