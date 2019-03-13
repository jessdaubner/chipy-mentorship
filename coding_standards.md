# Coding Standards

## The Zen of Python
The Zen of Python describes guiding principles for Python design. Following these principles will help you
write _pythonic_ code that is consistent with the spirit of Python programming. 

You can access the Zen of Python anytime, by starting the Python interpreter (enter `python` at the command prompt) and typing `import this`.

```bash
$ python
Python 3.7.2 (default, Jan 13 2019, 12:50:01)
[Clang 10.0.0 (clang-1000.11.45.5)] on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> import this
The Zen of Python, by Tim Peters

Beautiful is better than ugly.
Explicit is better than implicit.
Simple is better than complex.
Complex is better than complicated.
Flat is better than nested.
Sparse is better than dense.
Readability counts.
Special cases aren't special enough to break the rules.
Although practicality beats purity.
Errors should never pass silently.
Unless explicitly silenced.
In the face of ambiguity, refuse the temptation to guess.
There should be one-- and preferably only one --obvious way to do it.
Although that way may not be obvious at first unless you're Dutch.
Now is better than never.
Although never is often better than *right* now.
If the implementation is hard to explain, it's a bad idea.
If the implementation is easy to explain, it may be a good idea.
Namespaces are one honking great idea -- let's do more of those!
```

## Style Guides & Python Conventions
* [PEP-8](https://www.python.org/dev/peps/pep-0008/) is the definitive style guide for Python. Note that PEP stands for Python Enhancement Proposal, which is the process for improving Python as a programming language.
* [Google's Python Style Guide](http://google.github.io/styleguide/pyguide.html) and [Google Style Docstrings](https://sphinxcontrib-napoleon.readthedocs.io/en/latest/example_google.html) are also great resources.

### Static Linting
Tools like [`flake8`](https://github.com/PyCQA/flake8) and [`pylint`](https://github.com/PyCQA/pylint) will notify you when your code has programming errors before runtime and also points out when you've deviated from PEP-8 conventions.

### Docstrings
Docstrings are strings that occur as the first statements in a file (module), function, method, or class and provide useful documentation of that object.
They begin with a triple quote (e.g. `'''` or `"""`) and are accessible via the `__doc__` special attribute of that object. It's a good practice to
document all modules, functions, methods, and classes. Your collaborators and/or future self with thank you!

```python
def add(a, b):
    """Adds a and b

    Args:
      a (int): an integer
      b (int): an integer

    Returns:
      int, the sum of a and b
    """
    return a + b
```
