Problem Breakdown:
In this program, we need to keep track of how many fruits a user wants to buy, calculate the total cost, and then display that total. We'll loop through a dictionary that stores the price for each type of fruit, ask the user how many of each fruit they want, and then calculate the total cost.

Code Explanation:
Dictionary of fruits and their prices:

We define a dictionary fruits where the keys are the names of the fruits, and the values are their prices.

Looping through the dictionary:

We loop through each fruit in the dictionary.

For each fruit, we ask the user how many of that fruit they want to buy.

Calculating the total cost:

For each fruit, we multiply the price of the fruit by the quantity the user wants to buy.

We accumulate this value into the variable total_cost.

Displaying the total cost:

After processing all fruits, we print the total cost formatted as a dollar amount.

Solution Code:
python
Copy
def main():
    # Dictionary of fruits and their prices
    fruits = {'apple': 1.5, 'durian': 50, 'jackfruit': 80, 'kiwi': 1, 'rambutan': 1.5, 'mango': 5}
    
    total_cost = 0  # Initialize the total cost to 0
    
    # Loop through each fruit and ask how many the user wants to buy
    for fruit_name in fruits:
        price = fruits[fruit_name]  # Get the price of the current fruit
        # Ask user for the quantity they want to buy and convert it to an integer
        amount_bought = int(input(f"How many ({fruit_name}) do you want to buy?: "))
        # Add the cost of the purchased fruits to the total cost
        total_cost += price * amount_bought
    
    # Print out the total cost
    print(f"Your total is ${total_cost:.2f}")  # Format total to 2 decimal places


# Python boilerplate
if __name__ == '__main__':
    main()