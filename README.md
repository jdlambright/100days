# 100days
these are exercises for 100days bootcamp

import random

rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

print("Give me your best shot! Let's play ROCK PAPER SCISSORS!!!")

#users move
move= int(input("Type 0 for rock, 1 for paper, and 2 for scissors. What is your move? \n "))

if move == 0:
  print(rock)
elif move == 1:
  print(paper)
elif move == 2:
  print(scissors)
else:
  print("invalid response")
#computer move
rps = [rock, paper, scissors]
random = random.randint(0,2)

comp_move = rps[random]


print(comp_move)

#determine winner
if move == random:
  print("tie")
elif move >= 3:
  print("invalid response")
elif move == 0 and random== 2:
  print("You win")
elif move > random:
  print("You Win")
elif random== 0 and move == 2:
  print("you lose")
elif random > move:
  print("you lose")
