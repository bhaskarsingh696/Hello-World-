def calculator():
    print("Advanced Calculator")
    print("You can input expressions like: 2+3*5 or (10+5)/3")

    try:
        expression = input("Enter your mathematical expression: ")
        result = eval(expression)  # Evaluates the expression
        print(f"The result is: {result}")
    except ZeroDivisionError:
        print("Error: Division by zero is not allowed.")
    except Exception as e:
        print(f"Error: Invalid input ({e})")

calculator()