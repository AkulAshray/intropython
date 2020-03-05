# Importing

[Back to the outline](0_outline.md)

In the previous section, we looked at functions, including some of the built-in functions that are automatically included in Python. In this section, we will explore how to gain access to a wider range of pre-written functions.

### Learning objectives

- [ ] I can import modules and access their code
- [ ] I can import modules in different ways

### What is importing for?

The built-in functions are useful, and cover a lot of possibilities, but they don't cover everything. Frequently, you'll want to do things that you can't do easily, or at all, just using standard Python functions.

When that happens, you have two options:

1. write new functions yourself

2. use functions someone else has already written

Option 1 is the answer a lot of the time, and we will discuss defining your own functions in a [later section](10_writing_functions.md). However, there is little point reinventing the wheel and toiling for hours over problems that other people have already solved and shared the code for.

Option 2 gives you a way around obstacles that might otherwise distract from your main purpose. Python allows you to "import" functions and other code into your program - you can make use of functions that other people have written. It's an easy way to get complex behaviour out of a program without having to do everything from scratch.

### Importing modules

Importable code is stored in named "modules" or "libraries". To import a module/library, use the keyword `import` and then the name of the module at the top of your program.

`import random` is an instruction that tells Python to load the `random` library, making all the functions in the library available to you. `random` is a library that contains several useful functions for working with random - technically [pseudorandom](https://en.wikipedia.org/wiki/Pseudorandom_number_generator) - numbers. Once the library is imported, you can use functions such as `randint` to generate random numbers.

To use an imported function, you use the name of the library, followed by a full stop, and then the name of the function with brackets at the end. You cannot use an imported function in the code before you import the module - Python will raise an error if you try.

`random.randint()`

Using the operator '.' generally signifies going inside the contents or properties of the operator's first argument. For example, an expression like 'library1.function2()' signifies that we are going inside the contents of the library 'library1', into one of its functions - namely, 'function2' - and executing it.

There are many, many libraries freely available for Python programming. A lot of them come installed automatically with Python, while even more can be installed using [separate software](https://docs.python.org/3/installing/index.html).

### Partial importing

When you import a module just using the keyword `import`, you load the whole module into the program. With large enough modules, or several imports, this can slow your program and make it less efficient. Especially if you only need a couple of imported functions from a module, it's wasteful to import the whole thing.

You can use the `from` keyword to tell Python that you only want to fetch part of a module.

`from random import randint`

In the example above, only the function `randint` is imported. All the other functions are not loaded.

If you want to import more than one function from a module, separate them with commas.

`from random import randint, choice, randrange`

### Renaming modules

Sometimes you may wish to change the name of a module in your code - to save you having to type out the full name each time, or to avoid two things having the same name. Use the `as` keyword for this.

`import pandas as pd`

Using `as` renames the module **within your program**; the actual module name is unchanged, but you can refer to the module by the new name.

### Next steps

Take the time to experiment with different python modules and their capabilities. `pandas`and `sklearn` are very helpful for data science, and would be worth a look.

When you feel confident with imports, it's time for the [next section](8_loops.md).
