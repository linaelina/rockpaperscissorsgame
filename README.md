import random
turns = ['rock', 'scissors', 'paper']
human_turns = []
computer_turns = []

while(True):
    human_turn = input ('Enter jour turn: ')
    computer_turn = random.choice(turns)
    
    human_turns.append(human_turn)
    computer_turns.append(computer_turn)



    if human_turn == computer_turn:
     print('Draw!')
    elif human_turn == 'rock' and computer_turn == 'scissors':
     print('Human wins!')
    elif human_turn == 'paper' and computer_turn == 'rock':
     print('Human wins!')
    elif human_turn == 'scissors' and computer_turn == 'paper':
     print('Human wins!')
    else:
     print('Computer wins!')
print('You have played {len(human_turn)} times')
print(human_turn)
print(computer_turn)
