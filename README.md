# pythonproject
python mini projects
1. Grading System 
n=float(input('Enter your percentage : ')) if 
n>100 or n<0: 
 print('Invalid input from user.') 
elif n>85: 
 print('GRADE:A+') 
elif n>=65 or n<=85: 
print('GRADE:A') 
elif n>=45 or n<65: 
print('GRADE:B') 
elif n>=25 or n<45: 
print('GRADE:C') 
else: 
 print('GRADE:D') 
Output: 
2.Prin ng Numbers: # Prin ng according to user ch=input('Press F for 
forward prin ng or Press B for backward prin ng : ') if ch=='F': 
 st=int(input('Enter star ng point : ')) end=int(input('Enter ending 
point : ')) upd=int(input('Enter upda on : ')) ch1=input('Press R
for row prin ng or Press C for column prin ng:') 
 if ch1=='R': if st<=end: 
for i in range(st,end+1,upd): 
 print(i,end=' ') 
else: 
 print('Invalid star ng and ending point.') 
elif ch1=='C': if st<=end: for i in 
range(st,end+1,upd): 
 print(i) 
else: 
 print('Invalid star ng and ending point.') 
else: 
 print('Invalid choice.') 
elif ch=='B': 
 st=int(input('Enter star ng point : ')) end=int(input('Enter ending 
point : ')) upd=int(input('Enter upda on : ')) ch2=input('Press R 
for row prin ng or Press C for column prin ng:') 
 if ch2=='R': if st>=end: 
for i in range(st,end-1,-upd): 
 print(i,end=' ') 
else: 
 print('Invalid input(s).') 
elif ch2=='C': if st>=end: 
for i in range(st,end-1,-upd): 
 print(i) 
else: 
 print('Invalid 
input(s).') else: 
print('Invalid choice') 
 
else: 
 print('Enter either F or B. Thank you.') 
Output: 

3.Vo ng Age System 
#VOTING SYSTEM 
age=int(input('Enter age of the voter : ')) 
if age>=18 and age<=100: 
print('Welcome, you are eligible for vo ng.') 
ask=int(input('Enter Aadhar number to con nue : ')) 
print('Press : 1 for BJP ; 2 for INC ; 3 for AAP ; 4 for BSP ; 5 for RJD') 
ch=input('Enter your decision : ') 
ch=int(ch) if ch==1: 
print('You voted for BJP.Thank you.') elif 
ch==2: 
print('You voted for INC.Thank you.') 
elif ch==3: 
print('You voted for AAP.Thank 
you.') elif ch==4: 
print('You voted for BSP.Thank you.') 
elif ch==5: 
print('You voted for RJD.Thank you.') 
else: 
print('Invalid Choice.') 
else: print('YOU CANNOT 
VOTE.') 
Output: 
4. Inventory 
# inventory dic onary 
inventory = {} 
def addproduct(item,quan ty): 
 if item in inventory: 
 inventory[item] += quan ty 
 else: 
 inventory[item] = quan ty def 
removeproduct(item, quan ty): 
 if item in inventory: 
 if inventory[item] >= quan ty: 
inventory[item] -= quan ty 
if inventory[item] == 0: 
del inventory[item] 
 else: print(f"Not enough {item} 
in stock.") else: 
 print(f"{item} not found in inventory.") 
def totalitems(): 
 print("Items in Inventory:") 
 for item, quan ty in inventory.items(): 
 print(f"{item}: {quan ty}") 
addproduct("Apples", 10) 
addproduct("Bananas", 15) 
addproduct("Oranges", 20) 
removeproduct("Bananas", 5) 
totalitems() Output: 
5. Vowel Coun ng 
s=input() 
count=0 
s=s.lower() a=s.strip() for x in a: if x=='a' or 
x=='e' or x=='i' or x=='o' or x=='u': 
 count+=1 
print('No of Vowels = %d'%(count)) 
Output: 
6. Guess a number import random def guessing_num(): 
num = random.randint(1, 100) a empts = 0 
print("Welcome to the Number Guessing Game!") 
print("Computer has chosen a number. Can you guess it?") 
 while True: 
 guess = int(input("Enter your guess: 
")) a empts += 1 if guess < num: 
 print("Too low.Try again.") 
elif guess > num: 
 print("Too high.Try again.") 
 else: 
 print("Congratula ons! You've guessed the number %d in %d 
a empts!"%(num,a empts)) 
 break 
guessing_num() 
Output: 
7. Rock Paper Scissors 
import random 
def get_user_choice(): 
while True: 
 user_choice = input("Enter your choice (rock, paper, scissors): 
").lower() if user_choice in ['rock', 'paper', 'scissors']: 
 return user_choice 
 else: 
 print("Invalid choice. Please enter rock, paper, or scissors.") 
def get_computer_choice(): 
 return random.choice(['rock', 'paper', 'scissors']) 
def determine_winner(user_choice, computer_choice): 
if user_choice == computer_choice: 
 return "It's a e!" elif (user_choice == 'rock' and 
computer_choice == 'scissors') or \
 (user_choice == 'paper' and computer_choice == 'rock') or \
 (user_choice == 'scissors' and computer_choice == 'paper'): 
 return "You win!" 
 else: 
 return "Computer wins!" 
def play_game(): 
 user_choice = get_user_choice() computer_choice = 
get_computer_choice() print("You chose:", user_choice) 
print("Computer chose:", computer_choice) 
print(determine_winner(user_choice, computer_choice)) 
play_game() 
Output: 
8. Dice Roller 
import random 
def roll_a_dice(): return 
random.randint(1, 6) result = 
roll_a_dice() print("You 
rolled a", result) Output: 
9. Calculator 
# Simple calculator 
def add(x, y): 
return x + y def 
subtract(x, y): 
return x - y 
def mul ply(x, y): 
return x * y def 
divide(x, y): if y 
== 0: return 
"Error" else: 
 return x / y 
print("Choose opera on : ") 
print("1. Add") print("2. 
Subtract") print("3. Mul 
ply") print("4. Divide") 
while True: 
 ch = input("Enter choice(1/2/3/4): ") 
 if ch in ('1', '2', '3', '4'): 
 num1 = float(input("Enter first number: ")) 
num2 = float(input("Enter second number: ")) 
 if ch == '1': print(f"The result is 
{add(num1, num2)}") 
 elif ch == '2': print(f"The result is 
{subtract(num1, num2)}") 
 elif ch == '3': print(f"The result is {mul 
ply(num1, num2)}") 
 elif ch == '4': 
 print(f"The result is {divide(num1, num2)}") 
 nex = input(" Next calcula on ? (yes/no): ") 
 if nex!= 'yes': 
 break 
 else: 
 print("Invalid Input") 
Output:
