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
# Class Attributes
What is a class attribute? A class attribute is a variable that belongs to a class. It is a property of the class. It belongs to the class rather than any specific object. This attribute is created outside of the constructor method (__init__). Below, we have a code that demonstrates how we create class attributes in a class.
A class is a prototype from which objects are created. Classes provide a means of bundling data and functionality together.

Syntax: Class Definition
class ClassName:
    # Statement
    
super() used to get an instance of the parent class
To create a class named MyClass:
                                  class MyClass :
                                  x = 5
Now we can use the class named MyClass to create objects:
Create an object named p1, and print the value of x:
p1 = MyClass()
print(p1.x) // 

Create a class named Person, use the __init__() function to assign values for name and age:
class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

p1 = Person("John", 36)

print(p1.name)
print(p1.age)

The __init__() function is called automatically every time the class is being used to create a new object.

The __str__() function controls what should be returned when the class object is represented as a string.
If the __str__() function is not set, the string representation of the object is returned:

class Person:
  def __init__(self, name, age):
    self.name = name
    self.age = age

  def __str__(self):
    return f"{self.name}({self.age})"

p1 = Person("John", 36)

print(p1)


# Instance Attributes
Class attributes (variables) belong to a class and not to a specific object. However, we can also create instances that belong to an object or instance. These attributes are called “instance attributes.” Instance attributes are created inside a constructor. The constructor for instance attributes is the __init__() method. 
Instance attributes are declared inside any method, while class attributes are declared outside any method.

# Instance Methods
Instance methods can access and modify both class attributes and instance attributes. Similar to a class method, an instance method is just a function in a class. It also starts with the keyword “def”. Its first parameter is the keyword “self”

# Static Methods
static methods cannot access class attributes or instance attributes. In Python, we create a static method using a decorator. We write @staticmethod right above the method we want to decorate. Static methods have no implicit first argument. Neither cls nor self is passed as the first argument. Static methods are just functions that you can call from the class or instance of the class

# Summary
Class methods can access class attributes, but they cannot access instance attributes. Instance methods can access both class and instance attributes. Static methods are just utility functions. They do not have access to class attributes or instance attributes.

Syntax Python Static Method: 
class C(object):
    @staticmethod
    def fun(arg1, arg2, ...):
        ...
returns: a static method for function fun.

## Inheritance
Inheritance allows us to define a class that inherits all the methods and properties from another class.
Parent class is the class being inherited from, also called base class.
Child class is the class that inherits from another class, also called derived class.
Use the pass keyword when you do not want to add any other properties or methods to the class.

# Syntax
Class BaseClass:
    {Body}
Class DerivedClass(BaseClass):
    {Body}

# Creating a Parent Class
     # A Python program to demonstrate inheritance
class Person(object):

      # Constructor
def __init__(self, name, id):
	self.name = name
	self.id = id

       # To check if this person is an employee
def Display(self):
	print(self.name, self.id)

       # Driver code
emp = Person("Satyam", 102) # An Object of Person
emp.Display()

# Creating a Child Class
   class Emp(Person):

def Print(self):
	print("Emp class called")
	
Emp_details = Emp("Mayank", 103)

    # calling parent class function
Emp_details.Display()

    # Calling child class function
Emp_details.Print()

# Example of Inheritance in Python 
A Python program to demonstrate inheritance
Base or Super class. Note object in bracket.
(Generally, object is made ancestor of all classes)
In Python .x "class Person" is equivalent to "class Person(object)"

class Person(object):

	# Constructor
	def __init__(self, name):
		self.name = name

	# To get name
	def getName(self):
		return self.name

	# To check if this person is an employee
	def isEmployee(self):
		return False


# Inherited or Subclass (Note Person in bracket)
class Employee(Person):

	# Here we return true
	def isEmployee(self):
		return True


# Driver code
emp = Person("Geek1") # An Object of Person
print(emp.getName(), emp.isEmployee())

emp = Employee("Geek2") # An Object of Employee
print(emp.getName(), emp.isEmployee())


## Import Libraries

