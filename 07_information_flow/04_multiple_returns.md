Problem Statement
There are times where you are working with lots of different data within a function that you want to return. While generally, we want to keep functions to have a precise purpose, sometimes that purpose just deals with multiple bits of data.

To practice this, imagine we are working on a program where the user needs to enters data to sign up for a website. Fill out the get_user_data() function which:

Asks the user for their first name and stores it in a variable

Asks the user for their last name and stores it in a variable

Asks the user for their email address and stores it in a variable

Returns all three of these pieces of data in the order it was asked

You can return multiple pieces of data by separating each piece with a comma in the return line.

Here is an example run of the program:

What is your first name?: sheeraz

What is your last name?: ahmed

What is your email address?: sheerazahmedjogi@gmail.com

Received the following user data: ('sheeraz', 'ahmed', 'sheerazahmedjogi@gmail.com')

(Note. This idea is called tuple packing/unpacking. We "pack" our return values into a single data structure called a tuple. We can then "unpack" these values back into our original values or leave them as a tuple.)

Starter Code:
def main():
    print("Delete this line and write your code here! :)")

# This provided line is required at the end of
# Python file to call the main() function.
if __name__ == '__main__':
    main()

    Solution:
def get_user_info():
    # Ask the user for their first name, last name, and email address
    first_name = input("What is your first name?: ")
    last_name = input("What is your last name?: ")
    email_address = input("What is your email address?: ")
    
    # Return all three pieces of information as a tuple
    return first_name, last_name, email_address

########## No need to edit code past this point :) ##########

def main():
    # Call get_user_info() to get the user's data
    user_data = get_user_info()
    
    # Print out the received user data
    print("Received the following user data:", user_data)

if __name__ == "__main__":
     main()