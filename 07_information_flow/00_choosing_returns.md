
Problem Statement:
There are times where we want to return different things from a function based on some condition. To practice this idea, imagine that we want to check if someone is an adult. We might check their age and return different things depending on how old they are!

We are provided with the ADULT_AGE variable which has the age a person is legally classified as an adult (in the United States).

You need to complete the function is_adult(age) which:

Returns True if the provided age is greater than or equal to ADULT_AGE (18 in this case).

Returns False if the age is less than ADULT_AGE.

Starter Code:
def main():

# This provided line is required at the end of
# Python file to call the main() function.
if __name__ == '__main__':
    main()
Solution:
python
Copy
ADULT_AGE : int = 18  # U.S. legal age for adulthood

def is_adult(age: int):
    if age >= ADULT_AGE:
        return True
    return False

########## No need to edit code beyond this point :) ##########

def main():
    age = int(input("How old is this person?: "))
    print(is_adult(age))

if __name__ == "__main__":
    main()