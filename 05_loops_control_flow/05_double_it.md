Problem Statement:

Write a program that asks a user to enter a number. Your program will then double that number and print out the result. It will repeat that process until the value is 100 or greater.

For example, if the user enters the number 2 you would then print:

4 8 16 32 64 128
Note that:

2 doubled is 4

4 doubled is 8

8 doubled is 16

and so on.

We stop at 128 because that value is greater than 100.

Solution:

def main():
    curr_value = int(input("Enter a number: "))  # Ask the user to enter a number
    
    while curr_value < 100:  # Keep doubling the value until it's greater than or equal to 100
        curr_value = curr_value * 2  # Double the current value
        print(curr_value, end=" ")  # Print the doubled value followed by a space

if __name__ == '__main__':
    main()