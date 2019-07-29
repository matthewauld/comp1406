# Assignment 4

## Due  <span style="color:red">Wednesday, August 7th</span> at <span style="color:red">5:30pm</span>

---

Submit a single file called `assignment4.zip` to the submission server

http://134.117.26.180:9091

Your zip file must contain a directory called `comp1406a4` and all of your  `.java` files must be in this directory. Do not include your `.class` files.


---


# 1. Balanced Parentheses [30 marks]

A stack is a data structure where data is accessed using the LIFO (last in first out) principle.  In this problem, you will use a stack to check whether a string has balanced 
parentheses `(`, `)` and brackets `{`, `}`, `[`, `]`, or not. 

A string that has balanced parentheses and brackets will be said to be __balanced__. Any character that is __not__ one of `(`, `)`, `[`, `]`, `{`, or `}` is not important when deciding if
a string is balanced and can be ignored. 

We will define balanced as follows. A string `str` is balanced

- if `str` does not contain a parenthesis or bracket symbol
- if `str` consists of a balanced string surrounded by opening and closing parentheses or matching brackets. That is, `str` is `(b)`, `{b}` or `[b]`, where `b` is any balanced string, or
- if `str` is the concatenation of any two balanced strings. That is, 
`str` is `bc`, where `b` and `c` are any balanced strings. Example: `(){}`


You will complete the provided `Balanced` class that has two 
static methods `isBalanced(String)` and `numberOfBalancedStrings(String[])`.  


Your `isBalanced` method must use the `java.util.Stack` class (in a way that solves the problem) to receive any grades
for this problem.  


[http://docs.oracle.com/javase/8/docs/api/java/util/Stack.html](http://docs.oracle.com/javase/8/docs/api/java/util/Stack.html)


## Examples

The following strings have balanced parentheses
- `()`, `()()`
- `cat`, `c(at)`, `(hello)(kitty)`
- `if( ((x-y) < 4) || (x > 12))`
- `()(((s)))()()()()(x()((y))(x))()(ccccc(w))ssss()`

The following strings do __not__ have balances parentheses

- `)`, `)(a)`, `)a(`


The following strings have balanced parentheses and brackets

- `a`, `[]`, `{}`, `[()]`, `[]{}({[{}]})`, 
- `for(int i=0; i<12; i+=1){x[i]+=f(1);}`


The following strings do __not__ have balanced parentheses and brackets
- `(]`, `{)`, `[}`, `[}`, `(]`, `({)}`h, `[(]())`
- `for(int i=0; i<12; i+=1){`

Note: You will receive partial marks if you code only works for parentheses (and not brackets).

# 2. Linked Lists [40 marks]

Create a concrete `LinkedList` class that extends the provided `ALinkedList` class. You will need to override the `extract()` method in your class. You can use your `main()` method for testing your method (although you do not need to provide a main method).

Recall that a list is an ordered collection of data
```
X_0, X_1, X_2, ..., X_n-1
```

The `extract(int start, int end)` method removes all elements
``` 
X_start, X_start_1, ..., X_end-1
```
from the list. It also returns all removed elements as a new list (`LinkedList`) that retains the same ordering.

For example, if the initial list called `animals` was
```
cat, dog, eel, cow, owl, pig, pip
```
then `animals.extract(1,5)` would return the new list
```
dog, eel, cow, owl
```
and `animals` would now be the list
```
cat, pig, pip
```

The `AlinkedList` class also has a `sort()` method that currently does nothing. Complete this method so that it sorts the current linked list (alphabetically). 

For example, if there was a list called `kids` that consisted of
```java
puppy, kitten, cub, leveret, kit, cygnet
```
then after calling `kids.sort()`, the list would now be
```java
cub, cygnet, kit, kitten, leveret, puppy
```
Don't worry about efficiency. Linked lists are not a great data structure if you need to sort the list. The sort method is worth 10 marks (so 10% of the assignment).


# 3. Draw a Picture [30 marks]

Draw a picture.

Think about your experience so far in COMP1006/1406. 
Your task in this problem is to draw a picture that expresses this reflection.

My hope	in asking you to draw a picture is that you will critically reflect on the material and challenges you have seen in this course so far. It should also make this assignment a bit lighter than the others. The intention is that this problem should not cause you stress. Do not worry about your
_artistic ability_. You will not be graded on that at all. Have fun.

Your submission should be in PDF format (if you prefer to hand in a physical copy then contact me and we will make arrangements for this). Ideally, the size of your drawing should be a standard letter size in horizontal orientation. If you submit your picture in a file called `Public.pdf` then you agree to have your picture 
shown to the class. If you prefer that your picture not be shown then submit it in a file called `Private.pdf`.

Note: Offensive/rude/insensitive 
submissions will receive zero marks and may be forwarded to the Dean's office depending on the severity.
(This has never happened before and I trust it will not now.)

# Submission Recap

A complete assignment will consist of a single file `comp1406a4.zip` that has a single folder/directory called `comp1406a4`. The `comp1406a4` folder will have the following three files included:

```java
Balanced.java
LinkedList.java
Public.pdf or Private.pdf
```

All classes must be in the `comp1406a4` package. That is, all files must have the `package comp1406a4;` directive as the first line. Your code will NOT compile if it does not have this and you will receive zero correctness marks if your code does not compile.
