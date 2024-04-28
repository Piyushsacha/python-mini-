# python-mini-
1.calculator


import math
def sum():
    a=int(input("enter value of a:"))
    b=int(input("enter value of b:"))
    sum =a+b
    return sum
def sub():
    a=int(input("enter value of a:"))
    b=int(input("enter value of b:"))
    sub =a-b
    return sub
def mul():
    a=int(input("enter value of a:"))
    b=int(input("enter value of b:"))
    mul =a*b
    return mul
def div():
    a=int(input("enter value of a:"))
    b=int(input("enter value of b:"))
    div =a/b
    return div
def sqrt():
    a=int(input("enter value of a:"))
    sqrt =math.sqrt(a)
    return sqrt
def pow():
    a=int(input("enter value of a:"))
    b=int(input("enter value of b:"))
    pow =a**b
    return pow
def log():
    a=int(input("enter value of a:"))
    log =math.log(a)
    return log
def sin():
    a=int(input("enter the value of a:"))
    sin =math.sin(a)
    return sin
def cos():
    a=int(input("enter the value a:"))
    cos =math.cos(a)
    return cos
def tan():
    a=int(input("enter the value a:"))
    tan =math.tan(a)
    return tan
def exp():
    a=int(input("enter the value a:"))
    
    exp =math.exp(a)
    return exp
def fact():
    a=int(input("enter the value a:"))
    
    fact =math.factorial(a)
    return fact
def mod():
    a=int(input("enter the value a:"))
    b=int(input("enter the value b:"))
    mod =a%b
    return mod
def sqr():
    a=int(input("enter the value a:"))
    sqr =a**2
    return sqr
def cube():
    a=int(input("enter the value a:"))
    cube =a**3
    return cube

    
while True:
    choice=int(input("enter your choice 1->sum 2->sub 3->div 4->mul 5->sqrt 6->pow 7->pow 8->log 9->sin 10->cos 11->tan 12->exp 13->fact 14->mod 15->sqr 16->cube 17->exit:"))
    if choice==1:
       print(sum())
    elif choice==2:
       print(sub())
    elif choice==3:
        print(div())
    elif choice==4:
        print(mul())
    elif choice==5:
        print(sqrt())
    elif choice==6:
        print(pow())
    elif choice==7:
        print(log())
    elif choice==8:
        print(sin())
    elif choice==9:
        print(cos())
    elif choice==10:
        print(tan())
    elif choice==11:
        print(exp())
    elif choice==12:
        print(fact())
    elif choice==13:
        print(mod())
    elif choice==14:
        print(sqr())
    elif choice==15:
        print(cube())
    elif choice==16:
        break
    else:
        print("invalid choice")

2.grading system

nventory={}
while True:
    action= input("enter what want you to do? add, remove, display,quit:")
    if action=='add':
        item=input("enter item name:")
        quantity=int(input("enter your quantity:"))
        if item in inventory:
            inventory[item]+=quantity
        else:
            inventory[item]=quantity
    elif action=='remove':
        item=input("enter the name of item you want to remove:")
        quantity=int(input("enter the quantity you want to remove:"))
        if item in inventory and inventory[item]>=quantity:
            inventory[item]-=quantity
        elif item in inventory and inventory[item]<quantity:
            print(f"There are only {inventory[item]} left in {item} left in inventory.")
        else:
            print("ther is no item left in inventory.")
    
    elif action=='display':
        print("Inventory")
        for key,value in inventory.items():
            print(f"{key}:{value}")
    
    elif action =='quit':
        break
    else:
        print("invalid entry please try again")


3.inventory system

 

import random
    
num = random.randint(1, 10)
guess = None
    
while guess != num:
    guess = input("guess a number between 1 and 10: ")
    guess = int(guess)
    
    if guess == num:
        print("congratulations! you won!")
        print(guess)
        break
    else:
        print("nope, sorry. try again!")
print("Thank You :)")

