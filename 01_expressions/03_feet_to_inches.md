"""
Program: Feet to Inches Converter
---------------------------------
This program converts feet into inches using the
conversion factor: 1 foot = 12 inches.
"""

# Constant for conversion
INCHES_IN_FOOT = 12  # 1 foot = 12 inches

def main():
    # Asking the user for input in feet
    feet = float(input("Enter number of feet: "))

    # Converting feet to inches
    inches = feet * INCHES_IN_FOOT

    # Displaying the result
    print("That is", inches, "inches!")

# Ensuring the main() function runs when the script is executed
if _name_ == '_main_':
    main()