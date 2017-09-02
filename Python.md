# Python

## Reverse

`astring = "Hello world!"
print(astring[::-1])`

## Upper and Lower Cases

`astring = "Hello world!"
print(astring.upper())
print(astring.lower())`

## Boolean check
`astring = "Hello world!"
print(astring.startswith("Hello"))
print(astring.endswith("asdfasdfasdf"))`

## Splitting
`astring = "Hello world!"
afewwords = astring.split(" ")
print(afewwords)`

## Boolean Operators
`
name = "John"
age = 23
if name == "John" and age == 23:
    print("Your name is John, and you are also 23 years old.")`

`if name == "John" or name == "Rick":
    print("Your name is either John or Rick.")`

## The "in" Operator
`name = "John"
if name in ["John", "Rick"]:
    print("Your name is either John or Rick.")`

## The 'is' operator
Unlike the double equals operator "==", the "is" operator does not match the values of the variables, but the instances themselves. For example:

`x = [1,2,3]
y = [1,2,3]
print(x == y) # Prints out True
print(x is y) # Prints out False`

