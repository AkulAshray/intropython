# Writing functions

[Back to the outline](0_outline.md)

We've already used functions like `print()`, `input()` and `max()`; now it's time to learn how to write your own functions.

### Learning objectives

- [ ] I can write functions
- [ ] I understand how to use the `return` keyword
- [ ] I can create functions with parameters

### Functions

To [review](6_comments_and_using_functions.md), a function is a **named**, **repeatable** block of code. Functions are called by name, and can have information passed to them when they are called. Some functions `return` a value, and some don't.  

### Why use functions

One of the guidelines that you should follow when writing code is the **DRY** principle - Don't Repeat Yourself. If you find yourself writing the same (or very similar) code again and again, that's a good sign that you should be writing a function instead. Once a function has been written once, it can be called as many times as you want. Instead of writing ten lines of code thirty times, you can write ten lines once, and call the function thirty times. As much as possible, push the work onto the computer.

### Defining functions

The keyword `def` is used to create functions. It's short for "define", as that is what we are really doing - "defining" a new word for the computer to understand.

```
def get_full_hippo_name():
  return "hippopotamus"
```

The above function has one job - it returns the word "hippopotamus"; it's not a very useful function, but it makes the syntax clear. First comes the keyword `def`, then the name of the function, then brackets, and then the colon. All of these parts are necessary.

Just as with loops and IF statements, the code indented under a function belongs to the function.

Function names are similar to variables - they can be almost anything you want. [PEP8](https://www.python.org/dev/peps/pep-0008/#function-and-variable-names), the Python style guide, recommends that you write function names in lower case, with underscores - "\_" - separating words.

The `return` keyword is an important one to understand. A function stops when it reaches a `return` keyword; no code after the `return` is ever run. When a function uses `return`, the value following the return is passed back out to wherever you called the function from. In the example below, the variable `animal` is set equal to "hippopotamus", because that is the value the function returns.

```
  animal = get_full_hippo_name()
```

### Parameters & arguments

A function that returns a hard-coded value isn't particularly useful; we might as well just use the value directly. Functions always do the same thing, but they can do the same thing on different inputs to get more useful output.

When we covered [using functions](6_comments_and_using_functions.md), we discussed "arguments". An argument is a value passed to a function when it runs, but we need to tell the function to expect the value. To do that, we need parameters.

Parameters and arguments look very similar, and are easy to get confused. Most of the time, the difference is unimportant, but the essential idea is that arguments are the actual values, and parameters are placeholders for those values.

To define a parameter, we put the parameter name (which works just like a variable name) in the brackets after the function name. Just like with arguments, you can have more than one, and the order is important.

Once a parameter has been named, you can use the name within the function as though it was a variable. When the function is called, the arguments will take the place of the parameters in the code.

```
def birthday_greeting(name):
  print("Happy Birthday, name + "!")
```

The function above has one parameter - `name`. When the function is called, it expects an argument to fill that parameter; calling the function without one - `birthday_greeting()` will cause an error. An error will also occur if you give the function more arguments than it expects. If you call the function with one argument, it uses that argument to fill the placeholder parameter.

`birthday_greeting("Sarah")` will print out "Happy Birthday, Sarah!". `birthday_greeting("Dracula")` will print out "Happy Birthday, Dracula!". The function always does exactly the same thing, but the value you give it changes the eventual output.

### Guidelines

Don't over-complicate your functions - ideally, a function should do one thing well. If you find your functions getting large and complex, then you should probably turn each part of it into a new function.

Don't overuse functions; they aren't always necessary. If you just want to add two numbers together, there is nothing wrong with using `2 + 2` rather than writing a function to do that. Functions should make your life easier, not more complicated.

### Next steps

You should now have the skills to attempt [challenge 5](./challenges/challenge_5.md).

Functions might not seem that useful at first, but as the complexity of your programs grows, they'll start to become indispensable. If you are sure you understand everything up until now, move on to the [final section](11_next_steps.md).
