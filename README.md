# Rock-paper-scissors

import random

def rock_paper_scissors():
    print("Welcome to Rock, Paper, Scissors!")
    choices = ["rock", "paper", "scissors"]    
    while True:
        player_pick = input("Enter rock, paper, or scissors (or 'quit' to stop): ").lower()
        if player_pick == "quit":
            print("Thanks for playing!")
            break
        if player_pick not in choices:
            print("Invalid choice. Try again.")
            continue       
       
