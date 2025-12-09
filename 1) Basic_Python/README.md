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
### Exercise 1: Understanding variables:
#Declare three varibales. Print all Three variables.
```
name = 'salman' #String
age = 25 #Integer
height = 5.7 #Float

print('Name: ', name)
print('Age : ', age)
print('Height : ', height)
```

### Exercise 2: Data types:
#Create variable to store "a number, a decimal number,a word, a truth value(True/False)"

#Use the type() function to print the data type of each variable
```
number = 10
decimal = 3.14159
word = 'pillow'
truth = True

print('Whole number: ', type(number))
print('Decimal: ', type(decimal))
print('Word: ', type(word))
print('Truth Value: ', type(truth))
```


### Exercise 3: Type Conversion:
#create a variable with a string value of "25". Convert it into an integer and a float and print both results.
```
value = "25"
print(value)
print('Type of value:', type(value))
int_value = int(value) #converting str to int
print(int_value)
print('Type of int value: ', type(int_value))


float_value = float(value) #converting to float
print(float_value)
print('Type of float value: ', type(float_value))
```

### Exercise 4: Arithmetic Operators:
#Given the variables a=5, b=9 perform and print the results of the following operations:

#Addition,subtraction,multiplication,division,floor division,modulus,exponentiation.
```
a = 5
b = 9
print('Addition: ', a+b)
print('Subtraction: ', a-b)
print('Multiplication: ', a*b)
print('Division: ', a/b)
print('Floor Division: ', a//b) #only the whole number
print('Modulus (remainder): ', a%b) #what will remain after division
print('Exponentiation: ', a**b)  #a to the power b
```

### Exercise 5: Comparison and logical operators:
#Define two variables: x=5,y=10

#Print the results of the following comparisons:

#x is greater than y, x is less than or equal to y, x is equal to y, x is not equal to y.
```
x = 5
y = 10
print('x is greater than y:', x>y) #False
print('x is less than or equal to y:', x<=y) #True
print('x is equal to y:', x==y) #False
print('x is not equal to y:', x !=y) #True
```

--------------------------------------------------------------------------------------------------------------------------------

## a) For loop:

for loop repeats a block of code a fixed number of times. It is useful when you know in advance how many times you want to iterate.

```
for i in range (5):
    print("Iteration", i)
```

## b) While loop:
While loop repeats while a condition is True.
(we are only going to enter the loop if the condition is true. Be careful with infinite loop)

```
count = 0
while count < 3:
    print("Count:", count)
    count += 1   #increment count. if we miss this, it will be infinite loop.
```

## c) Breaking and skipping loops :
### break :
break basically you add the condition and then if the condition is met, you can break the loop.
```
for i in range (5):
    if i == 3:
        break
    print(i)
```

### continue: 
continue means skip the iteration.

```
for i in range (5):
    if i == 2:
        continue
    print(i)
```

## d) Conditional Statements: if-elif-else
Conditional statements allow your program to make decisions based weather certain conditions are true or false.
#### The if statement :
The if statement is the simplest form of conditional statement. It executes a block of code only if a specified condition is True.

```
#Basic of if statement
age = 18
if age >= 18:
    print("You are an adult.")
```

### The if-else statement :
The if-else statement provides an alternative block of code to execute when the condition is False.

```
#if-else statement
temperature = 15
if temperature > 25:
    print("Its a hot day.")
else :
    print("Its not very hot today.")
```

### The if-elif-else statement :
The if-elif-else statement allows you to check multiple conditions.

```
#if-elif-else statement
score = 85
if score >= 90:
    print("grade: A")
elif score >= 80:
    print("grade: B")
elif score >= 70:
    print("grade: C")
elif score >= 60:
    print("grade: D")
else:
    print("grade: F")
```


## e) Nested Conditional Statements :
You can also nest conditional statements inside each other.

```
#Nested if statements
age = 25
has_liscense = 1 #Bollean, any number=True, 0=False

if age >= 18:
    print("Age requirement passed.")

    if has_liscense:
        print("You can drive a car.")
    else:
        print(" You need a liscense to drive.")
else:
    print("You are too young to drive.")
```

## f) Logical Operators In Conditions :

and : Both conditions must be True.

or : At least one condition must be true.

not : Inverts the condition.(True becomes False, False becomes True)

```
#using logical operators:
age = 10
income = 65000

if age > 20 and income > 30000:
    print("You qualify for the loan.")
if age > 30 or income > 60000:
    print("You are qualify for the premium card.")
if not (age < 18):
    print("You are not a minor.")
```


## For Loop :

### For Loops with range() :
for loops allow you to execute a block of code multiple times. When using range(), the loops iterates over a sequence of numbers.

#### Basic For Loop with range() :
The range() function generates a sequence of numbers. By default it starts at 0 and increments by 1.

```
#Basic for loop with range
for i in range(5):
    print(f"Iteration {i}")
```
#### Specifying Start and stop in range() :
you can specify both the start and stop values in range().

```
#Range with start and stop values
for i in range(2,8):   #2 is minimum & 8 is maximum value
    print(f"Number: {i}")
```

#### Specifying Step in range() :
you can also specify the step (increment) value in range().

```
#Range with start, stop and step values
for i in range(1, 10, 2):   #start value, end-1, increment
    print(f"odd number: {i}")
```

#### Counting Backwards with range() :
you can count backwards by using a negative step value.

```
#counting backwords with range
for i in range(10, 0, -1):   #increment is negative, so it downgrade number
    print(f"countdown: {i}")
```

### Nested For Loops :
you can nest one for loop inside another to create more complex patterns.

```
#nested for loop
for i in range(1, 4):
    print(f"Outer loop {i}")
    
    for j in range(1, 3):
        print(f" inner loop{j}")
```

### Break & Continue in For Loops :

break: Exits the loop immediately

continue: Skips the current iteration and moves to the next one.

```
#using break in a for loop
for i in range(1, 10):
    if i == 5:
        print("Breaking the loop at i=5")
        break
    print(f"Number: {i}")
```

```
#using continue in a for loop
for i in range(1, 6):
    if i == 3:
        print("Skipping i=3")
        continue
    print(f"Number: {i}")
```

