---
assignment: Dictionaries and Structuring Data
---

# Practice Questions

Answers

1. Problem 1 — What does the code for an empty dictionary look like?
   - Answer:
     `{}`

2. Problem 2 — What does a dictionary value with a key 'foo' and a value 42 look like?
   - Answer:
     `{'foo': 42}`

3. Problem 3 — What is the main difference between a dictionary and a list?
   - Answer:
     Lists are ordered collections indexed by integer positions; dictionaries store key–value pairs and are accessed by keys.

4. Problem 4 — What happens if you try to access spam['foo'] if spam is {'bar': 100}?
   - Answer:
     It raises a `KeyError` because 'foo' is not a key in the dictionary.

5. Problem 5 — Difference between 'cat' in spam and 'cat' in spam.keys()?
   - Answer:
     No difference; `'cat' in spam` checks keys, exactly like `'cat' in spam.keys()`.

6. Problem 6 — Difference between 'cat' in spam and 'cat' in spam.values()?
   - Answer:
     `'cat' in spam` checks whether 'cat' is a key, while `'cat' in spam.values()` checks if 'cat' is a value.

7. Problem 7 — What is a shortcut for the following code?

        if 'color' not in spam:
            spam['color'] = 'black'

   - Answer:
     `spam.setdefault('color', 'black')`

8. Problem 8 — What module and function can be used to “pretty print” dictionary values?
   - Answer:
     The `pprint` module and the `pprint()` function.
