# Python-Game-Rock-Paper-Scissors-
 Let’s create a simple command-line Rock-Paper-Scissor game without using any external game libraries like PyGame. In this game, the user gets the first chance to pick the option between Rock, paper, and scissors. After the computer select from the remaining two choices(randomly), the winner is decided as per the rules.
import random
rock='''
   _______
---'   ____)  
      (_____)  
      (_____)  
      (____)
---.__(___)  
'''
paper='''
   _______
---'   ____)____  
          ______)  
          _______)  
         _______)
---.__________)  
'''
scissors='''
    _______
---'   ____)____  
          ______)  
       __________)  
      (____)
---.__(___)  
'''  
print("WELCOME GAMERS\nGET READY TO PLAY ROCK, PAPER & SCISSORS")
user_choice=int(input("**INSTRUCTIONS**\nPress 0 for Rock\nPress 1 for paper\nPress 2 for scissors\n\n\nlets get started\npress any given option\n"))

computers_choice=random.randint(0,2)

print(f"your choice is 👉 ")
if user_choice==0:
    print(rock)
elif user_choice==1:
    print(paper)
else:
    print(scissors)     

print(f"computers choice is 👉 ")
if computers_choice==0:
    print(rock)
elif computers_choice==1:
    print(paper)
else:
    print(scissors)     

if user_choice==0 and computers_choice==0:
    print(f"you both choose the same\n\n IT IS A TIE 🤔")
elif user_choice==0 and computers_choice==1:
    print("you choose Rock, computer chosse Paper\n\nYou Loose 🙊")
elif user_choice==0 and computers_choice==2:
    print("you choose Rock, computer choose Scissors\n\nYou Win 👌")
elif user_choice==1 and computers_choice==0:
    print("you choose Paper, computer choose Rock\n\nYou Win 👌")
elif user_choice==1 and computers_choice==1:
    print("you both choose Paper \n\nit is a Tie 🤔")
elif user_choice==1 and computers_choice==2:
    print("you choose Paper, computer choose Scissors\n\nYou loose 🙊")
elif user_choice==2 and computers_choice==0:
    print("you choose Scissors, computer choose Rock\n\nyou loose 🙊")
elif user_choice==2 and computers_choice==1:
    print("you choose Scissors, computer choose Paper\n\nyou win 👌")
elif user_choice==2 and computers_choice==2:
    print("you choose Sciccors\n\nTie 🤔")
