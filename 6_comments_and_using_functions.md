# Comments and using functions

[Back to the outline](0_outline.md)

So far, we have explored lots of concepts in Python, but not very much that allows you to actually instruct the computer. In this section, we will look at functions, a powerful way of giving instructions that can accomplish almost anything.

### Learning objectives

- [ ] I can add comments to my code
- [ ] I can use a range of Python functions
- [ ] I can pass arguments to functions

### Comments

Even simple programs can be hard to understand, particularly if you didn't write them yourself, or even if you did write the code, but a while ago. Comments let you add explanations and useful notes to your code, so that someone else (or you, six months later) can easily work out what the code does and why it works that way.

Comments are ignored by the computer when running code - they aren't a part of the actual program, even when they are written in the same file.

In Python, comments are started by the `#` character. Anything that comes after the `#`, on the same line, counts as a comment and will not be executed as code.

```
# Combines three strings together and stores the result in a variable
new_string = "Comments" + " are " + "useful."
```

You don't need to comment every single line, and you don't need to comment things that are obvious. `num = 2 + 2 # Adds 2 and 2 to get 4` is not a useful comment. Use comments when it isn't obvious from the code itself what is going on. If you have given specific & relevant names to your [variables](3_operators_and_variables.md), then someone reading your code won't need as much help to understand it.

Writing comments might seem tedious, but they're very useful. Comments make code more maintainable, so that you can easily update or reuse programs instead of having to start from scratch every time.

### Using functions

A function is a named, repeatable, set of instructions. Once a function has been created - "defined" - then it can be used - "called" or "executed" - as many times as you want.

To call a function, you need to use its name, followed by brackets. You have already used the `print` function.

`print()`

The brackets tell Python that the function is an instruction, and should be executed. Without the brackets, nothing happens.

Most functions also need to be given information when they are called. Each piece of information that you pass to a function when you call it is referred to as an 'argument'.

Function arguments go inside the brackets. If there is more than one argument, they are separated by commas.

`print("Hello World!")`

The print function simply displays a value to the user. In the above case, it would display the string "Hello World!".

Some functions simply perform an action, while others **return** a value. Function calls that return a value can be assigned to variables as though they were the value itself.

In the next example, the function `round` is used. This rounds a number to the nearest integer and returns a value.

```
num = round(3.71)
```

In the above example, the value of `num` is 4, as that is the value the function returns. Note the brackets - if they are missing, the function does not run, and so no new value is returned. `num` just becomes a copy of the function.

Further on in this module, we will discuss writing your own functions, but Python comes with some functions already built in. The following is a brief, non-exhaustive list of built-in functions that you can use:

* `print(x)` - displays x to the user. x should be a number/string
* `len(x)` - returns the length of x. x should be a list/string
* `max(x)` - returns the largest value in x, if x is a list of numbers
* `min(x)` - returns the smallest element in x, if x is a list of numbers
* `str(x)` - takes a number as x, returns x as a strings
* `int(x)` - takes a string/float as x, returns x as an integer
* `sorted(x)` - takes a list as x, returns x sorted in ascending order
* `input()` - waits for input from the user and returns it as a string.

The above explanations are slightly simplified - `len`, for example, can be used on more than strings and lists - it works on anything that is a group of items/values, but don't worry about other types of group for now.

Functions take different numbers of arguments - it depends on what they do, and what information they need to complete their task. If you pass too many or too few arguments to a function, an error will occur. You also need to make sure that arguments come in the right order. For a built-in function, check the [documentation](https://docs.python.org/3/) to find out what arguments are expected.

### Next steps

This has only been a very brief introduction to functions; it's a complex topic, and there is lots more to learn. Don't be discouraged if you still have questions - what's important for now is that you recognise what a function call looks like, and understand how to pass arguments to a function.

We will return to functions in a later section, and it's worth doing experimenting/reading further about them. When you want to move on, head to the [next section](7_importing.md).