import math
print("pri is", math.pi")  importing pi value which is 3.14

## Handling Errors and Exceptions
Errors and exceptions in Python may seem like different things, but they essentially work in similar ways. While the official Python documentation distinguishes exceptions as runtime issues that can be retried, and errors as non-recoverable, this isn't always strictly adhered to, even within Python itself.

Both errors and exceptions originate from the base exception class and share common properties for halting code execution and providing information about why the execution stopped. For instance, a division by zero error is a type of arithmetic error, which is a type of exception, all extending from the base exception class.

When an error or exception occurs, Python provides a stack trace, showing the trail of nested function calls where the error happened. This stack trace is crucial for debugging, especially in larger programs.

To handle exceptions, Python offers the try and except statements. By catching exceptions, you can prevent your program from crashing and obtain information about the error that occurred.

For example, you can catch a zero division error like this:

try:
    1/0
except Exception as e:
    print(type(e))
    
This code catches the zero division error, preventing it from crashing the program, and prints out the type of the exception (ZeroDivisionError in this case).

Overall, while exceptions may seem daunting, they are simply classes that can be handled like any other part of your code. Learning to handle exceptions effectively is an essential skill for writing robust and reliable Python programs.

## Different types of exceptions in python:
SyntaxError: This exception is raised when the interpreter encounters a syntax error in the code, such as a misspelled keyword, a missing colon, or an unbalanced parenthesis.
TypeError: This exception is raised when an operation or function is applied to an object of the wrong type, such as adding a string to an integer.
NameError: This exception is raised when a variable or function name is not found in the current scope.
IndexError: This exception is raised when an index is out of range for a list, tuple, or other sequence types.
KeyError: This exception is raised when a key is not found in a dictionary.
ValueError: This exception is raised when a function or method is called with an invalid argument or input, such as trying to convert a string to an integer when the string does not represent a valid integer.
AttributeError: This exception is raised when an attribute or method is not found on an object, such as trying to access a non-existent attribute of a class instance.
IOError: This exception is raised when an I/O operation, such as reading or writing a file, fails due to an input/output error.
ZeroDivisionError: This exception is raised when an attempt is made to divide a number by zero.
ImportError: This exception is raised when an import statement fails to find or load a module.


## Managing and Handling Exceptions
Exceptions in Python are not something to fear, but they do need to be managed effectively. One way to handle them is with the try/except statement. By using this pattern, you can catch exceptions and perform specific actions, such as returning the exception instance or printing a message.

Additionally, the finally statement can be added to ensure certain code always executes, regardless of whether an exception occurred. This is useful for cleanup tasks or logging. You can also use the time module to time the execution of a function, which is often done within a finally block.

When catching exceptions, it's important to consider the order of except statements. More specific exceptions should be caught before more general ones to ensure proper handling.

For more complex exception handling, such as dealing with different types of HTTP errors, you might want to encapsulate the try/except logic into a single function or use custom decorators. Decorators can help streamline exception handling and make your code more modular and reusable.

Raising exceptions is another aspect to consider. You can use the raise statement to create and throw custom exceptions. This is particularly useful for enforcing specific conditions in your code and providing clear error messages when those conditions are not met.

Overall, understanding how to effectively handle exceptions, whether by catching them, using finally blocks, or raising them yourself, is essential for writing robust and reliable Python code.

## Working With Custom Exceptions
Creating custom exceptions in Python is straightforward. You can define a custom exception class by extending the built-in Exception class:
class CustomException(Exception):
    pass
This creates a lightweight custom exception class that inherits the constructor of the Exception class. Typically, custom exceptions contain minimal additional attributes or methods, relying mainly on their name to convey information about the error.

You can raise a custom exception by defining a function that uses the raise statement:
def causeError():
    raise CustomException("This is a custom error message.")
When calling this function, the custom error message will be printed out.

Sometimes, you may want to add attributes to your custom exceptions to provide more information about the error. For example, if you're building a web server, you might define an HttpException class with attributes like status_code and message. Subclasses of HttpException, such as NotFoundHttpException or ServerError, can then inherit these attributes and provide specific error details.

Here's an example implementation:
class HttpException(Exception):
    def __init__(self, status_code=None, message=None):
        self.status_code = status_code
        self.message = message
        super().__init__(self.message)

class NotFoundHttpException(HttpException):
    def __init__(self):
        super().__init__(status_code=404, message="Resource not found.")

class ServerError(HttpException):
    def __init__(self):
        super().__init__(status_code=500, message="This server messed up!")

def raiseServerError():
    raise ServerError()

# Calling raiseServerError() will raise a ServerError with the appropriate status code and message.
Custom exception classes help keep your code organized and provide clear documentation about potential errors, their causes, and possible solutions. They also allow you to differentiate between expected errors and critical issues that require immediate attention.

## custom decorators not can 
Modify the arguments of a function.
Set up or tear down before and after a function runs.
Modify the return value of a function.

custom error classes
The name of the class can help users, They can extend any Python exception class, They can print messages in a stack trace.

## Fundamentals of Threads and Processes
Computers have both memory (short-term storage) and file storage (long-term storage), similar to our short-term and long-term memory. When we save a file, it goes into long-term storage, while declaring a variable in a program uses short-term memory in the processor.

The distinction matters because while different programs can access the same long-term storage, they can't access each other's short-term memory. The operating system allocates memory to each program and controls access to it, ensuring privacy between processes.

However, operating systems allow multiple pieces of code to run within the same process, sharing memory. This is achieved through threads. A process can have multiple threads executing code simultaneously, enabling parallelism. While we've been working in Python sequentially, in this chapter, we'll explore parallel computing using threads and processes.

## Multithreading
To get hands-on with threads in Python, we first import the threading and time modules. Then, we create a function called longSquare that calculates the square of a number but takes a long time to do it.

import threading
import time

def longSquare(n, results):
    time.sleep(1)  # Simulate a long calculation
    results[n] = n * n
Next, we demonstrate the power of threads by creating two threads to calculate the squares of numbers in parallel:


results = {}  # Dictionary to store results
t1 = threading.Thread(target=longSquare, args=(2, results))
t2 = threading.Thread(target=longSquare, args=(3, results))

t1.start()
t2.start()

t1.join()
t2.join()

print(results)  # Output: {2: 4, 3: 9}
However, we notice that we can't directly access the return value of the function from the threads. So, we modify the longSquare function to store the results in a shared dictionary:

def longSquare(n, results):
    time.sleep(1)  # Simulate a long calculation
    results[n] = n * n
Now, the results are accessible and can be printed:


print(results)  # Output: {2: 4, 3: 9}
To make it more efficient, we can use a list comprehension to create a list of threads and then start and join them:


threads = [threading.Thread(target=longSquare, args=(n, results)) for n in range(10)]

for t in threads:
    t.start()

for t in threads:
    t.join()

print(results)
This approach allows us to perform calculations in parallel, significantly reducing the overall execution time. We can even create 100 threads to further speed up the process.

## Multiprocessing
To explore multiprocessing in Python, we can start by using the `multiprocess` module, which is similar to the built-in `multiprocessing` module but doesn't have certain limitations, especially regarding function definition location.

First, we import the necessary modules:

from multiprocess import Process
import time
Then, we define a function `longSleep` that sleeps for a certain number of seconds:

def longSleep():
    time.sleep(1000)  # Sleep for 1000 seconds
    print("Finished computing")
Now, we can create and start multiple processes to run the `longSleep` function:


processes = [Process(target=longSleep) for _ in range(10)]
for p in processes:
    p.start()

for p in processes:
    p.join()
This will start 10 processes, each sleeping for 1000 seconds. However, since processes do not share memory, we can't access the results directly as we did with threads. Instead, we can print messages from within the function to indicate when the computation is finished.


def longSleep():
    time.sleep(1000)  # Sleep for 1000 seconds
    print("Finished computing")
This will print "Finished computing" from each process after it completes its sleep. However, the output may look a bit messy due to the asynchronous nature of multiprocessing.

A good way to collect output from multiple processes: writing the results to a file
processes; threads can contain multiple
Threads share the same space in memory
when the program has periods of "waiting" and doing nothing, multi-threading decrease the runtime of a program

## Opening, Reading and Writing
Working with files in Python involves some considerations, particularly when it comes to reading, writing, or appending data. Let's go through each operation:

### Reading Files:
To read a file in Python, you use the `open()` function, passing in the filename and the mode as arguments. The mode `'r'` signifies read mode.

```python
f = open('10_01_file.txt', 'r')
```

Once the file is opened, you can use methods like `readline()` or `readlines()` to retrieve the content of the file.

```python
line = f.readline()  # Reads one line at a time
lines = f.readlines()  # Reads all lines and returns a list of strings
```

### Writing Files:
To write to a file, you use `'w'` mode in the `open()` function. If the file doesn't exist, it will be created.
f = open('output.txt', 'w')

You can then use the `write()` method to write data to the file.
f.write('line 1\n')
f.write('line 2\n')

### Appending Files:
To append data to an existing file, you use `'a'` mode in the `open()` function.
f = open('output.txt', 'a')

Similar to writing, you can use the `write()` method to append data.
f.write('line 3\n')

Remember to close the file after you are done with it, using the `close()` method.
f.close()

When writing to files, Python buffers the data before actually writing it to the file. To ensure that all data is written to the file immediately, you can either close the file or use the `flush()` method.
f.flush()










