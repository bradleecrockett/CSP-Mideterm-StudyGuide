# AP CSP Midterm Study Guide

## Digital information

### Number Conversions

| Decimal (Base 10) | Binary (base 2) | Hexadecimal (base 16) |
|:-----:|:-----:|:---:|
| 23 |  |  |  
|  | 0b1001110 |  |  
|  |  | 0x2B |  
| 100 |  |  |  
|  | 0b00001110 |  |  
|  |  | 0xA1 |  

### Representing items
1) How many distinct items can be represented with 4 bis?
1) How many distinct items can be represented with 5 bits?
1) Describe what an overflow error is.
1) Describe what a roundoff error is.
1) Describe what round off error has to do with floating point comparisons in python.
    1) For example `print(5 / 3 == 1 + 2 / 3)`


### Digital Representation
1) ASCII - What is the following message?
0x41 0x63 0x65 0x20 0b01110100 0b01101000 0b01100101 0b00100000 109 105 100 116 101 114 109
![ASCII Table](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/ASCII-Table-wide.svg/800px-ASCII-Table-wide.svg.png)

1) Compare and contrast analog and digital data.
1) Describe what sampling is.
1) Compare and contrast lossy and lossless compression.

### Intellectual Property

1) Describe what Copyright is.
1) Describe what Fair Use is.


## Python

* `print()`
* math - `*`, `/`, `%`, `+`, `-`, `**`, `//`, `abs()`, `+=` 
* `input()` - when to cast and when not to cast
* Data types - strings, ints, floats, booleans
* Conditional statements - `if` `elif` `else`
* Boolean expressions and operations - `and`, `or`, `not` 


|x | y | x and y | x or y | not (x and y) | not(x or y) | not x and not y | not x or not y |
|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|:-----:|
|True | True | | | | |
|False | False | | | | |
|True | False | | | | |
|False | True | | | | | 

* For Loops
    * `range(number)`
* While Loops
    * Break and Continue Loop and a Half structure
* Strings
    * Indexing
    * Slicing [start_index : end_index] Remember that the end_index not included in the slice
    * `len()`
    * The `in` keyword
    * String methods like `.upper()` and `.lower()`
* The accumulator algorithm
````python
# Accumulate a number
# init a counter
count = 0
# start a loop
for i in range(15, 30, 3):  #15, 18, 21, 24, 27
    # cond. statement for when to count up
    if i % 2 == 1:
        count += 1

print("What happened", count, " times?")

# Accumulate a string
# init an empty str
vowels = ""
letter = ""
while not(letter == 'quit'):
    letter = input("Enter a letter, Enter 'quit' to quit: ")
    if letter in 'aeiou':
        print("That's a vowel!")
        vowels += letter
    else:
        print("Not a vowel")
print("Vowels entered were:", vowels)

````
    

