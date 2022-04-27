# This program determines whether there are certain items
# or if there aren't any
# the user will be informed
# that the item is not in
# stock

user_request_of_items = int(input("Enter the amount of item\'s: "))
limit_number = 1

while limit_number <= user_request_of_items:
    if user_request_of_items > 5:
        print("Please select only 5 item\'s or less. ")
    list_of_items = [
                    ["Basketball", "Soccer ball", "Tennis ball", "Football"],
                    ["Mouth wash", "Toothbrush", "Listerine", "Toothpick"],
                    ["Shirt", "Pants", "Underwear", "Muscle-shirt"],
                    ["Samsung", "Apple", "LG", "Motorola"]
                    ]

    user_interaction = str(input("Enter the item you\'re looking for: "))

    if user_interaction in list_of_items[0]:
        print("Still in stock")
    elif user_interaction in list_of_items[1]:
        print("Few item\'s in stock")
    elif user_interaction == list_of_items[2][0] or user_interaction == list_of_items[2][1] or \
            user_interaction == list_of_items[2][2] or user_interaction == list_of_items[2][3]:
        print("Item\'s running low in stock")
    elif user_interaction in list_of_items[3]:
        print("Must click following link for further instructions. ")
    else:
        print('\nOut of Stock' * 4)

    limit_number += 1
print("Thank for choosing コンビニエンスストア(Convenient Store)")
