# Cataloge-of-cars. That is simple cataloge of car. There you can add and show your collection!


cars = []

while True:
    print("\n That is your cataloge of cars!")
    print("1 - Add a new car to the list: ")
    print("2 - Show all cars from the list: ")
    print("3 - Exit")
    
    cataloge = input("Which option do you want to choice?")
    
    if cataloge == "1":
        w = input("Which car do yo want to add?")
        cars.append(w)
        print("This car added successfully!")
        
    elif cataloge == "2":
        if not cars:
            print("No cars in the list yet.")
        for i, car in enumerate(cars, start = 1):
            print(f"{i}. {car}")

    elif cataloge == "3":
        question = input("Are you sure? (yes/no): ").lower()
        if question == "yes":
            print("BYE!")
            break
        else:
