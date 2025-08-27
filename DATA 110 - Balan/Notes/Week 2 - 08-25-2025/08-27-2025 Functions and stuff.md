##### Enumeration
>Enumerating is useful if you want to print the index of an array.

```python
for index,element in enumerate(some_array_):
	print(index, element)
	```
##### Range
- Range is a special cousin of list used for sequential integers
- range(start, end, step)
	- Default for start is 0
	- Default for step is 1
- Includes start and up to end-1
- Special use case is range(n)
- Indexing and sequencing work the same as for list
- Often used with loops!
```python
my_range = range(0, 20, 2)
# my_range -> range(0, 20, 2)
list(my_range()
```