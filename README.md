# User_To_Count_Comparisson
# Python WHILE Loop - Compare User Input To Count Variable Lab

'''
Coding Challenge:
WHILE Loop - Compare User Input To Count Variable Lab

This Challenge is to write code that:
Asks the user for an integer number 0 to 9 as input
Validate it's an integer (Hint: use your TRY/EXCEPT code)
Prints out the user input.  
Then use a while loop with a count variable, and loop from 0 to 10, and check when the user input variable matches the count variable.
When the user variable and the count variable are equal, print "The User variable is equal to the count variable. User = <the user variable value> Count variable = <the count variable>" 

Expected Output: If the user variable input was "6"
    Starting Code Challenge
    6
    Starting While Loop - Comparing User & Count Variable
    0
    1
    2
    3
    4
    5
    The User variable is equal to the count variable. 
    User = 6 
    Count = 6
    7
    8
    9
    Starting While Loop
    End Code Challenge
'''

# Your Code Starts Here:

def main():
    print("Starting Code Challenge")

    # Ask user for an integer between 0 and 9
    while True:
        try:
            user_input = int(input("Enter an integer between 0 and 9: "))
            if 0 <= user_input <= 9:
                break  # Exit loop once we get valid input
            else:
                print("Please enter an integer between 0 and 9.")
        except ValueError:
            print("That's not a valid integer. Please enter a number.")

    # Print the user input
    print(f"User input: {user_input}")

    # Initialize the count variable and start the while loop
    print("Starting While Loop - Comparing User & Count Variable")
    count = 0

    # Start looping from 0 to 9
    while count < 10:
        print(count)
        if count == user_input:
            print(f"The User variable is equal to the count variable. User = {user_input} Count = {count}")
        count += 1

    print("Ending While Loop")
    print("Ending Code Challenge")

main()
