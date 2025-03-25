Problem Statement:

Write a program that prints out the calls for a spaceship that is about to launch. Countdown from 10 to 1 and then output Liftoff!

Here's a sample run of the program:

Copy
10 9 8 7 6 5 4 3 2 1 Liftoff!
Starter Code:

python
Copy
def main():
    print("Delete this line and write your code here! :)")

# This provided line is required at the end of
# Python file to call the main() function.
if __name__ == '__main__':
    main()
Solution:

python
Copy
def main():
    for i in range(10, 0, -1):  # Countdown from 10 to 1
        print(i, end=" ")  # Print the number without a newline
    print("Liftoff!")  # Print Liftoff!

if __name__ == '__main__':
    main()