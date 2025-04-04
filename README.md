num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
operation = input("Choose an operation (addition, subtraction, multiplication, division): ").lower()
if operation == "addition":
    result = num1 + num2
    symbol = "+"
elif operation == "subtraction":
    result = num1 - num2
    symbol = "-"
elif operation == "multiplication":
    result = num1 * num2
    symbol = "*"
elif operation == "division":
    if num2 != 0:
        result = num1 / num2
        symbol = "/"
    else:
        result = "undefined (cannot divide by zero)"
        symbol = "/"
else:
    result = "Invalid operation"
    symbol = "?"
print(f"{num1} {symbol} {num2} = {result}")
