# hello-world
Initial Repository
#Write a programme where the computer randomly generates a number between 0 and 20. The user needs to guess what the number is. If the user guesses wrong, tell them their guess is either too high, or too low. This will get you started with the random library if you haven't already used it.

import random
program = random.randint(0, 20)
while True:
    player = (input("Enter your guess between 1 and 20! "))
    try :
      playerint = int(player)
    except :
      print ('Please enter a number between 1 and 20')
    if playerint > 20 :
      print('Your number is not between 1 and 20, try again')
    if playerint > program :
      print('Lower...')
    elif playerint < program :
      print('Higher...')
    elif playerint is program :
      print('Yay! You got it!')
      break
