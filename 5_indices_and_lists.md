# Indices and lists

[Back to the outline](0_outline.md)

In previous sections, we've looked at different types of data, such as strings and integers. We've also looked at variables - named locations to store values. So far, we have dealt with single values at a time, but it's often useful to collect data in one place and work with multiple values at once. In this section, we will look at collections of values, and how to access just one part of a collection.

### Learning objectives

- [ ] I can create lists of values
- [ ] I can access a specific value from a list using indices
- [ ] I can access a character from a string using indices

### Indices

We've already encountered [strings](4_data_types_and_logic.md) - one of Python's fundamental data types, consisting of a group of characters inside speech marks, such as `"iguana"` or `'walrus'`. The computer interprets strings as text, unlike integers or other data types, which are treated directly as values.

Strings are slightly different to the other fundamental data types because they are collections of characters, not one indivisible concept like `True`. This means that strings in Python behave slightly differently to other data types.

Strings are "indexed" - each character in a string has a numbered location. Python, like many other programming languages, is "zero-indexed", which means that the numbering starts at 0. This is an important fact to remember, as forgetting it is one of the most common programming errors.

In the string `"Baba Yaga"`, the character "B" is at index 0. The highest index is 8, with the character "a". Using string indexing, we can access a specific character from a string using square brackets - `"Baba Yaga"[5]` is equal to "Y". Note that the space does count as a character.

If you have stored a string as a variable, indexing still works.

```
my_string = "I <3 Python"
my_string[2]
```

This method does not work with other data types. `123[2]` results in an error, not "3", just as `True`[1] does - Python only understands indexing for things it thinks of as groups of values, not single values.

### Lists

A list is a collection of values. It allows you to collect related data in one place, keeping it together and lessening the number of variables you need to create. Items in a list are referred to as "elements"

Python lists are created using square brackets. They can be assigned to variables just like a single value can be. Values in a list are separated by commas.

```
my_list = ["parrot", "budgie", "cockatoo"]

```
Lists can hold data of any type, in any combination.

```
another_list = [1,7,5,78]
yet_another = [1, True, "gecko", 0.33]
```

Lists are indexed, and a single value can be accessed from a list in the same way as you would access a single character from a string.

```
my_list = [5,6,7]
my_list[0]
```

You can also use indices to change a list element. Simply access the element you want using indexing, and then set it equal to a new value.

```
my_list = [3,4,5]
my_list[2] = 45

```

In the example above, the list ends up as `[3,4,45]`

### Next steps

You should now have the skills to attempt [challenge 2](./challenges/challenge_2.md).

Once you feel confident, move on to the [next section](6_comments_and_using_functions.md).
