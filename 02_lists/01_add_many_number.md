def sum_of_list(nums: list) -> int:
    """
    This function takes a list of numbers and returns their sum.
    """
    return sum(nums)  # Using Python's built-in sum() function

def main():
    numbers = [10, 20, 30, 40, 50]  # A different list of numbers
    result = sum_of_list(numbers)  # Calling our function
    print("The sum of the list is:", result)  # Displaying the sum

if _name_ == '_main_':
    main()