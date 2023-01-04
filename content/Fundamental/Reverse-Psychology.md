# Reverse Psychology

-   [Reverse Psychology](https://edabit.com/challenge/bMdFkscm8ESR5GLtN)

For this challenge, you will NOT be given a string. Your task isn't to add "Do not" before the given string. If there is no given string, you will not return "Do not do anything." Do not check the examples to know how to do this challenge.

**Examples**

```
reverse_psychology("wash the dishes") ➞ "Do not wash the dishes."

reverse_psychology("eat your lunch") ➞ "Do not eat your lunch."

reverse_psychology("go to school") ➞ "Do not go to school."
```

**Notes**

**Solution**  

```
def reverse_psychology(s = "Do not do anything."):
	return s if s == "Do not do anything." else "Do not " + s + "."
```

**Solution 2**  

-   [comecheckoutmycode](https://edabit.com/user/9ivvGvJGvtQfigQaZ)

```
ddef reverse_psychology(s="do anything"):
	return "Do not {}.".format(s)
```


```
def reverse_psychology(*s):
    return 'Do not ' + "".join(s) + '.' if s else 'Do not do anything.'

```