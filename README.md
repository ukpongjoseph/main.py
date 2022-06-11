# main.py
(Python program version of rock ,scissors,paper game)
def main():
   #creating rock,scissors,paper game. python version
    R = "rock"
    S = "scissors"
    P = "paper"
    pass
    #import random
    import random
    list1 = [R,P,S]
    #rock beats scissors,scissors beats paper,paper beats rock
    print("welcome to rock,scissors,paper game")
    user_choice = input("player,enter your choice\npick any of[rock,scissors,paper] : ")
    if user_choice in list1:
        print("welldone!!! your choice has been noted down")
    else:
        print("that's an invalid input,please try again later!!!")
        main()
    CPU_choice = random.choice(list1)
    print(CPU_choice)
    if user_choice==CPU_choice:
        print("it is a tie, No winner yet")
    elif user_choice=="paper" and CPU_choice=="rock":
        print("player win")
    elif user_choice=="scissors" and CPU_choice=="paper":
        print("player win")
    elif user_choice=="rock" and CPU_choice=="scissors":
        print("player win")
    elif user_choice=="rock" and CPU_choice=="paper":
        print("computer win")
    elif user_choice=="paper" and CPU_choice=="scissors":
        print("computer win")
    elif user_choice=="scissors" and CPU_choice=="rock":
        print("computer win")
        pass
    repeat = input("do you want to play again?")
    if repeat == "yes":
        print("loading....\nwelcome back")
        main()
    else:
        print("thanks for playing bye bye!!!")
        exit()
main()
