# Operators and variables

[Back to the outline](0_outline.md)

This section focuses on some fundamental Python ideas. Variables are the simplest way of storing information in a program, and operators are used for basic mathematical instructions. Python is capable of much more than basic mathematics, but one use of Python is as a calculator.

### Learning objectives

- [ ] I can use Python to perform simple calculations
- [ ] I understand what a variable is
- [ ] I can create variables and assign values to them

### Mathematical operators

Computers are very good at maths. They can solve complex conundrums in micro-seconds, and are invaluable for dealing with problems that are too difficult or tedious for people to want to solve.

In order to use Python to do calculations, we need to be familiar with Python's operators - the symbols which mean specific calculations. In `2 + 2`, the operator is '+', for addition.

The four main mathematical operators in Python are as follows:

* '+' for addition
* '-' for subtraction
* '\*' for multiplication
* '/' for division

There are other operators, but it's not necessary to know them yet. Feel free to experiment - try and work out what `9 % 2` does, or what `10**2` equals. How is '//' different from '/'?

Remember, if you want to actually see the result, you'll need to put your calculation inside a `print()` command.

### Variables

When programming, it's important to be able to store information, ideally with a memorable name. No one wants to have to type out the same long calculation multiple times, when we could just save the result somewhere. This is what variables are for.  

A variable is a named place to store a value that can change. A helpful analogy is to think of a variable as a box - it's worth whatever is inside it. If you put the value 4 inside a variable, then that variable has the value of 4 until you change it. You can then use the variable name in place of the number.

To create and assign a value to a variable in Python, you simply write the word you want to name your variable, the '=' symbol, and then the value.

`num = 34`

The above line of code sets the variable `num` equal to 34. Use `print(num)` to see the value of num.

Once the value is set, then you can use the variable.

`16 + num` is equal to 50.

You can re-assign the value of a variable as often as you want. You can even assign a variable to itself + 1 (or any other number).

`num = num + 1` increases the value of `num` by one.

That might look a bit confusing. To expand out what's happening, the computer is doing two things in one line. First, it gets the value of `num` and adds 1 to it. Next, it takes that new value and stores it in `num`.

`num = num * 2` doubles the value of the variable.

Variables can have almost any name you want, although there are rules about the characters you can use.

variable names must not:
* contain spaces
* consist solely of numbers
* contain punctuation such as '(' or '.'
* match 'keywords' (words that Python already assigns a meaning to), such as `print` or `for`.

Ideally, you should give variables relevant names: if you have a variable that stores the number of alligators you own, `numAlligators` is a better name than `flub`.

### Next steps

Take some time to experiment with operators and to make sure you understand variable assignment. The more comfortable you are with these ideas, the easier you'll find it to understand more complex Python.

When you are ready, move on to the [next section](4_data_types_and_logic.md)
