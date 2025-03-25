Problem Breakdown:
In this problem, we want to create a "Guess My Number" game where the computer selects a secret number between 0 and 99, and the user is tasked with guessing it. After each guess, the program will provide feedback if the guess was too high or too low until the user guesses the correct number.

Key Concepts:
Random Number Generation: We'll use Python's random.randint(1, 99) to generate a secret number between 1 and 99.

User Input and Comparison: The program will continuously prompt the user for a guess and compare it to the secret number. Based on whether the guess is higher or lower than the secret number, it will give appropriate feedback.

Looping: The program should keep prompting the user for guesses until they correctly guess the number. We'll use a while loop to continue asking for input until the guess is correct.

Code Explanation:
Generate the Secret Number: The random.randint(1, 99) generates a random number between 1 and 99, which will be the secret number.

User Guess Loop: We prompt the user for a guess using input(), convert it to an integer, and then enter a loop to keep comparing the guess to the secret number. If the guess is too low, we print "Your guess is too low", and if it’s too high, we print "Your guess is too high". The loop continues until the user guesses correctly.

Exit Condition: Once the user guesses the correct number, the program prints "Congrats! The number was: ", and the game ends.

Solution Code:
python
Copy
import random

def main():
    # Generate the secret number at random!
    secret_number = random.randint(1, 99)
    
    print("I am thinking of a number between 1 and 99...")
    
    # Get the user's first guess
    guess = int(input("Enter a guess: "))
    
    # Loop until the guess is correct
    while guess != secret_number:
        if guess < secret_number:
            print("Your guess is too low")
        else:
            print("Your guess is too high")
        
        print()  # Print a blank line for cleaner output
        guess = int(input("Enter a new guess: "))  # Get a new guess from the user
    
    # Congratulate the user once they guess the correct number
    print("Congrats! The number was: " + str(secret_number))
    
# Python boilerplate to ensure the main() function is called
if __name__ == '__main__':
    main()