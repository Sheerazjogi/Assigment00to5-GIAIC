Problem Statement:

Write a function that takes two numbers and finds the average between the two.

Solution:
python
Copy
def average(a: float, b: float):
    """
    Returns the number which is halfway between a and b.
    """
    sum = a + b
    return sum / 2

def main():
    # Example use cases for the average function
    avg_1 = average(0, 10)  # Average of 0 and 10
    avg_2 = average(8, 10)  # Average of 8 and 10
    
    final = average(avg_1, avg_2)  # Average of avg_1 and avg_2
    
    print("avg_1:", avg_1)
    print("avg_2:", avg_2)
    print("final:", final)

if __name__ == '__main__':
    main()