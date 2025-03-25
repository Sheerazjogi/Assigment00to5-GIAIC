Problem Statement:
We need to implement the function in_range(n, low, high) which takes in three integers as parameters and returns True if the number n is between low and high (inclusive). high is guaranteed to be greater than low.

Starter Code
def main():

# This provided line is required at the end of
# Python file to call the main() function.
if __name__ == '__main__':
    main()
Solution:
def in_range(n, low, high):
    """
    Returns True if n is between low and high, inclusive. 
    high is guaranteed to be greater than low.
    """
    if low <= n <= high:
        return True
    return False

def main():
    # Example test cases
    print(in_range(5, 1, 10))  # Expected: True
    print(in_range(0, 1, 10))  # Expected: False
    print(in_range(10, 1, 10))  # Expected: True

if __name__ == '__main__':
    main()