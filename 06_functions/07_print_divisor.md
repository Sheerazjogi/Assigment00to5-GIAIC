Problem Statement:
Write a helper function print_divisors(num) that takes in a number and prints all of its divisors (all the numbers from 1 to num inclusive that num can be cleanly divided by).

Solution Code:
def print_divisors(num: int):
    # Print the header message
    print("Here are the divisors of", num)
    # Loop through all numbers from 1 to num
    for i in range(1, num + 1):  # Start from 1 and go up to num inclusive
        if num % i == 0:  # If there is no remainder when num is divided by i
            print(i)  # Print i as it is a divisor of num

def main():
    # Ask the user to input a number
    num = int(input("Enter a number: "))
    # Call the print_divisors function to print the divisors of the number
    print_divisors(num)

# This is required to execute the main() function when the script is run directly
if __name__ == '__main__':
    main()