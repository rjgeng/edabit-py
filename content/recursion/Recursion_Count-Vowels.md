# Recursion: Count Vowels

-   [Recursion: Count Vowels](https://edabit.com/challenge/nHxBoXmRYq5vnoEnq)

Write a function that **recursively** returns the number of vowels in a string.

**If it wasn't clear enough already, you should use recursion in your solution.**

**Examples**

```
vowels("apple") ➞ 2

vowels("cheesecake") ➞ 5

vowels("bbb") ➞ 0

vowels("") ➞ 0
```

**Notes**
-   Recursive functions call themselves.
-   All letters will be in lower case.
-   For this challenge, the vowels are a, e, i, o, and u.

**Solution**  

```
VOWELS = 'aeiouAEIOU'

def vowels(s):
    if not s:
        return 0
    elif s[0] in VOWELS:
        return 1 + vowels(s[1:])
    else:
        return 0 + vowels(s[1:])
```

**Solution 2**  

-   [zatoichi49](https://edabit.com/user/tAF9Gf6PiGogbZuWs)

```
def vowels(s):
	return 0 if not s else (s[0] in 'aeiou') + vowels(s[1:])
```