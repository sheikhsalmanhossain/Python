## Basic Stractures: Variables, Data Types and Operators:

A variable is a named container for storing data.

```
Defferent type of variable :
name = 'salman'      #(String - any type of text)
age = 25             #(Integer- whole number)
height = 5.7         #(Float - any number with decimal place)
is_student = True    #(Boolean - True or False)

print("Name:", name)
print("Age:", age)
print("Height:", height)
print("Is a student:", is_student)

```

### Type Conversion :
```
print("\nConverting data types:")
age_str = str(age) # convert int to string
height_int = int(height) # Convert float to int
is_student_int = int(is_student) # Convert Boolean to int



print("Age as string:", age_str, "(Type:", type(age_str), ")")
print("Height as integer:", height_int, "(Type:", type(height_int), ")")
print("Boolean as integer:", is_student_int, "(Type:", type(is_student_int), ")")

```

## Basic structure operations :

### Operators in python :

```
print("\nArithmetic Operators:")
a = 10
b = 3
print("Addition:", a + b)
print("Subtraction:", a - b)
print("Multiplication:", a * b)
print("Division:", a / b)
print("Floor Division:", a // b)
print("Modulus (Remainder):", a % b)
print("Exponentiation:", a ** b)


print('\nComparison Operators')
print('a is greater than b:', a > b)
print('a is less than b:', a < b)
print('a is greater than or equal to b:', a >= b)
print('a is less than or equal to b:', a <= b)
print(' a is equal to b:', a == b)
print('a is not equal to b:', a != b)


print('\nLogical Operators')
print(a > b and a < 20)
print(a < b or a > 11)
```

## Exercise :
### Exercise1: Understanding variables:
#Declare three varibales. Print all Three variables.
```

name = 'salman' #String
age = 25 #Integer
height = 5.7 #Float

print('Name: ', name)
print('Age : ', age)
print('Height : ', height)
```
