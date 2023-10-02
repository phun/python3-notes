# Python3 Notes
Most useful things in Python3 for scripts and leetcoding

## Glossary
1. [Arrays](#arrays)
2. [Strings](#strings)

## Arrays



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

### `String.isalnum()`
Returns `True` if all the characters in the string are alphanumeric, (A-Za-z) or (0-9).
```python3
"Hello".isalnum() # Returns True
"123".isalnum() # Returns True
"Hello123".isalnum() # Returns True
"Hello world".isalnum() # Returns False because of space
```

### `String.lower()`
Returns version of the  string where all characters are lower case. 
```python3
"Hello world".lower() # Returns "hello world"
"wat".lower() # Returns "wat"
"HELLO 123".lower() # Returns "hello 123"
```
