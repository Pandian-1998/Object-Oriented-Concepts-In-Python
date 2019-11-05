import sys
class Customer:
    '''customer class with bank operations'''
    bankname="DURGABANK"
    def __init__(self,name,balance=0.0):
        self.name=name
        self.balance=balance

    def deposit(self,amount):
        self.balance=self.balance+amount
        print("The amount after deposit is",self.balance)

    def withdraw(self,amount):
        if amount > self.balance:
            print("Entered amount for withdrawl is not in your account")
            # c.Exit()
            sys.exit()
        else:
            self.balance=self.balance-amount
            print("The amount after withdrawl is",self.balance)

print("welcome to",Customer.bankname)
name=input("Enter your name:")
c=Customer(name)
while(True):
    print("d-Deposit\nw-Withdraw\ne-Exit\n")
    option=str(input("Choose your option:")).lower()
    if option == 'd':
        amount=float(input("enter the amount to deposit:"))
        c.deposit(amount)
    elif option=='w':
        amount=float(input("enter the amount to withdraw:"))
        c.withdraw(amount)
    elif option=='e':
        # c.Exit()
        print("Thanks for banking")
        sys.exit()
    else:
        print("you have choosen the Invalid option")
        print("Please choose the valid option")
    
    #break
