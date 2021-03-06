[<<< Previous](09-google.md) |  [Next >>>>](11-introspection.md)

# A Little Motivation

Early on, we learned a bit about lists, which look like this:

```python
['rose', 'violet', 'buttercup']
```

We're going to create a small application that will print a random motivational saying every time a user presses `Enter`. Our first step will be to create a list of positive sayings:

```python
motivational_phrases = [
        "Importing modules is easy!",
        "Programming! Yay!",
        "You write lists like a pro!",
    ]
```

Lists open with a square bracket `[`, have items seperated with commas, and end with a square bracket `]`, like this:

```python
[1, 2, 3, 4, 5]
```

Our positivity list above spreads the list out over multiple lines for greater readability, which is allowed in Python. Remember that you can change the strings in the list to whatever phrases you choose.

## Importing a module

Now that we have our sayings, let's use it in conjunction with some functionality from a module that's built into Python: the `random` module.

```python
import random

motivational_phrases = [
        "Importing modules is easy!",
        "Programming! Yay!",
        "You write lists like a pro!",
    ]

print(random.choice(motivational_phrases))
```

The `random.choice` function chooses a random item from a list and returns it. The `.` syntax indicates that the function is coming from the `random` library.

1. The real point of this section is to learn `import`, which is where Python really starts to get interesting. Python comes with many libraries (importable collections of code), and you can install many more. Think of something you're interested in doing (statistics, text analysis, web scraping, quantitative analysis, processing Excel/PDF/image files) and search google "\<thing you're interested in> python library". You're almost certain to find some useful results.

2. (optional) As with our weather app, this positive saying generator could be improved by making it so the program doesn't have to run again every time to get new output. Add a while loop for the final version. You can see a solution [here](solutions/motivation.md).

# Challenge: library research

As we've learned, libraries are Python code written by others that can be pulled into your program, allowing you to use that functionality. In this challenge, do a little research on Python libraries that might solve a problem for you or address a domain that you're interested in.

The best way to find a Python library in a particular area is to do a Google search. For example, if you wanted to find Python libraries for dealing with cleaning up HTML files, you might search one of these:

> working with html python library
  
> html parser python library

In your research, you may also want to look at the libraries that come with Python. You can find a list of libraries in these libraries [here](https://docs.python.org/3/py-modindex.html).

[<<< Previous](09-google.md) |  [Next >>>>](11-introspection.md)
