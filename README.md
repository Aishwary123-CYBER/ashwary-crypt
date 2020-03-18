# ashwary-crypt
# code for making computer generated numner equals to our number
import random
choice = int(input("enter the input"))
computer_gen = random.randrange(1,10)
attempts = 0
while choice != computer_gen:
    str2 = input("enter high or low")
    if str2 == 'high':
        computer_gen+=1
        attempts +=1
        print(computer_gen)
    if str2 == 'low':
        computer_gen-=1
        attempts +=1
        print(computer_gen)
    if computer_gen == choice:
        attempts +=1
        print("it was fun and same you won in",attempts,"attempts")