4.number mission game
order1 = input("Enter your choice: ")
if order1 == "R":
    print("You have choose Reverse order.")
    s_p = int(input("Enter starting point: "))
    e_p = int(input("Enter ending point: "))
    print("r for Row order and c for Column order.")
    order2 = input("Enter your choice: ")
    if order2 == "r":
        print("You have choose Row order.")
        for x in range(s_p, e_p, -1):
            print(x, end = " ")
    elif order2 == "c":
        print("You have choose Column order.")
        for x in range(s_p, e_p, -1):
            print(x)
    else:
        print("You have choose Invalid choice.")
elif order1 == "F":
    print("You have choose Forward order.")
    s_p = int(input("Enter starting point: "))
    e_p = int(input("Enter ending point: "))
    print("r for Row order and c for Column order.")
    order2 = input("Enter your choice: ")
    if order2 == "r":
        print("You have choose Row order.")
        for x in range(s_p, e_p, 1):
            print(x, end = " ")
    elif order2 == "c":
        print("You have choose Column order.")
        for x in range(s_p, e_p, 1):
            print(x)
    else:
        print("You have choose Invalid choice.")
else:    
    print("You have choose Invalid choice.")
print("THANKYOU USER :)")

5. number system

name = input("Enter ur name: ")
mark1 = int(input("Enter ur 1st marks: "))
mark2 = int(input("Enter ur 2nd marks: "))
mark3 = int(input("Enter ur 3rd marks: "))
mark4 = int(input("Enter ur 4th marks: "))
mark5 = int(input("Enter ur 5th marks: "))
per = ((mark1+mark2+mark3+mark4+mark5)/5)
if (mark1, mark2, mark3, mark4, mark5 > 100):
    print("Invalid Marks.")
else:
    if 90<per<=100:
        print("A")
        print(per, "%")
    elif 80<per<=90:
        print("B")
        print(per, "%")
    elif 70<per<=80:
        print("C")
        print(per, "%")
    elif 60<per<=70:
        print("D")
        print(per, "%")
    elif 50<per<=60:
        print("E")
        print(per, "%")
    else:
        print("You fail.")
if per > 100:
    print("Invalid Percentage.")

6. readme

 

import random

def check(comp, user):
    if comp == user:
        return 0

    if(comp == 0 and user == 1):
        return -1

    if (comp == 1 and user == 2):
        return -1

    if (comp == 2 and user == 0):
        return -1

    return 1

comp = random.randint(0, 2)
user = int(input("0 for rock, 1 for paper and 2 for scissor:  \n"))

score = check(comp, user)

print("You: ", user)
print("Computer: ", comp)

if score == 0:
    print("It's Draw.")
elif score == -1:
    print("You Loose.")
else:
    print("You Won.")


7.rock paper scissor


 

import random
repeat = True
while repeat:
    print("You rolled",random.randint(1,6))
    print("Do you want to roll again? Y/N")
    repeat = "Y" in input()


8.roll the dice


  
 
# Function to cast a vote
def cast_vote(votes, candidate):
    if candidate in votes:
        votes[candidate] += 1
    else:
        print(f'Error: {candidate} is not a valid candidate')

# Function to tally the votes
def tally_votes(votes):
    total_votes = 0
    for candidate, count in votes.items():
        total_votes += count
        print(f'{candidate}: {count} votes')
    print(f'Total votes: {total_votes}')

# Get the candidates from the user
candidates = input('Enter the candidates (separated by commas): ').split(',')

# Create an empty dictionary to store the votes
votes = {}

# Add the candidates to the dictionary
for candidate in candidates:
    votes[candidate.strip()] = 0

# Cast some votes
cast_vote(votes, 'BJP')
cast_vote(votes, 'CNG')
cast_vote(votes, 'TMC')
cast_vote(votes, 'AAP')
cast_vote(votes, 'RJD')

# Tally the votes
tally_votes(votes)
