# PYTHON PROGRAMING MODULE 2
## Name: SAKTHI SUNTHAR K K
## Register Number: 212225040361
## Date: 23.3.26

# Built-in Functions -Binary Conversion Using Built-in Functions in Python

## 🎯 Aim
To write a Python program to convert the number **16** into its **binary representation** using built-in Python functions.

## 🧠 Algorithm
1. Assign the value `16` to a variable `a`.
2. Use the built-in `bin()` function to convert the number to binary.
3. Print the result.

## 🧾 Program
```
a = 16
print(bin(a))
```
## Output

![502979761-8d96f9fc-b6a6-4b22-9c56-8acc05ea1dd7](https://github.com/user-attachments/assets/43568afa-6013-463f-8dd9-c51a9e69b66b)

## Result
The program successfully converts the number 16 into its binary representation and displays the result as 0b10000 on the screen.


# Functions in Python: Modulo Calculator

## 🎯 Aim
To write a Python program that defines a function which accepts two values and returns their **modulo** using the `%` operator.

## 🧠 Algorithm
1. Define a function called `result` that takes two arguments `a` and `b`.
2. Inside the function, compute the modulo using `a % b`.
3. Print the result of the modulo operation.
4. Get two integer inputs from the user.
5. Call the `result` function with the user-provided values.

## 🧾 Program
```
def result(a,b):
   return a%b
a=int(input())
b=int(input())
modulo=result(a,b)
print("modulo is",modulo)
```
## Output

![502979972-8b040bc5-e390-4c61-ab87-6aa5d8a165a2](https://github.com/user-attachments/assets/6bd1baa3-a03c-408e-9b55-8d0e872b2ca4)

## Result
The program successfully defines a function and returns the modulo of the two inputs


# Lambda Function in Python: Addition of Two Numbers

## 🎯 Aim
To write a Python program that defines a **lambda function** which takes two arguments `a` and `b`, and returns their sum.

## 🧠 Algorithm
1. Get two integer inputs from the user.
2. Use a **lambda function** to define a function `f` that returns `a + b`.
3. Call the function with the user inputs and print the result.

## 🧾 Program
```
a=int(input())
b=int(input())
f=lambda a,b:a+b
c=f(a,b)
print(c)
```

## Output

![502987960-24c80356-08bf-4aff-bc88-689ed4835fca](https://github.com/user-attachments/assets/197cc355-1d07-48fa-a6cf-4dd306dbba65)

## Result
The program successfully created lambda function to find the sum.


# 🔺 Looping(Patterns)-Pascal's Triangle Generator in Python

This project demonstrates a simple Python program to generate **Pascal’s Triangle**, where the number of rows is provided by the user.

---

## 🎯 Aim

To write a Python program that generates **Pascal's Triangle** using numbers. The number of rows is accepted from the user.

---

## 🧠 Algorithm

1. Start the program.
2. Input the number of rows from the user.
3. Loop from 0 to the number of rows.
4. For each row:
   - Print appropriate spaces to shape the triangle.
   - Compute values using the formula:  
     \[
     C(n, k) = \frac{n!}{k!(n-k)!}
     \]
5. Print all rows of Pascal’s Triangle.
6. End the program.

---

## 🧪 Program
```
def pascal_triangle(n):
    for i in range(n):
        print(" "*(n-i-1),end="")
        val=1
        for j in range(i+1):
            print(val,end=" ")
            val=val*(i-j)//(j+1)
        print()
n=int(input())
pascal_triangle(n)
```

## Sample Output

![502980149-818e79d2-e43f-47e8-b1bd-0ba71c278922](https://github.com/user-attachments/assets/51e6f829-c905-4011-838a-1985b5122266)

## Result
The Python program successfully takes the number of rows as input from the user and generates Pascal’s Triangle.


## Loops in Python: Palindrome Number Checker

## 🎯 Aim
To write a Python program that checks whether a given number is a **palindrome** using loops.

## 🧠 Algorithm
1. Get input from the user and assign it to a variable `num`.
2. Assign the value of `num` to a temporary variable `temp`.
3. Initialize a variable `rev` to 0 (used to store the reversed number).
4. Use a `while` loop to reverse the digits:
   - While `temp > 0`:
     - `rev = (10 * rev) + temp % 10`
     - `temp = temp // 10`
5. After the loop, compare `rev` with `num`:
   - If equal, print that the number is a palindrome.
   - Else, print that it is not a palindrome.

## 🧾 Program
```
n=int(input())
rev=0
org=n
while n>0:
    rem=n%10
    rev=rev*10+rem
    n//=10
if(rev==org):
  print("The given number",org,"is a Palindrome")
else:
    print("The given number",org,"is not a palindrome")
```
## Output

![502980573-2eef6559-26f4-43c4-b6e5-d6e94e3e0548](https://github.com/user-attachments/assets/43fe3d1d-290a-4cf3-812e-07d9db7cd1fb)

## Result
The program successfully takes a number as input from the user, reverses it using a while loop, and compares it with the original number. If both are equal, it confirms that the number is a palindrome; otherwise, it displays that it is not a palindrome.
