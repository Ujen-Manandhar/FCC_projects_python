# FCC_projects_python
These Projects are projects done in free code camp for learning python.
---
## 1. [Ceaser Cipher](https://github.com/Ujen-Manandhar/FCC_projects_python/blob/main/1.%20Ceaser_cipher.ipynb)[^1]<br/>
The Ceaser Cipher project helped me take a grasp of `for loops`, `if...else` statement, `function`, and the `.find` method and indexing. <br/> 
The Cipher is simple project which takes in the user input and shifts the letters in order to create a chiper text<br/>

## 2. [Vigenère cipher](https://github.com/Ujen-Manandhar/FCC_projects_python/blob/main/2.%20Vigen%C3%A8re%20cipher.ipynb)[^1]
The Vigenère cipher project hepled in taking a grasp of the indexing in python, along with getting a grasp of functional programming. <br/>
This project also helped me identify innovative way of using modulo operator`%` to wrap numbers around a string; to wrap around a text let’s say if the text is to be repeated then the second text is small or is an end we can use the modulo operator `%` to wrap around the text.

## 3. [Luhn Algorithm](https://github.com/Ujen-Manandhar/FCC_projects_python/blob/main/3.%20Luhn_algo.ipynb)[^1]
The Luhn Algorithm is widely used for error-checking in various applications, such as verifying credit card numbers.<br/>
In this project `string slicing [::]` along with method `replace`, `str.maketrans` and `translate` were understood, The project also helped in grasping the concept of using quotient`//` and modulus`%` to identify the first and second digit.<br/>
```
my_number = 12
first_digit = my_number // 10
second_digit = my_number % 10
# here the first digit is one and the second digit is two.
```
## 4. [Expense_tracker](https://github.com/Ujen-Manandhar/FCC_projects_python/blob/main/4.%20Expense_tracker.ipynb)[^1]
The Expense_tracker helped be grasp a level of fuctional programming ie make different function in order to acomplish an overall problem. This intuitive way helped me break the overall problem into functional bits (or parts) and to one extent not write repetitive code.<br/>
This project also introduced me with `lambda function` with using `map` and `filter` expression to write more efficient and powerful code.<br/>
    -`lambda function` unlike function in python are used to write more brief, anonymous functions in Python, ideal for simple, one-time tasks.<br/>
    - `map function` map fuction takes in two arguments `map(func, iterable)` in each iteration the map function passes the `iterable` to the `func` and returns a iterable object.<br/>
    -`filter function` similar two the map function the `filter function` takes in two arguments `filter(func, iterable)` and where `map function` in case for equality returs `True` filter function returs the value as an iterable object.<br/>

```
expenses = [{'amount': 1000, 'category': 'coke'},{'amount': 2000, 'category': 'Fanta'}, {'amount': 1000, 'category': 'coke'}]
category = coke
filter(lambda expenses : expenses['category'] == category, expenses)
    >>[{'amount': 1000, 'category': 'coke'}, {'amount': 1000, 'category': 'coke'}]
map(lambda expenses : expenses['amount'], expenses)
    >> [True, False, True]
```
## [snake_case_converter]()[^1]
The snake case converter is a simple program that converts PascalCase and camelCase into snake_case. The first approch of solving uses a simple function where the char is taken and then uses `.isupper()` method of string to check if the charcter is upper then in the list append the `_ + letter.lower()` in order add space to the different cases as both cases follow capital letter in case of spaces. Then after all the letter are appended, The `.join(lst)` method is called to join the string in the list and also`.strip('_')` method to strip `_` at the beginning and at the end of the text.<br/>
<br/>
For the second part of the program rather then writing long program. List comprehension was used a list comprehension is a construct that allows you to generate a new list by applying an expression to each item in an existing iterable and optionally filtering items with a condition. Apart from being briefer, list comprehensions often run faster.<br/>

```
lst = [i * 2 for i in iterable]
```
### References
[^1]: https://www.freecodecamp.org/learn/scientific-computing-with-python/
