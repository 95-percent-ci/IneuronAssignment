## Assignment Part-1

Q1. Why do we call Python as a general purpose and high-level programming language?

Python is called general purpose as it can be used to create variety of applications in different domains (Data Science, User Interface, Web Development Etc). For example HTML is not general purpose as it is created mainly to create front end solutions

Python is high-level programming language as it is create with ease of understanding and usage of english semantics in mind. Python has an interpreter which converts the code into Machine Code, which is then sent to processor

Q2. Why is Python called a dynamically typed language?

Python doesn't knows the data type of the variable when it is created. This is inferred during the runtime

Languages Like C++, needs to have data type defined for a variable when it created, to allocate memory

Q3. List some pros and cons of Python programming language?

| Pros                                   | Cons                                                                                                                                                                                                                                                          |
| -------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Easier to understand and use           | Not used to building enterprise level application                                                                                                                                                                                                             |
| Number of Lines of Code is Less        | Execution is slower as compared to c++ as it is high level language                                                                                                                                                                                           |
| Large use base and open source support | No Support for Multithreading. As Python is interpreted language, the code gets converted into bytecode and sent to PVM (Python Virtual Machine) to convert to Machine Code and effectively a single sequence is handled due to Globle Interpreter Lock (GIL) |
|                                        |                                                                                                                                                                                                                                                               |


Q4. In what all domains can we use Python?

Web development, Data Science, UI , Automation, DevOps

Q5. What are variable and how can we declare them?

Q6. How can we take an input from the user in Python?

Python Built-ins function `input()` can be used to take input from user. 
Other way is to use command line arguments

Q7. What is the default datatype of the value that has been taken as an input using input() function?

Default datatype is string 

Q8. What is type casting?

Type Casting is method of convertin a DataType to Another Data Type. For Example

```num_str = "5"  
   num_int = int(num_str)
```

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

We can take more than input by single use of `input()` function.  Since return of input is a string, this string can be spliited into multiple variables by using split function using a separator

For example if I want take 2 values of input() function

```
# Keep single space between x and y while inputting 
x, y = input("Enter 2 Numbers").split(" ") 
```

Q10. What are keywords?

Keywords in any programming language are special words that have specific meaning and purpose
There are 35 Keywords that are available in Python anytime a code or script is run 

Q11. Can we use keywords as a variable? Support your answer with reason.

No we can't use keywords as a variable. Suppose I create a variable named **print** , this will clash directly with keyword **print** and I would get error during the runtime of the code

Q12. What is indentation? What's the use of indentaion in Python?



Q13. How can we throw some output in Python?

Using **print** keyword

Q14. What are operators in Python?

Operators are used to operate in values and variables. This could include mathematical operatos, logical operators, comparison operators, assignment operators, bitwise operators etc

Q15. What is difference between / and // operators?

/ is simple Float Division, where for example 5 / 2 = 2.5
// is Floor Division, where for example 5 // 2 = 2

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```

```
val_str = "iNeuron"
print(val_str * 4)
```

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

```
x = int(input("Enter the Number to check for odd or even"))

if x % 2 == 0:
   print('Even')
else:
   print('Odd')
```

Q18. What are boolean operator?

Boolean operators (True, False) is used to check for truth or false for any statement in python


Q19. What will the output of the following?
```
1 or 0
True

0 and 0
False

True and False and True
False

1 or 0 or 0
True
```

Q20. What are conditional statements in Python?

Conditional Statements are a form of control sequence which checks for truthfullness of a statement and extecutes next part of code

Q21. What is use of 'if', 'elif' and 'else' keywords?

**if**:  Statement is true then, indented code block is executed

**else**: if statement is False, indented block inside else block is executed

**elif**: Nested if-else, with same logic as above

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

```
age = float(input('Enter the Age'))

if age >= 18:
   print('I can vote')
else:
   print("I can't vote")

```

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

```
numbers = [12, 75, 150, 180, 145, 525, 50]

sum_even = 0

for num in numbers:
   if num % 2:
       sum_even += num

print(sum_even)

```

Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

```
x,y,z = input("Enter 3 numbers").split(" ")

# Changing Data Type
x, y, z = float(x), float(y), float(z)

if x > y:
   if x > z:
      print(x)   
else:
   if y > z:
      print(y)
   else:
      print(z)
```

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

```
numbers = [12, 75, 150, 180, 145, 525, 50]
select_list = []

for val in numbers:
   if val == 500:
      break
   if val % 5 == 0 and val < 150:
      select_list.append(val)

print(select_list)      
```