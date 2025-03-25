Problem Statement:
We have written a helper function for you called greet(name) which takes as input a string name and prints a greeting. You need to write some code in the main() function to get the user's name and then greet them, ensuring that you call the greet(name) helper function.


Starter Code:
def main():

# This provided line is required at the end of
# Python file to call the main() function.
if __name__ == '__main__':
    main()
Solution:
def greet(name):
    return "Greetings " + name + "!"

def main():
    name = input("What's your name? ")  # Get the user's name
    print(greet(name))  # Greet the user using the greet() function

if __name__ == '__main__':
    main()