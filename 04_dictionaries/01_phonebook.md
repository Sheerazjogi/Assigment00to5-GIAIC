Problem Breakdown:
Store Information: We'll create a dictionary where each key is a name, and the value is the phone number.

Print Phonebook: We'll print out the entire phonebook, showing names and their corresponding phone numbers.

Lookup Phone Numbers: We'll allow the user to search for a phone number by entering a name. If the name is not found, the program will inform the user.

Code Implementation:
python
Copy
def read_phone_numbers():
    """
    Ask the user for names/numbers to store in a phonebook (dictionary).
    Returns the phonebook.
    """
    phonebook = {}  # Create empty phonebook

    while True:
        name = input("Name: ")
        if name == "":  # If the name input is empty, break the loop
            break
        number = input("Number: ")
        phonebook[name] = number  # Store the name and number in the dictionary

    return phonebook


def print_phonebook(phonebook):
    """
    Prints out all the names/numbers in the phonebook.
    """
    for name in phonebook:
        print(str(name) + " -> " + str(phonebook[name]))  # Print each name and number


def lookup_numbers(phonebook):
    """
    Allow the user to lookup phone numbers in the phonebook
    by looking up the number associated with a name.
    """
    while True:
        name = input("Enter name to lookup: ")
        if name == "":  # If the user inputs an empty string, break the loop
            break
        if name not in phonebook:
            print(name + " is not in the phonebook")  # Name not found in the phonebook
        else:
            print(phonebook[name])  # Print the number associated with the name


def main():
    phonebook = read_phone_numbers()  # Collect names and numbers from the user
    print_phonebook(phonebook)  # Print the phonebook
    lookup_numbers(phonebook)  # Allow the user to lookup numbers


# Python boilerplate.
if __name__ == '__main__':
    main()