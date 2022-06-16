# Intro to Data Structures

## Learning Goals

- Understand what a data structure is and how they are used in Python
- Learn which types of tasks data structures are used to solve

## Introduction

**Data** is information that has been standardized in such a way that it is
useful to the individual or machine that is working with it. Everything that
you see on your computer screen right now is composed of data. The letters
in this paragraph, the colors on this page, the links and buttons that navigate
to and from resources on the internet- all data.

In **Python Fundamentals**, we talked about the importance of organizing our
code for other humans to be able to read. After all, [a foolish consistency is
the hobgoblin of little minds][pep 8 hobgoblin]. **Data structures** are a way
for us to organize data in a way that is easy for computers to read.

[pep 8 hobgoblin]: https://peps.python.org/pep-0008/#a-foolish-consistency-is-the-hobgoblin-of-little-minds

## Why Don't We Just Put Everything in a List?

`list` objects are very useful for storing data in Python, but there are many
situations where a computer would want data stored in a different way.

To provide some perspective, let's compare a `list` with a `set`:

<table>
<tr>
<th> list </th>
<th> set </th>
</tr>
<tr>
<td>

Can store all types of data.

Indexed - Each item in a list has a set location.

Mutable - Can be extended or converted to another data type.

Items can be repeated.

Items can be changed or replaced.

</td>
<td>

Can store all types of data.

Unindexed - Items in a set are stored through a [hash][hash table] of the
item's name.

[hash table]: https://en.wikipedia.org/wiki/Hash_table

Mutable - Can be extended or converted to another data type.

Items are unique.

Items cannot be changed or replaced.

</td>
</tr>
</table>

There are a number of similarities here, and it's clear that `list` objects
are much more flexible than `set` objects. But if we're looking for _which_
items exist rather than _how many_, a data structure with unique items that
allows us to access them by _name_ rather than _index_ is more useful. Lucky
for us, Python provides the `set` data structure out of the box!

[hash table]: https://en.wikipedia.org/wiki/Hash_table

## Types of Data Structures in Python

Python gives us access to a number of different data structures to help us
communicate with our computers. Some are built-in **data types** while others
require a little more work to set up.

### Data Types that are Data Structures

- `list`
- `tuple`
- `str`
- `set`
- `dict`
- [_`frozenset`_*](https://docs.python.org/3/library/stdtypes.html#frozenset)
- [_`bytes`_*](https://docs.python.org/3/library/stdtypes.html#bytes)
- [_`bytearray`_*](https://docs.python.org/3/library/stdtypes.html#bytearray)

\* _We won't be covering these in our curriculum, but they may be useful to you
in mathematics or academic computer science_

### `collections` and `queue`

Python does not come with _every_ data structure built into its data types, but
the standard library includes several modules and packages that help us build
out more complex data structures. `collections` and `queue` are the two most
common; we'll explore them later on in this unit.

Be sure to check out the resources below as well, and bookmark them for future
reference!

## Resources

- [Python 3.8 documentation](https://docs.python.org/3.8/)
- [Python documentation: Data Structures](https://docs.python.org/3/tutorial/datastructures.html)
- [Common Python Data Structures](https://realpython.com/python-data-structures/)
