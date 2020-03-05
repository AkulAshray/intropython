# IF statements

[Back to the outline](0_outline.md)

A key part of programming is using conditional logic - making a program behave differently depending on user input or data. One of the main ways this is accomplished is through IF statements.

An IF statement is a piece of code that only runs **if** a condition is `True`; it's the main use of [boolean expressions](4_data_types_and_logic.md). If a the condition is `False`, the code is skipped.

### Learning objectives

- [ ] I use IF statements to make decisions in code
- [ ] I understand the structure and syntax of complex IF statements
- [ ] I can include multiple conditions within the same IF statement

### IF

The syntax of an IF statement is similar to a FOR loop.

```
if 3 < 4:
  print("Three is less than four.")
```

There is the `if` keyword, followed by an expression that could evaluate to `True` or `False`. The line is ended by a colon.

Code indented underneath the `if` line runs **only** if the condition evaluates to `True`. If it is `False`, the code is missed out entirely.

```
if 4 < 3:
  print("This line never prints.")
  print("Neither does this one.")

print("This one does, because it is not indented.")
```

### ELSE

The `else` keyword is used when you want to run code if the checked condition is not `True`.

```
if animal == "cat":
  print("It is a cat.")
else:
  print("It is not a cat.")
```

In the above code, if the variable `animal` is equal to "cat", then the program prints out the first line. If it is equal to anything else, then the second line is printed.

### ELSE IF

Sometimes, you will want to choose between several blocks of code. The `elif` keyword - short for "else if" allows you to check multiple conditions.

```
animal = input()

if animal == "cat":
  print("It is a cat.")
elif animal == "horse":
  print("It is a horse.")
elif animal == "budgie":
  print("It is a budgie.")
else:
  print("Unknown animal. Possibly a crocodile.")
```

In the code above, the user is first prompted to enter a value. The value is stored in the variable `animal`, and then is checked against each condition in turn until it either finds a `True` condition, or reaches the `else`.

You can have 0 `elifs` inside an IF statement, or you can have as many as you want.

### Conditional sequence

Every IF statement has to start with an `if`. `else` is optional, as are `elif`s. The program checks each condition in strict sequence, and stops checking the conditions when it finds a `True`. It's important to carefully order your conditions, so that the right ones get evaluated first. `if` always goes first, `else` last, but the order of the conditions attached to those keywords can have significant effects on programs.

Note that `else` has no condition - it catches everything that has not already matched another condition.

### Next steps

You should now have the skills to attempt [challenge 4](./challenges/challenge_4.md).

IF statements can be combined in a lot of ways, and allow very complicated programs. Take the time to be clear on how they work, exactly how they are written, and how the different keywords relate to each other. Then head to the [next section](10_writing_functions.md).
