# Python-Assignment
Simple Calculator Program

def main():
    # Get user input
    num1 = float(input("Enter the first number: "))
    num2 = float(input("Enter the second number: "))
    operation = input("Enter the operation (+, -, *, /): ")
    # Perform the operation
    if operation == '+':
        result = num1 + num2
    elif operation == '-':
        result = num1 - num2
    elif operation == '*':
        result = num1 * num2
    elif operation == '/':
        if num2 != 0:
            result = num1 / num2
        else:
            print("Error: Division by zero is not allowed.")
            return
    else:
        print("Error: Invalid operation.")
        return
    # Print the result
    print(f"{num1} {operation} {num2} = {result}")

if __name__ == "__main__":
    main()

    PS C:\Users\HomePC\Desktop\Files\PLP> python PythonAssignment.py
Enter the first number: 12
Enter the second number: 6
Enter the operation (+, -, *, /): /
12.0 / 6.0 = 2.0
PS C:\Users\HomePC\Desktop\Files\PLP> 
