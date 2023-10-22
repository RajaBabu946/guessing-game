# guessing-game
import random  # Import the random module to generate random numbers

# Generate a random number between 1 and 1000 and store it in the 'jackpot' variable
jackpot = random.randint(1, 1000)

# Initialize the 'guess' variable by getting user input
guess = int(input(" guess "))

# Initialize a 'counter' variable to keep track of the number of attempts
counter = 1

# Start a loop that continues until the user's guess matches the 'jackpot'
while guess != jackpot:
    # Check if the guess is lower or higher than the jackpot and provide hints
    if guess < jackpot:
        print("Guess higher")
    else:
        print("Guess lower")
        
    # Get the next guess from the user and increment the 'counter'
    guess = int(input(" guess "))
    counter += 1

# If the loop exits, it means the user guessed the correct number
print("Correct answer")
print("You took", counter, "attempts")

