Problem Statement:
You need to implement the chaotic_counting() function which prints numbers from 1 to 10. However, before printing each number, you should call a done() function, which will return True with a certain probability (DONE_LIKELIHOOD). If done() returns True, you stop counting and exit the function. If done() never returns True, it will count up to 10.


Solution:
import random

# You can adjust the probability here for when the counting should stop
DONE_LIKELIHOOD = 0.3

def chaotic_counting():
    for i in range(10):
        curr_num = i + 1
        if done():
            return # If done() returns True, exit the function
        print(curr_num)

def done():
    """ Returns True with a probability of DONE_LIKELIHOOD """
    if random.random() < DONE_LIKELIHOOD:
        return True
    return False

def main():
    print("I'm going to count until 10 or until I feel like stopping, whichever comes first.")
    chaotic_counting()
    print("I'm done")

if __name__ == "__main__":
    main()