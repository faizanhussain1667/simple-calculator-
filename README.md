# simple-calculator-

# Function to add two numbers
def add(x, y):
    return x + y

# Function to subtract two numbers
def subtract(x, y):
    return x - y

# Function to multiply two numbers
def multiply(x, y):
    return x * y

# Function to divide two numbers
def divide(x, y):
    return x / y

# Prompt the user for input
print("Select operation:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

# Take input from the user for operation
choice = input("Enter choice (1/2/3/4): ")

# Take input from the user for numbers
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

# Perform the operation based on user choice
if choice == '1':
    print(f"The result of {num1} + {num2} is: {add(num1, num2)}")
elif choice == '2':
    print(f"The result of {num1} - {num2} is: {subtract(num1, num2)}")
elif choice == '3':
    print(f"The result of {num1} * {num2} is: {multiply(num1, num2)}")
elif choice == '4':
    if num2 != 0:
        print(f"The result of {num1} / {num2} is: {divide(num1, num2)}")
    else:
        print("Error! Division by zero is not allowed.")
else:
    print("Invalid input. Please select a valid operation."
