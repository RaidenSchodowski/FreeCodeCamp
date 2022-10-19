# Basics

1. **Reserved Words** = words you cannot use as variable names
```
False, None, True, and, as, assert, break, class, if, def, del, elif, else, except, 
return, for, from, global, try, import, in, is, lambda, while, not, or, pass, raise, 
finally, continue, nonlocal, with, yield.
```
2. **Constants** = fixed values, do not change. Numbers, letters, or strings. String constants use single or double quotes(',")
3. **Variables** = a name placed in memory to store and retrieve data. All variables must start with a letter or underscrore (but starting with an underscore is a bad idea). After the first letter varioables can have letters, numbers, or underscores. They are case sensitive, but differentiating with only difference is capitalization is confusing. 
4. **Numeric Expressions**
```
+ Addition, - Subtraction, * Multiplication, / Division, 
** Power, % Remainder, = assigns variable
```
```
< less than, <= less than or equal to, > greater than, 
== equal to, != not equal
```
5. **Type**: intiger(int), float, string(str), Boolean, or none. Can only combine things of the same type. You can ask python which type a variable is. You can convert between different types. Divition will always result in a floating type. 
6. **Indentation**: very important for if/while statements. You will get an error if the indentation is not correct. You cannot replace tabs for spaces. There is no 'end' command as in Matlab, so the indentation is how Python knows to exit a loop
7. **Try/except Structure** = If you know there is a line of code which will most likely give back an error, sorround it in a try/except loop. If the try works, except is skipped. If try fails, except is run. Normally the error would stop the entie code, but this allows the rest of the code to continue running. 
8. **Functions**: Coders dont like to retype the same thing twice. This is for ease of debugging or changing. If you find something wrong in one place you now need to go find it 10 more times unless it is saved as a function. `def` creates, names, and records the function. To run the code you later call it by name(). It is best practice to output functions with return() command instead of print().
9. [Built in functions](https://docs.python.org/3/library/functions.html)
10. **Arguments** = value passed into the function as an input when you call the function
11. **Parameters** = a variable used in the function definition
12. **Pyhon operators**: 
```
break = stops the exicution of a loop (for or while)
return = stops the exicution of a function and speecifies output
continue = ends the current iteration and jumps to the top of the loop
in = cycles through each of the variable in a set, useful in for loops
is = logical operator. Similar to the '==' but stronger since it requires the variables 
to be the same type. Ex: 0==0.0 is true but 0 is 0.0 is false.
is not = logical operator. Opposite of the is operator.
```
13. **Loops** = Make sure to avoid infinite loops, they will drain all processing power. You can break out of them with 'break' command. While loops are indefinite, for loops are definite.
14. **Boolean Variables** = the variables True and False only. Starts at False and is set to True once we find what we are looking for.
15. **None type** = only has one variable (empty, NA, nothing). It is a placeholder.
16. **Strings**: are indexed with a starting value of 0 (Ex: banana would be assigned 012345)
17. **Spicing Strings**: variable[0:4] would be from the first letter to the third since it is 'up to but not including 4'. If the variable is only 2 letters long it will still accept 4 as an input, it'll just truncate it where it ends. 
18. **String Library**: special functions for interfacing with string types. If you have a string named x, the command dir(x) will show all strings interface commands able to be used. [Link](https://docs.python.org/3/library/stdtypes.html#string-methods)
19. **Files** 
```
x = open(filename,mode) reads the file and assigns to variable x. filename must include .txt 
extension and is a 'string'
Mode = r if reading the file, w if writing to the file. This is optional
```
21. **New line**: \n character. It is hidden in most cases but must be included in your count so remember it is there. 
22. **Collection**: Allows you to put many values in a single variable
23. **Mutable** = changable. Lists are mutable, strings are not. 
24. **Range** = returns a list of numbers that range from zero to one less then the parameter it is set to 
25. [List functions](http://docs.python.org/tutorial/datastructures.html)
26. **Append** = adding elements to the end of an existing list 
27. **Dictionaries** = A type of collection. A "bag" of values, each with its own label. Everything has a key, but there is no order. Lists stay in order and you can retrieve them by number. They are Pythons most powerful data collection. 
28. **List Comprehension**: Pythons ability to generate a list instead of be given the list values directly. 
29. **Expressions** = searching for information, very old very well used. Must initieate it by using `import.re` at the beginnging. `re.search()` checks if a string matchs a regular expression like the find command, returns true/false only. `re.findall`extracts portions of a string that match the regular expression.
```
^        Matches the beginning of a line
$        Matches the end of the line
.        Matches any character
\s       Matches whitespace
\S       Matches any non-whitespace character
*        Repeats a character zero or more times
*?       Repeats a character zero or more times (non-greedy)
+        Repeats a character one or more times
+?       Repeats a character one or more times (non-greedy)
[aeiou]  Matches a single character in the listed set
[^XYZ]   Matches a single character not in the listed set
[a-z0-9] The set of characters can include a range
(        Indicates where string extraction is to start
)        Indicates where string extraction is to end
```
