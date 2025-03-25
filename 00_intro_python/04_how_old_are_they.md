"""
Program: Age Calculation
------------------------
This program calculates the ages of five friends based on given conditions
and prints their names with their respective ages.
"""

def main():
    # Storing each person's age based on given conditions
    anton = 21  # Anton's age
    beth = anton + 6  # Beth is 6 years older than Anton
    chen = beth + 20  # Chen is 20 years older than Beth
    drew = chen + anton  # Drew's age is Chen's age plus Anton's age
    ethan = chen  # Ethan is the same age as Chen

    # Printing the calculated ages
    print("Anton is " + str(anton))
    print("Beth is " + str(beth))
    print("Chen is " + str(chen))
    print("Drew is " + str(drew))
    print("Ethan is " + str(ethan))

# This line ensures the main() function runs when the script is executed
if _name_ == '_main_':
    main()