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
    - `map function` map fuction takes in two arguments `map(func, iterable)` in each iteration the map function passes the `iterable` to the `func` and returns a iterable object. Map function is used to transform the return value.<br/>
    -`filter function` similar two the map function the `filter function` takes in two arguments `filter(func, iterable)` and where `map function` in case for equality returs `True` filter function returs the value as an iterable object. Here the `filter function` dosen't transforn the retrun value and stores the orginal value in a return filter object while `mapfunction` transforms the return value and dosen't filter the value.<br/>

```
expenses = [{'amount': 1000, 'category': 'coke'},{'amount': 2000, 'category': 'Fanta'}, {'amount': 1000, 'category': 'coke'}]
category = coke
filter(lambda expenses : expenses['category'] == category, expenses)
    >>[{'amount': 1000, 'category': 'coke'}, {'amount': 1000, 'category': 'coke'}]
map(lambda expenses : expenses['amount'] == category, expenses)
    >> [True, False, True]
```
## 5. [snake_case_converter](https://github.com/Ujen-Manandhar/FCC_projects_python/blob/main/5.%20snake_case_converter.ipynb)[^1]
The snake case converter is a simple program that converts PascalCase and camelCase into snake_case. The first approch of solving uses a simple function where the char is taken and then uses `.isupper()` method of string to check if the charcter is upper then in the list append the `_ + letter.lower()` in order add space to the different cases as both cases follow capital letter in case of spaces. Then after all the letter are appended, The `.join(lst)` method is called to join the string in the list and also`.strip('_')` method to strip `_` at the beginning and at the end of the text.<br/>
<br/>
For the second part of the program rather then writing long program. List comprehension was used a list comprehension is a construct that allows you to generate a new list by applying an expression to each item in an existing iterable and optionally filtering items with a condition. Apart from being briefer, list comprehensions often run faster.<br/>

```
lst = [i * 2 for i in iterable]
```
## 6. [Bisection_method](https://github.com/Ujen-Manandhar/FCC_projects_python/blob/main/6.%20Bisection_method.ipynb)[^1]
Bisection Method is a numerical method of finding square root of number. The program takes in 3 argument where the two argument `tolerance` and `max_iterations` have a default value ie when an argument have default value associated with the argument. The `tolerance` argument also uses a scientific notation to indicate `0.0000001`or `1 x 10^-7` used to check the error of the computation.<br/>
<br/>
Writing the program also introduced me with a new fuction in python `max()` which returns the higgest value of the number or string. And th `abs()` which acts as absolute value to check with the tolerance level. Also a `count_it` was used to identify the number of iterations it took to identify the square root.<br/>
<br/>
The program also introduce a convention of using `_` in a for loop if the variable of the loop ins't being used.<br/>

## 8. [Password Generator](https://github.com/Ujen-Manandhar/FCC_projects_python/blob/main/08.1. Password generator.ipynb)[^1]
The project focuses upon making a password generator with regular expression to match pattern of the requirements of the password and make the password completely random. The library used in the programs were
1. secrets: The secrets module ensure the most secure source of randomness based on the OS can provide, the random module wasn't used because due to the pseudo-random numbers being predictable.
2. strings: The stirng library was used to get the letters, digits, symbols and no white space for the password.
3. re(regex): The re library was used for matching purposes. The regex expression was used to check if the password generated had the minium requirement need as specified.<br/>


The `for loop` used also focuses upon convention of using `_` if the variable of the loop isn't being used.<br/>
<br/>
Regex uses strings to search the character as sometimes python escape characer is needed as such we use `r` in front of the string to convert the string passed in as `r'[a-z]'` a raw string to ignore escape characters and it is a good idea to write regex with raw strings.<br/>
<br/>
Then using the constraints list and tuple unpacking we check using a generator expression and `all()` function to check if all the constraints are true then print or return the password. The generator expression is more preferable as we don't need the list to be stored it is not need to be stored in memory so using a generator expression is more memory efficient.<br/>
<br/>
Generator expressions follow the syntax of list comprehensions but they use parentheses instead of square brackets.<br/>
<br/>
`all() is a built-in Python function that returns True if all the elements inside a given iterable evaluate to True.`
<br/>
`generator_expression = (len(re.findall(pattern, password)) >= constraint for constraint , pattern in constraints)`




### References
[^1]: https://www.freecodecamp.org/learn/scientific-computing-with-python/
