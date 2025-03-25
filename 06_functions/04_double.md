Problem Statement:
You need to implement the double(num) function that takes a number, multiplies it by 2, and returns the result. The main() function asks the user for a number, calls double(num), and then prints the result.

Solution Code:
def double(num: int):
    return num * 2

def main():
    num = int(input("Enter a number: "))
    num_times_2 = double(num)
    print("Double that is", num_times_2)

if __name__ == '__main__':
    main()