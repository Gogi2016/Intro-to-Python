# Intro-to-Python

Python 

## Working with number & Operators
print(2+2)
  output will be 4

print(5%2)
  output will be 1 (remainder)

## Strings
print("Whatsúp")
  output will be Whatsúp

Alwyas type you string in sides quotes
you can use single or double qoutes when printing a string

# This is a commmennt

## Variables
Must contain letterd, numbers or underscores
Should not start with a number
Spaces are not allowed
can not be key words
Case Sensitive (GOGI is not the same with gogi)
short and descriptive

Examples
name = "Vuyokazi" 
print(name) it will print Vuyokazi

age = 30
age = 24
print(age)
  it will print 24 because it will take the last value that is assigned to it 

del a(age) this will delete variable "age" and it wont be printed out bcz it is deleted 
  
to see the type 
print(type(name)) this will print <class str>
print(type(age)) this will print <class int>

## To allow input
name = input(What is your name?)
print(name)
  it will allow you to write on the terminal

## Conditional Logic
print(5==4) checks for equality 
it will print False

print(5!=4)
it will print True

There are many operators we can use: ==,>=, <=, <, >, !=

## If, Elif, Else statement
Thomas_Age = 3
Age_at_Kindergarten = 5
print(Thomas_Age == Age_at_Kindergarten) This will print False

Thomas_Age = 3
Age_at_Kindergarten = 5

if Thomas_Age < Age_at_Kindergarten:
    print("Thomas should be in pre-school") // it will print this if its true (if 3<5)

elif Thomas_Age == Age_at_Kindergardten
     print("Enjoy Kindergarten") // it wi print this if 3 was equal to 5

else:
     print("Thomas should be in another class") // or print this if its false it 3 was not less than 5)


## Lists
Stores list of information

friends = ["Kevin", "Karen", "Jim" ]



## Functions
Its a block of code that you can package it together with a name and does something, it takes an action. 

def print_DSTV():
    text = "DSTV has a great channels"
    print(text)

print_DSTV()  //this calls a function, if you did not call the fuction it will print nothing
    

def print_DSTV(text): expecting text to be passed in
    print(text)

print_DSTV("DSTV has a great channels") passed values

useing If statement in function 

def school_age_calculator(age,name)
     if age < 5:
       print("Enjoy your time", name "is only", age)
      elif age ==5:
        print("Enjoy Kindergarten", name)
      else:
        printy("They grow up so fast")

        school_age_calculator(3,"Thomas") // Enjoy your time, Thomas is only, 3
        school_age_calculator(5,"Thomas") // Enjoy Kindergarten, Thomas
        school_age_calculator(10,"Thomas") // They grow up so fast


def add_ten_to_age(age):
    new_age = age + 10
    return new_age

How_old_will_i_be = add_ten_to_age(3)
print(How_old_will_i_be)               // it retirns 13


## Loops
Allows you to execute a block of code multuply time

## While
x=0
while (x<5):
   print(x)
   x=x+1  adding 1 till x is no longer less than 5
   // print from 0 and when x 
    

## For
for x in range(5,10):
     print(x) it start from 5 up untill 10 but does not include 10

days =["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "sun" ]

for d in days:
     if(d=="Thu"): break  // it will stop when it breaks and no longer continue, does not include Thu
     print(d)


for d in days:
     if(d=="Thu"): continue // skip Thursday and continue with other days
     print(d)

## Import Libraries

import math
print("pri is", math.pi")  importing pi value which is 3
.14



        
