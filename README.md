# Intro-to-Python

Python code is both compiled and interpreted


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

## These are commmennt
"#" single line comments
'''Some string'''  multi-line comment

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

  ## OR Opeartor
  
is_male = False
is_Tall = True

if is_male:
    print("You are a male")
else:
    print ("You are not a male")

    if is_male or is_Tall:
        print("You are a male or tall or both")
    else:
    print ("You are not either male or Tall")

## AND Operator 

is_male = False
is_Tall = False

if is_male:
    print("You are a Tall male")
    
elif is_male and not (is_Tall)
      print("You are a short Male")
      
elif not (is_male) and is_Tall
      print("You are a short Male")
      
else:
    print ("You are not a male and not tall")


## Comparisons 
def max_num(num1, num2, num3):
    if  num1 >= num2 and num1>= num3:
        return num1
    elif num2 >= num1 and num2 >= num3:
          return num2
    else:
         return num3

print(max_num(3,4,5))

print(5==4) checks for equality 
it will print False

print(5!=4)
it will print True

There are many operators we can use: ==,>=, <=, <, >, !=

    
## Lists
Stores list of information, you can put stings, numbers or anything in the list

friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby" ]
print(friends) // Print all listed frinds

print(friends[0]) can only print 1st index which is Kevin
print(friends[-1]) can only print Jim, when you use (-)  //it starts from back of the list 

print(friends[1:])  // start to print fron index 1 which is Jim
print(friends[1:3]) //Only print index 1,2

friends[1] = "Mike"   // updating the 1st element
print(friends[1])  // this will print Mike

## List Functions

lucky_numbers = []4, 8, 15, 16 , 23, 42]
friends = ["Kevin", "Karen", "Jim", "Oscar", "Toby" ]

print(friends)  // print only friend

print.extend(lucky_numbers) // allow you to take a list and append other list
print(friends)  //  now the output will include lucky numbers and friends

friends.append("Creed") // Add creed to the list
firnds.insert(1, "Kelly") Insert Kelly to the 1st index.
friends.remove("Jim") // Jim is removed from the list
friend.clear()  // get rid of all elements in the list
friends.pop() // Removes the last element in the list
print(friends.index("Kevin")) // tells you the index where Kevin is
print(friends.count("Kevin")) // tells you how many times Kevin appears on the list 
friends.sort() // Sort the elements ascending or alphabetically
lucky_numbers.reverse() // Rreverse the numbers starting from the last number
friends2 = frinds.copy() // copy the elements of the friends list to friends2


## Tuples
is a type of data structure, basically means its a container that can store different values more like lists.
Stores multiple values
They are immutable, Can not be changed or modified, can not add elements 

corodinates = (4, 5)     // Tuples use parenthesis while list uses square brackets
print(cordinates[0])     // this will print 4

corodinates = [(4, 5), (6, 7), (80, 34)]  // Square brackest only used when you have list of Tuples 

You cannot remove items from a tuple.
Tuples are very memory-efficient.
Sets must contain unique values.

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


## Return Statement
def cube(num):
    num*num*num
print (cube(3)) // print none 

def cube(num):
    return num*num*num
print (cube(3)) // prints 27 which is 3**3


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


## Dictioneries
is a special structure which allows you to store information in key value pairs 
word is a key and value is the actual defination.
Keys must be unique
Keys do not have to be string hey can be numbers too

monthConversions = {
    "Jan": "January",
    "Feb": "February",
    "Mar": "March", 
}
print(monthConversion["Jan"]) // this will pint full name which is January, it give you value that is associated with the key

if you print key that is not in the dictionary it prints none

 ## Handling missing keys in a dictionary:
using a defaultdict
checking with an "if key in dictionary" statement, then adding a value
using the get function

## Objects and Classes
super() used to get an instance of the parent class

## Import Libraries

import math
print("pri is", math.pi")  importing pi value which is 3.14



        
