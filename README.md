# My_Crazy_Restaurant
# My_Crazy_Restaurant is a foodie-based mini-project. Imagine you are a customer and feeling tired from your same day-to-day work. Recently you found a restaurant and want to eat something crazy then You are at the correct place. You can order anything you want just by writting the correct spell which is already provided you in your menu card..
# So Order your favourite dish now and ENJOY!!!


menu = {
  'mix Veg pizza': 100,
  'panner pizza': 80,
  'cheese pizza': 85,
  'panner cheese pizza': 120,
  'vegetable cheese burger': 90,
  'veg cheese sandwich': 120,
  'vegetable sandwich': 90,
  'manchurian sandwich': 110,
  'panner cheese sandwich': 140,
  'veg roll': 60,
  'veg cheese roll': 75,
  'panner roll': 80,
  'manchurian roll': 65,
  'vegetable pasta': 60,
  'chilli pasta': 65,
  'cold-coffee with icecream': 65,
  'cold-coffee': 60,
  'milk': 25,
  'coffee': 20,
  'tea': 10,
}

print('----------Welcome to Crazy Restaurant-----------')
print('Here is the Menu\n')
print("mix veg pizza: Rs.100\npanner pizza: Rs.80\ncheese pizza: Rs.85\npanner cheese pizza: Rs.120\nvegetable cheese burger: Rs.90\nveg cheese sandwich: Rs.120\nvegetable sandwich: Rs.90\nmanchurian sandwich: Rs.110\npanner cheese sandwich: Rs.140\nveg roll: Rs.60\nveg cheese roll: Rs.75\npanner roll: Rs.80\nmanchurian roll: Rs.65\nvegetable pasta: Rs.60\nchilli pasta: Rs.65\ncold-coffee with icecream: Rs.65\ncold-coffee: Rs.60\nmilk: Rs.25\ncoffee: Rs.20\ntea: Rs.10\n")

total_order_cost = 0
item1 = input("Enter the name of the item you want to order: ")
if item1 in menu:
  total_order_cost += menu[item1]
  print(f'Your item{item1} has been ordered..  Please wait..')
  
else:
  print(f'Ordered item {item1} is not available..')
  
another_item = input('Do you want to add another item? (yes/no)')
if another_item == 'yes':
  item2 = input("Enter the name of second item: ")
  if item2 in menu:
    total_order_cost += menu[item2]
    print(f'Item {item2} has been added')
  else:
    print(f'item {item2} is not available')
    
print(f'The Total amount of items are {total_order_cost}')
print('Thank You')
