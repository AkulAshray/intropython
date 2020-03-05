# Loops

[Back to the outline](0_outline.md)

Programming isn't very useful if we have to write new code every time we want to do something, even if we've already done it before. The whole point of code is to make the computer do tasks that are too boring or repetitive for humans.

Loops allow you to tell Python to repeat a section of a code a number of times. Instead of writing the same lines again and again, you can write them once and put them in a loop.

### Learning objectives

- [ ] I can use FOR and WHILE loops to repeat code
- [ ] I understand the structure of loops
- [ ] I can use count variables inside loops

### FOR Loops

A FOR loop is used when you want to do something a known number of times. The below code prints out "Watch me loop!" ten times.

```
for i in range(0, 10):
  print("Watch me loop!")
```

The syntax for a FOR loop is quite specific. First comes the `for` keyword, and then a variable name. This variable is used to store how many times the loop has run; by convention, `i` is used as the variable name, but it could be anything.

After that, you need to tell Python the start number for `i`, and the end number. This is accomplished by using `range(start, end)`. The loop will run as many times as there are integers between the first number (inclusive) and the last number (exclusive). `range(0,5)` runs 5 times, for 0,1,2,3,4.

The final key piece is the colon - it's easy to forget, but Python will error without it. That completes the actual loop instructions.

Underneath that line, anything indented will run as many times as the loop runs. The indentation is vital, as it tells Python which lines are part of the loop. Other languages use curly brackets "{}" to show which code belongs to the loop, but in Python, you need to make absolutely sure that the code you want to run is indented correctly.

```
for i in range(0,5):
  print("inside the loop")

print("outside the loop")
```
In the above code, "inside the loop" will print out 5 times - as many times as the loop runs - but "outside the loop" will only display once.

### Count variables

The `i` (or other name) variable is a "count" variable. The variable will be increased automatically by 1 each time through the loop. By default, a `for` loop runs as many times as it takes for the variable to get from the first number to the second number by adding 1 each time.

```
for count in range(0,1000):
  print(count)
```

In the above code, the variable `count` has been used instead of `i`, simply to demonstrate that `i` is not the only possible name. Note that `count` can also be accessed inside the loop; it's often useful to know how many times the loop has run, especially when combined with [indexing](5_indices_and_lists.md) to access each part of a list in turn.

### WHILE Loops

A WHILE loop is used when you want to repeat something an unknown number of times. As a general rule, you should aim to use WHILE loops rarely, as they easily lead to infinite loops and other issues.

WHILE loops repeat the code indented beneath them as long as an expression evaluates to `True`.

```
while 3 < 4:
  print("always true")
```

The above loop would repeat forever, as 3 will always be less than 4. The loop below will run 0 times, as the condition is never `True`.

```
while False:
  print("This line will never run")
```

Just as with FOR loops, the indentation is important.

### Next steps

You should now have the skills to attempt [challenge 3](./challenges/challenge_3.md).

As with every concept we've covered so far, this has been a brief introduction to basic loops. They can be customised and combined in all sorts of ways. Once more, you should experiment until you feel comfortable with the concepts. After that, there is the [next section](9_if_statements.md).
