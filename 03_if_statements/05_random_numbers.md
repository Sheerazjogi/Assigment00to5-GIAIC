Problem Statement:
Write a program that prints 10 random numbers in the range from 1 to 100.

Here is an example run:

Copy
45 79 61 47 52 10 16 83 19 12
Each time you run the program, the numbers should be different.

Hint: Use the random.randint() function from the random module, which generates a random integer between the given range (inclusive).

Starter Code:
python
Copy
import random

N_NUMBERS: int = 10  # Number of random numbers to print
MIN_VALUE: int = 1    # Minimum possible value
MAX_VALUE: int = 100  # Maximum possible value

def main():
    print("Delete this line and write your code here! :)")

# This provided line is required at the end of
# Python file to call the main() function.
if __name__ == '__main__':
    main()

    import random

N_NUMBERS: int = 10  # Number of random numbers to print
MIN_VALUE: int = 1    # Minimum possible value
MAX_VALUE: int = 100  # Maximum possible value

def main():
    # Generate 10 random numbers in the range 1 to 100 and store them in a list
    random_numbers = [random.randint(MIN_VALUE, MAX_VALUE) for _ in range(N_NUMBERS)]
    
    # Print the numbers, space-separated
    print(" ".join(map(str, random_numbers)))  # Convert each number to string and join them with spaces

if __name__ == '__main__':
    main()
