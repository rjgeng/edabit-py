# Slightly Superior

-   [Slightly Superior](https://edabit.com/challenge/ZF6vZwPc5He5u5EFe)

You will be given two **extremely** similar lists, but exactly one of the items in a list will be valued slightly higher than its counterpart (which means that evaluating **the value > the other value** will return 'True').

Create a function that returns whether the first list is slightly superior to the second list.

**Examples**

```
is_first_superior([1, 2, 4], [1, 2, 3]) ➞ True
# The pair of items at each index are compared in turn.
# 1 from the first list is the same as 1 from the second list.
# 2 is the same as 2.
# However, 4 is greater than 3, so list one is superior.

is_first_superior(["a", "d", "c"], ["a", "b", "c"]) ➞ True

is_first_superior(["zebra", "ostrich", "whale"], ["ant", "ostrich", "whale"]) ➞ True

is_first_superior([1, 2, 3, 4], [1, 2, 4, 4]) ➞ False

is_first_superior([True, 10, "zebra"], [True, 10, "zebra"]) ➞ False
```

**Notes**


-   oth lists will be the same length.
-   All values and their counterparts will always be the same data type.
-   The lists will only be different by one element.
-   If the two lists are the same, return `False`.

**Solution**  

```
def is_first_superior(lst1, lst2):
	for i in range(len(lst1)):		
		if (lst1[i] > lst2[i]):
			return True
	return False
```

**Solution 2**  

-   [Joshua Señoron](https://edabit.com/user/PXAcsKkssS2yLyDv2)

```
def is_first_superior(lst1, lst2):
	return lst1 > lst2
```


