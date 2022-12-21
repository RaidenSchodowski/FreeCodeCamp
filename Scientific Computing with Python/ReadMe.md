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
is = logical operator. Similar to the '==' but stronger since it requires the 
variables to be the same type. Ex: 0==0.0 is true but 0 is 0.0 is false.
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
x = open(filename,mode) reads the file and assigns to variable x. filename must 
include .txt extension and is a 'string'
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
30. **Transport Control Protocol (TCP)** = Built ontop of internet protocol, it handles the communication between to computers (aka, two sockets). **Port Numbers** are the "numbers" you dile to reach specific ports/sockets. The **Application Protocol** is what to do with that connection once it is established. 
31. *HTTP*: Hypertext transfer protocol, one of the application protocols to use once you have a socket connection. Of the format `http://www.name.com/page.htm` which is `protocol-host-document`. Goverened by the internet standards: RFCs. By using the command line to use these protocols you can "hack" them which is how actual hackers work.
32. **Text Processing** = Assigns a number (0-256) to every single character and is then stored in 8 bits of memory as a byte. `ord()` returns that numeric number. But in the US we use the ASCII which only includes basic latin alphabet, nothing for many other languages. Now use [unicode](http://unicode.org/charts) instead. UTF-8 is the best practice for compression and sending this unicode over the internet. 
33. **Web Scraping** = when a program pretends to be a browser and retrieves web pages, looks at them, extracts information, and then looks at more web pages. With enough time it should be able to find every single webpage that has other webpages linking to it. Allows you to retrieve information from a page that has no "export capability", monitor a site for new information, make a database for a search engine, etc. Some sites will ban you for doing this. [link](http://en.wikipedia.org/wiki/Web_scraping), and [link](http://en.wikipedia.org/wiki/Web_crawler). 
34. **BeautifulSoup**: a program for web scraping that makes it sooo much easier. Must be installed. [Link](https://www.crummy.com/software/BeautifulSoup/)
35. **eXtensible Markup Language**: help information systems share structures data
```
Tags          indicate the beginning and ending of elements
Attributes    keyword/value pairs on the opening tag of XML
Serialize     Convert data in one program into a common format that can be 
              stored/transmitted
XML Format    Every start tag neesd an end tag
```
36. **XML Schema**: description of legal format of XML document to specify a "contract" between systems. XML and XML Schema are both passed through a validator to make sure it is legal. [link](http://en.wikipedia.org/wiki/Xml_schema)
37. **JSON**: Better for pulling data and moving it, as opposed to XML is better for heirarchical structure. Born from Javascript. Not an international standard. [Link](https://www.json.org/json-en.html). Returns everything as a dictionary or list depending on how you format it. Retrieval request is written in one large string. 
38. **Service Oriented Approach**: for dealing with information that is spread across multiple locations. [explinations]
39. **API**: Application Program Interface = documentation for different websites that lays out the rules of how to use it. 
40. **Objects**: instead of being the whole program - each object is a little "island" within the program and cooperatively works together. Approach is to break the problem into smaller understandable parts. Have boundaries that allow us to ignore un-needed detail. 
41. **Class** = a template or key for an object you are going to make. A more abstract concept. 
42. **Method** = function that lives inside of the class / a defined capability of a class
43. **Field or attribute** = a bit of data in a class 
44. **Object/Instance** = a particular instance of a class. Many objects from one class
45. **Object Lifestyle**  = act of creating (constructor) and destroying (destructor) objects. Constructors are used more more often than destructors. Constructurs set up initial variables, etc. 
46. **Inheritance** = instead of making a new class from scratch we are startig from an existing class, branching off of it essentially. Creates object heirarchies. Called Parent-Child relationships or subclassing
47. **Database* = contains many tables
48. **Relation/table** = contains tuples and attributes
49. **Tuple/row** = a set of fields that generally represents an object like a person or a music track
50. **Attribute/column** = one of possibly many elements of data corresponding to the object represented by the row
51. **SQL** = structures query language is the language we use to issue commands to the data base. creates a table, retrieve some data, insert data, delete data, etc.
```
Common database systems:
Oracle    Large, commercial, enterprise-scale, very tweakable
MySql     Simpler but very fast and scalable - commercial open source 
Sqlserver Very nice, from microsoft
HSQL, SQLite, Postgress, etc are all smaller projects that are free and open source
```
52. [SQL code](https://www.py4e.com/lectures3/Pythonlearn-15-Database-Handout.txt)
 
