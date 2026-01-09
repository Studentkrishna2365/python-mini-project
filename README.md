# python-mini-project
menu = {
    'pasta':50,
    'pizza':100,
    'coffe': 70,
    'burger':60,
    'salad':50, 
}
print("Welcome to python Restaurant !")

print('pasta:Rs50\npizza:Rs100\ncoffe:Rs70\nburger:Rs60\nsalad:Rs50')
total_Order = 0
item_1 = input("enter your first item of our menu :")
if item_1 in menu:

    total_Order += menu[item_1]
    print(f"your item {item_1} has been orederd")
else:
    print(f"your oreder {item_1} has benn not in our restaurant")

another_order = input("enter your another item (yes/no)?")
if another_order == "yes":
    item_2 = input("enter your second order ")
    if item_2 in menu :
        total_Order += menu[item_2]
    print(f"item 2 is {item_2} has been added")
else:
    print("order is {item_2} has been not available") 
print(f"total amount of order to item pay {total_Order}Rs")

