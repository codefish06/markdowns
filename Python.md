# Python

## Reverse

```
astring = "Hello world!"
print(astring[::-1])`
```
## Upper and Lower Cases

```
astring = "Hello world!"
print(astring.upper())
print(astring.lower())`
```

## Boolean check
```
astring = "Hello world!"
print(astring.startswith("Hello"))
print(astring.endswith("asdfasdfasdf"))`
```

## Splitting
```
astring = "Hello world!"
afewwords = astring.split(" ")
print(afewwords)
```

## Boolean Operators

```
name = "John"
age = 23
if name == "John" and age == 23:
    print("Your name is John, and you are also 23 years old.")`

`if name == "John" or name == "Rick":
    print("Your name is either John or Rick.")
```

## The "in" Operator
```
name = "John"
if name in ["John", "Rick"]:
    print("Your name is either John or Rick.")
```

## The 'is' operator
Unlike the double equals operator "==", the "is" operator does not match the values of the variables, but the instances themselves. For example:

```
x = [1,2,3]
y = [1,2,3]
print(x == y) # Prints out True
print(x is y) # Prints out False
```

## Looping

### For-loop
```
primes = [2, 3, 5, 7]
for prime in primes:
    print(prime)`
```

### Range
Starting fom 0 onwards:

```
# Prints out the numbers 0,1,2,3,4
for x in range(5):
    print(x)`

Limited from and to

# Prints out 3,4,5
for x in range(3, 6):
    print(x)`

Limited and Gap

# Prints out 3,5,7
for x in range(3, 8, 2):
    print(x)
```

### "While" Loops
While loops repeat as long as a certain boolean condition is met. For example:

```
count = 0
while count < 5:
    print(count)
    count += 1  # This is the same as count = count + 1
```

### "break" and "continue" statements
break is used to exit a for loop or a while loop, whereas continue is used to skip the current block, and return to the "for" or "while" statement. A few examples:

```
count = 0
while True:
    print(count)
    count += 1
    if count >= 5:
        break`

`for x in range(10):
    # Check if x is even
    if x % 2 == 0:
        continue
    print(x)`
```

## Functions
```
def my_function():
    print("Hello From My Function!")`

`def my_function_with_args(username, greeting):
    print("Hello, %s , From My Function!, I wish you %s"%(username, greeting))
```

## Classes and Objects
Objects are an encapsulation of variables and functions into a single entity. Objects get their variables and functions from classes. Classes are essentially a template to create your objects.

```
class MyClass:
    variable = "blah"

    def function(self):
        print("This is a message inside the class.")

myobjectx = MyClass()
```

## Dictionaries
A dictionary is a data type similar to arrays, but works with keys and values instead of indexes. Each value stored in a dictionary can be accessed using a key, which is any type of object (a string, a number, a list, etc.) instead of using its index to address it.

```
phonebook = {}
phonebook["John"] = 938477566
phonebook["Jack"] = 938377264
phonebook["Jill"] = 947662781
print(phonebook)
```

Alternatively, a dictionary can be initialized with the same values in the following notation:

```
phonebook = {
    "John" : 938477566,
    "Jack" : 938377264,
    "Jill" : 947662781
}
print(phonebook)
```

### Iterating over dictionaries
Dictionaries can be iterated over, just like a list. However, a dictionary, unlike a list, does not keep the order of the values stored in it. To iterate over key value pairs, use the following syntax:

```
phonebook = {"John" : 938477566,"Jack" : 938377264,"Jill" : 947662781}
for name, number in phonebook.items():
    print("Phone number of %s is %d" % (name, number))
```

### Removing a value
To remove a specified index, use either one of the following notations:

```
phonebook = {
   "John" : 938477566,
   "Jack" : 938377264,
   "Jill" : 947662781
}
del phonebook["John"]
print(phonebook)
```

## Modules and Packages

## Numpy Arrays

### Getting Started
Numpy arrays are great alternatives to Python Lists. Some of the key advantages of Numpy arrays are that they are fast, easy to work with, and give users the opportunity to perform calculations across entire arrays.

In the following example, you will first create two Python lists. Then, you will import the numpy package and create numpy arrays out of the newly created lists.

```height = [1.87,  1.87, 1.82, 1.91, 1.90, 1.85]
weight = [81.65, 97.52, 95.25, 92.98, 86.18, 88.45`

import numpy as np

np_height = np.array(height)
np_weight = np.array(weight)
```

