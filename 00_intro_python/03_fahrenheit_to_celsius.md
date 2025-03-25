"""
Program: Fahrenheit to Celsius Converter
----------------------------------------
This program prompts the user for a temperature in Fahrenheit
and converts it to Celsius using the given formula.
"""

def main():
    # Asking the user for temperature in Fahrenheit
    fahrenheit = float(input("Enter temperature in Fahrenheit: "))

    # Converting Fahrenheit to Celsius
    celsius = (fahrenheit - 32) * 5.0 / 9.0

    # Printing the result
    print("Temperature:", str(fahrenheit) + "F =", str(celsius) + "C")

# This line ensures the main() function runs when the script is executed
if _name_ == '_main_':
    main()