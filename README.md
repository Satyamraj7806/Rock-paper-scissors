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
             computer = random.choice(choices)
        print(f"Computer chose: {computer}")        
        if player_pick == computer:
            print("It's a tie!")
        elif (player_pick == "rock" and computer == "scissors") or \
             (player_pick == "paper" and computer == "rock") or \
             (player_pick == "scissors" and computer == "paper"):
            print("You won!")
        else:
            print("You lose!")

if __name__ == "__main__":
    rock_paper_scissors()

       
