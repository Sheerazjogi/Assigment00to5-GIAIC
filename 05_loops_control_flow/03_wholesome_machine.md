Problem Statement:
Write a program which prompts the user to type an affirmation of your choice (we'll use "I am capable of doing anything I put my mind to.") until they type it correctly.


AFFIRMATION = "I am capable of doing anything I put my mind to."

def main():
    # Ask the user to type the affirmation
    print("Please type the following affirmation: " + AFFIRMATION)

    # Get the user's input
    user_feedback = input()

    # Continue prompting the user until they type the correct affirmation
    while user_feedback != AFFIRMATION:
        print("That was not the affirmation.")
        print("Please type the following affirmation: " + AFFIRMATION)
        user_feedback = input()  # Get new input from the user

    print("That's right! :)")  # Print a success message when the user types it correctly


# Main execution
if __name__ == '__main__':
    main()