# Constants for time calculation
DAYS_PER_YEAR = 365
HOURS_PER_DAY = 24
MIN_PER_HOUR = 60
SEC_PER_MIN = 60

def main():
    # Calculating total seconds in a year
    total_seconds = DAYS_PER_YEAR * HOURS_PER_DAY * MIN_PER_HOUR * SEC_PER_MIN
    
    # Printing the result
    print("There are " + str(total_seconds) + " seconds in a year!")

# Ensuring the main() function runs when the script is executed
if _name_ == '_main_':
    main()