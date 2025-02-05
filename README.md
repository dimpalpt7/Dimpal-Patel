# Dimpal-Patel
@Roll the Dice
import random

def roll_dice():
    return random.randint(1, 6)

def dice_game():
    print("Welcome to the Dice Rolling Game!")
    while True:
        input("Press Enter to roll the dice...")  # Wait for the user to press Enter
        roll = roll_dice()  # Roll the dice
        print(f"You rolled a {roll}!")

        play_again = input("Do you want to roll again? (y/n): ").lower()
        if play_again != 'y':
            print("Thanks for playing! Goodbye!")
            break

# Run the game
dice_game()
