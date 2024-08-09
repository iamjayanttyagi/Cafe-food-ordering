# Cafe-food-ordering
So i just created a cafe menu ordering program using python, which takes input with different conditions from user and gives output as per their conditons entered.

# cafe menu My first silly mini project
menu = {
    "Mango Shake": 50, 
    "Burger": 100,
    "Pasta": 60,
    "Pizza": 99
}

print ("Hello, welcome to our cafe\n""These are the iteams we have: ")
print("Mango Shake: Rs50\nBurger: Rs100\nPasta:Rs60\nPizza: Rs99\nChoose any food item from the menu")
       
totalorder = 0  

order1 = input("Kindly enter your order from the list: ")
if order1 in menu:
    totalorder += menu[order1]
    print(f"your order {order1} has been placed")
    print(f"your total amount to be paid is {totalorder}")    
else:
    print(f"please order something else, {order1} is not available in our cafe")

totalorder2 = 0
order2 = input("would you like to add something else?(Yes/No): ")    
if order2 == "Yes":
    order2 = (input("enter another food iteam: "))

if order2 in menu:
    totalorder2 += menu[order2] + totalorder
    print(f"your updated bill of your order is: {totalorder2}")

elif order2 == "No": 
    print("Thankyou for visiting")
else:
    print(f"The iteam {order2} is not available in our cafe")






    
