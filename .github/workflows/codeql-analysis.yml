#imports
import random, os, time
print()
os.system('clear')

def clear():
  os.system('clear')

#variables
guess_count = 7
Instr=("Type one of the letters from each of the hidden words each round.\n\n\n\n")
wordlist = ('deckthehalls', 'joy', 'christmasspirit', 'christmasdecoration', 'ornaments', 'christmastablecloth', 'santa', 'thanksgiving', 'tablecloth', 'thanksgivingfoods', 'turkey', 'cranberry', 'potatosalad', 'summerholidays')
answer = random.choice(wordlist)
life = 7
chosen_letters = []
game_over = False

#functions
def display_blanks():
  display_txt = ""                    

  for letter in answer:
    if letter in chosen_letters:
      display_txt += letter + " "
    else:
      display_txt += "_ "
  return display_txt + "\n"

def hangmanthing():
      if life == 6:
          print("""____________
|          |
|          |
|          0
|         
|         
|
|\n""",end="")
      elif life == 5:
        print("""____________
|          |
|          |
|          0
|          |
|         
|
|\n""",end="")
      elif life == 4:
        print("""____________
|          |
|          |
|          0
|         /|
|         
|
|\n""",end="")
      elif life == 3:
        print("""____________
|          |
|          |
|          0
|         /|\\
|         
|
|\n""",end="")
      elif life == 2:
        print("""____________
|          |
|          |
|          0
|         /|\\
|         /
|
|\n""",end="")
      elif life == 1:
        print("""____________
|          |
|          |
|          0
|         /|\\
|         / \\
|
|\n""",end="")

      elif life == 7:
        print("""____________
|          |
|          |
|          
|         
|         
|
|\n""", end="")
      else:
        pass

print("""____________
|          |
|          |
|          
|         
|         
|
|\n""", end="")

print()
print("_ " * len(answer))


while life > 0 and game_over == False:
  print()
  print("Guesses left: ", life)
  input_letter = input("Please enter a letter: ")
  time.sleep(1)
  os.system('clear')

  if input_letter in chosen_letters:
    hangmanthing()
    print("You have entered these letter before: " + str(chosen_letters) + "\n")

  elif input_letter in answer: 
    chosen_letters.append(input_letter)
    print()
    output_text = display_blanks()
    hangmanthing()


    if "_" in output_text:
      print(output_text)

    else:
      game_over = True

  else:
    life -= 1
    hangmanthing() 
    chosen_letters.append(input_letter) 
    print()
    print(display_blanks())

print("""
____________
|          |
|          |
|          0
|         /|\\
|         / \\
|    ROBLOX GUY COMMITS SUICIDE!
|\n""",end="")
print("\n\n")
print("Game over!")
print("Answer:", answer)
