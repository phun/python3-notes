# Python3 Notes
Most useful things in Python3 for scripts and leetcoding

## Glossary
1. [Arrays](#arrays)
2. [Dictionaries](#dictionaries)
3. [Strings](#strings)
4. [Looping](#looping)
5. [Built-in functions](#built-in-functions)

## Arrays

## Dictionaries

### `Dict.get(key, default_value)`
Returns the value at index `key`. If index does not exist, return the `default_value` instead.
```python3
# Count occurences in an array
map = {}
for n in nums:
  map[n] = map.get(n, 0) + 1
```
### `(key in dict)` and `(key not in dict)`
Returns boolean based on if `key` is in or not in `dict`.
```python3
map = {}
map['j'] = 1
('j' in map) # Returns True
('k' not in map) # Returns True
```

### Tips

#### You can use tuples as keys
```python3
memo = {}
memo[(left+1, right)] = maxDiff(left+1, right)
```

## Strings

### `String[start:stop:step]`
Returns the character(s) starting from index `start`, ending at (but **not** including) index `end`, with every `step`th character.
```python3
"Helping"[0] # Returns "H"
"Helping"[1] # Returns "e"
"Helping"[-1] # Returns "g"

"Helping"[:3] # Returns "Hel"
"Helping"[1:3] # Returns "el"

"Helping"[:6:2] # Returns "Hli"
```

### `String.count(c)`
Returns and integer of the number of occurences of character `c`
```python3
"00010".count('1') # Returns 1
"00010".count('0') # Returns 4
```

### `String.isalnum()`
Returns `True` if all the characters in the string are alphanumeric, (A-Za-z) or (0-9).
```python3
"Hello".isalnum() # Returns True
"123".isalnum() # Returns True
"Hello123".isalnum() # Returns True
"Hello world".isalnum() # Returns False because of space
```

### `String.lower()`
Returns version of the string where all characters are lower case. 
```python3
"Hello world".lower() # Returns "hello world"
"wat".lower() # Returns "wat"
"HELLO 123".lower() # Returns "hello 123"
```

## Looping

### Basic `for` loop
We have no access to the index.
```python3
for item in iterable:
```

### Using `range()` and indexes
Using `range()`, we can loop and have access to the index.
```python3
for i in range(len(iterable)):
  item = iterable[i]
```

### Using `enumerate()` and indexes
Using `enumerate()`, we can also loop and have access to the index with 1 less line of code. It's lower than the overhead of looping over a range and indexing each time, and lower than manually tracking and updating the index separately. It is heavily optimized.
```python3
for i, item in enumerate(iterable):
```

## Built-in Functions

### `all()`

### `any()`

### `len()`

### `max()`

### `min()`
