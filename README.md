# Task-1
def add(a, b):
    return a + b

def subtract(a, b):
    return a - b

def multiply(a, b):
    return a * b

def divide(a, b):
    if b == 0:
        return "Error! Division by zero."
    return a / b

def calculator():
    print("Welcome to the basic calculator!")

  try:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))

   print("\nChoose an operation:")
        print("1. Addition (+)")
        print("2. Subtraction (-)")
        print("3. Multiplication (*)")
        print("4. Division (/)")

  choice = input("Enter the operation (1/2/3/4): ")

  if choice == '1':
            result = add(num1, num2)
            operation = '+'
        elif choice == '2':
            result = subtract(num1, num2)
            operation = '-'
        elif choice == '3':
            result = multiply(num1, num2)
            operation = '*'
        elif choice == '4':
            result = divide(num1, num2)
            operation = '/'
        else:
            print("Invalid operation choice.")
            return

  print(f"\nResult: {num1} {operation} {num2} = {result}")

   except ValueError:
        print("Error! Please enter a valid number.")

# Run the calculator
calculator()
