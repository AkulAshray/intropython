# Data types and logic

[Back to the outline](0_outline.md)

This section deals with two core concepts in programming - data types and logic. Data types are important for anything to do with information, while understanding programming logic is the first step towards complex, branching programs.

### Learning objectives

- [ ] I understand the differences between the data types
- [ ] I can identify different data types
- [ ] I can evaluate logical/boolean expressions

### Data types

Programs often involve several different types of data, and the computer will store and interpret each type differently. Python is a [dynamically typed](https://pythonconquerstheuniverse.wordpress.com/2009/10/03/static-vs-dynamic-typing-of-programming-languages/) language, which essentially means that it is less strict with data types than some other programming languages, but it is still important to know the different types and what they mean.

The basic data types in Python are as follows:

* integer - a whole number, such as `7`
* float - a non-integer number, e.g. `3.546`
* string - a collection of characters between speech marks such as `"crocodile"` or `"alligator"` ('\'' and '\"' are both fine, as long as they match)
* boolean - `True` or `False`

```
num = 7
num = "seahorse"
num = False
```

The above code does not cause any errors - a variable can store data of any type. However, you cannot combine data of different types without first converting one datum into a different type. `num = 'seahorse' + False` would cause an error.

### Logic

A key part of programming is being able to write logical expressions. An expression is something that the computer can evaluate as `True` or `False`. `2 != 3` is an expression that evaluates to `True` - the '!=' is a comparison operator (similar to the mathematical ones from the [previous section](3_operators_and_variables.md)) that means 'not equal to'. 2 is *not equal to* 3, and so the computer evaluates the expression to `True`.

`True` and `False` are the only two values that the 'boolean' data type can be. Logical expressions are also called boolean expressions, because they are evaluated to boolean values.

When an expression is evaluated, we say that it "returns" a value.

### Comparison Operators

Being able to compare values together is useful in all sorts of programs; by using comparison operators to create expressions which evaluate to boolean values, we can create programs with multiple paths and decisions.

In this section, we aren't going to go into conditional programming - that comes later. However, understanding the operators is the first step towards making such programs.

* ">" - greater than
* "< " - less than
* "==" - equal to
* "!=" - not equal to
* ">=" - greater than or equal to
* "<=" - less than or equal to

`5 < 4` returns `False`.

`4 == 4` evaluates to `True` - note the double equals sign. In Python, single equals is for assigning a value, while double equals is for comparing them.

`3 >= 9` is `False` but `9 != 3` is `True`.

`True == False` results in `False`.

### Logical Operators

Comparison operators only allow you to check one thing at once. If you want to check multiple conditions - is a value greater than 4 but not equal to 7, for example - you need to use logical operators.

Logical operators allow you to chain logical expressions together to create more complex ones. The logical operators are `and`,`or`, and `not`.

`and` returns `True` if the expressions on both sides of it return `True`. `or` returns `True` if at least one side evaluates to `True`. `not` returns the opposite of what the expression following it would normally return.

`89 != 45 and "dog" != "cat"` returns `True`, because both sides are `True`.
`False and True` evaluates to `False` because the left-hand side is `False`.
`23 > 4 or False` evaluates to `True` because the left side is `True`, even though the right side isn't.
`not True` is `False`, because it reverses the expression. `not False` is `True`.

### Next steps

You should now have the skills to attempt [challenge 1](./challenges/challenge_1.md).

When you are ready, move on to the [next section](5_indices_and_lists.md).
