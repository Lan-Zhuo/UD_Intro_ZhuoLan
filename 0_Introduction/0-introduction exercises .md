# Exercise 00

Write a bit of code that prints Introduction to Programming to the console and execute the cell


```python
print('Introduction to Programming')
```

    Introduction to Programming


# Exercise 01

Hello World is traditionally the first program anyone writes. It is very simple and the only thing it should do is print Hello World! to the terminal window. Create a file called HelloWorld.py and edit the contents so it prints Hello World! to the terminal and execute it using the command line.

![%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-10-02%20235427.png](attachment:%E5%B1%8F%E5%B9%95%E6%88%AA%E5%9B%BE%202023-10-02%20235427.png)

# Exercise 02

Write some code to print your name, email, and age on separate lines. For each element first assign it to a variable and use the variable to print.

Bonus: try to create the print statement for all variable in one line of code. (hint: '\n' is the character for a new line)


```python
name=' Lan Zhuo\n'
email='lan.zhuo.23@ucl.ac.uk\n'
age='23\n'
print(name,email,age)
```

     Lan Zhuo
     lan.zhuo.23@ucl.ac.uk
     23
    


# Exercise 03

Print the numbers 0, 178, -21, 2938 divided by 49, 436 multiplied with 9948 and 12 to the power of 20

(Hint: Look up the documentation of basic arithmetic operators)


```python
for i in {0,178,-21,2938}:
    m=i/49
    print(m)
print(436*9948)
print(12**20)
```

    0.0
    3.63265306122449
    -0.42857142857142855
    59.95918367346939
    4337328
    3833759992447475122176


# Exercise 04

Print sin(200), cos(100), tan(π/4)

(Hint: Look up for how to use trigonometric function, and how to get the value of π.)


```python
import math
print(math.sin(200))
print(math.cos(100))
print(math.tan(math.pi/4))
```

    -0.8732972972139945
    0.8623188722876839
    0.9999999999999999


# Exercise 05

Write a program to read your first and last names from the console seperately, and then print them on the console together, separated by a space.


```python
firstname='lan'
lastname='zhuo'
print(firstname)
print(lastname)
print(firstname+' '+lastname)
```

    lan
    zhuo
    lan zhuo


# Exercise 06

Write a program that determines whether a number given as user input is positive or negative

You will need to convert the console input from a string to a number first!


```python
x=int(input())
if x>0:
    print('The given number is positive')
elif x<0:
    print('The given number is negative')
else:
    print('The given number is zero')
```

    0
    The given number is zero


# Exercise 07

Write a program that picks a random number between 1-20 and makes the user guess until they get the number right. Then print a congratulations message

(Find out yourself how to generate a random integer)

Bonus: make the user choose the range within which they have to guess

Bonus: keep track of how many guesses were made and print this at the end


```python
import random
x=random.randint(1,21)
y=int(input())
t=0
while y!=x:
    print('Sorry,you are wrong!')
    t=t+1
    print("Let's have some tips!I will give you a range,please enter a number to compare with the answer.")
    z=int(input())
    if x>z:
        print('Bigger!')
    elif x<z:
        print('Smaller!')
    else:
        print("Congratulations !That's it!")
    y=int(input())
print('Congratulations !')
```

    8
    Sorry,you are wrong!
    Let's have some tips!I will give you a range,please enter a number to compare with the answer.
    10
    Bigger!
    15
    Sorry,you are wrong!
    Let's have some tips!I will give you a range,please enter a number to compare with the answer.
    15
    Smaller!
    13
    Sorry,you are wrong!
    Let's have some tips!I will give you a range,please enter a number to compare with the answer.
    13
    Bigger!
    14
    Congratulations !


# Exercise 08

Ask a sentence as input, then print the words in alphabetical order. Hint: look up how to split up a string



```python
x=input()
list1=list(x)
list2=sorted(list1)
print(list2)
```

    qafjwirof
    ['a', 'f', 'f', 'i', 'j', 'o', 'q', 'r', 'w']


# Exercise 09

Write a program using for loops to print a christmas tree of x lines high specified by the user. (use for loops) so for instance, a chrismas tree of 4 high should looks like this:

hint: first combine strings into a variable before printing


```python
x=int(input())
z=x+1
list1=list(range(1,z))
for i in list1:
    y=i*2-1
    t=x-i
    print(' '*t+'*'*y)
print(' '*(x-1)+"|")
```

    3
      *
     ***
    *****
      |


# Exercise 10

Write a piece of code that prints the first n numbers of the padovan sequence


```python
x=int(input())
t=4
if x<4:
    if x==1:
        print(1)
    elif x==2:
        print('1,1')
    else:
        print('1,1,2')
list1=[1,1,2]
if x>=4:
    while x-t>=0:
        y=list1[t-3]+list1[t-4]
        list1.append(y)
        t=t+1
print(list1)
```

    10
    [1, 1, 2, 2, 3, 4, 5, 7, 9, 12]



```python

```
