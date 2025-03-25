Problem Statement:
Write a function print_multiple(message, repeats) which takes two parameters:

message (a string to print),

repeats (an integer indicating how many times the message should be printed).

Solution Code:
python
Copy
def print_multiple(message: str, repeats: int):
    # Loop through the number of repeats and print the message each time
    for i in range(repeats):
        print(message)

def main():
    # Get user input for the message
    message = input("Please type a message: ")
    # Get user input for the number of times to repeat the message
    repeats = int(input("Enter a number of times to repeat your message: "))
    
    # Call the function to print the message the specified number of times
    print_multiple(message, repeats)

# The following line is required to run the main function when this file is executed directly
if __name__ == '__main__':
    main()