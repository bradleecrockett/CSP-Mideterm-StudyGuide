# AP CSP Midterm Study Guide

## Digital information

### Number Conversions

| Decimal (Base 10) | Binary (base 2) | Hexadecimal (base 16) |
|:-----:|:-----:|:---:|
| 23 |  |  |  
|  | 0b01001110 |  |  
|  |  | 0x2B |  
| 100 |  |  |  
|  | 0b00001110 |  |  
|  |  | 0xA1 |  

### Representing items
1) How many distinct items can be represented with 4 bits?
1) How many distinct items can be represented with 5 bits?
1) Describe what an overflow error is.
1) Describe what a round off error is.
1) Describe what round off error has to do with floating point comparisons in python.
    1) For example `print(5 / 3 == 1 + 2 / 3)`


### Digital Representation
1) ASCII - What is the following message?

    `0x41 0x63 0x65 0x20 0b01110100 0b01101000 0b01100101 0b00100000 109 105 100 116 101 114 109`

![ASCII Table](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/ASCII-Table-wide.svg/800px-ASCII-Table-wide.svg.png)

1) Compare and contrast analog and digital data.
1) Describe what sampling is.
1) Compare and contrast lossy and lossless compression.

### Intellectual Property

1) Describe what Copyright is.
1) Describe what Fair Use is.

### Need Practice?
* [Changing Bits](https://codehs.com/editor/381129/155141/2639/1780)
* [Bits](https://codehs.com/editor/381106/155141/2639/1780)
* [Encoding Data](https://codehs.com/editor/381139/155141/2639/1780)
* [Data Compression](https://codehs.com/quiz/384494/155141/2639/1780?)


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
```python
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

```

* Lists
    * Indexing
    * Slicing
    * Methods: These manipulate lists and can change the values contained within a list. They use the dor operator.    
        * `append(element)`, `sort()`, `index(element)`, `insert(index, element)`, `remove(element)`
    * Functions: These functions **do not** use the dot operator, rather, you pass a list as a parameter into the function. The function then returns a value (or list of values). This does not modify the original list.
        *  `max(list)`, `min(list)`, `sorted(list)`

### Need practice
Look through the CodeHS python quizzes or the following AP Style questions. Note that there are  some differences between the AP Language and the Python language some are outlined in the table below.
* [Boolean Expressions](https://codehs.com/quiz/381077/155141/2639/1780?)
* [Algorithms](https://codehs.com/editor/381003/155141/2639/1780)
* [Missing Code](https://codehs.com/editor/381014/155141/2639/1780)
* [For Loops](https://codehs.com/editor/381087/155141/2639/1780)
* [While Loops](https://codehs.com/editor/381051/155141/2639/1780)
    
| Python | AP Language | Notes |
|:-----:|:-----:|:-----:|
|`print()` | DISPLAY() | The AP language does not move to the next line.|
|`x = 8` | x <- 8 | The assignment operator is a left facing arrow. |
|`num == 7` | num = 7 | Check for equality is a single equal sing in the AP language.|
|`for i in range(5)` | REPEAT 5 Times | The AP Language uses a repeat instead of a `for` loop. |


