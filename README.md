# Function 1: Sum of 5 numbers
def func1(a, b, c, d, e):
    return a + b + c + d + e

# Function 2: Multiplication of 5 numbers
def func2(a, b, c, d, e):
    return a * b * c * d * e

# Function 3:  Function 2 - Function 1, func 2*func1, func 2 + func 1, func 2 / func 1)
def func3(x, y):
    print("Subtraction (func2 - func1):", y - x)
    print("Multiplication (func2 * func1):", y * x)
    print("Addition (func2 + func1):", y + x)

    if x != 0:
        print("Division (func2 / func1):", y / x)
    else:
        print("Division not possible (division by zero)")

# Taking input
a = int(input("Enter number 1: "))
b = int(input("Enter number 2: "))
c = int(input("Enter number 3: "))
d = int(input("Enter number 4: "))
e = int(input("Enter number 5: "))

# Calling functions
sum_result = func1(a, b, c, d, e)
mul_result = func2(a, b, c, d, e)

# Only func3 will print
func3(sum_result, mul_result)
