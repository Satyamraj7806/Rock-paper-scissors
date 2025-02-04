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

       
![image](https://github.com/user-attachments/assets/bbfe6850-3e43-4b36-aefd-e4eacb3b0931)
![image](https://github.com/user-attachments/assets/22d4c3d1-fbaf-43c3-9ce0-32ab95fa94dd)
![image](https://github.com/user-attachments/assets/2119657e-93b4-4873-934e-410e84262bf7)


