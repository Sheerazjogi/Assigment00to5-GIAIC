Problem Statement:
You need to implement the get_name() function that returns your name as a string. The main() function calls get_name(), retrieves the name, and prints a greeting.

Solution Code:

def get_name():
    return "Sophia"

def main():
    name = get_name()  # get_name() will return a string which we store in the 'name' variable here
    print("Howdy", name, "! 🤠")

if __name__ == '__main__':
    main()