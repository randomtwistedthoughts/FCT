# Managing Strings — Practice Questions & Answers

## 1. What are escape characters?
**Answer:** Escape characters are special sequences that represent characters that are difficult or impossible to type directly into a string.  
**Explanation:** They start with a backslash (\) and allow insertion of tabs, newlines, quotes, etc.

## 2. What do the `\n` and `\t` escape characters represent?
**Answer:** `\n` represents a newline, and `\t` represents a tab.  
**Explanation:** They control formatting inside a string.

## 3. How can you put a `\` backslash character in a string?
**Answer:** Use `\\` inside the string.  
**Explanation:** The first backslash escapes the second.

## 4. The string value `"Howl's Moving Castle"` is a valid string. Why isn't it a problem that the single quote in the word *Howl's* isn’t escaped?
**Answer:** Because the string uses double quotes around it.  
**Explanation:** Single quotes only need escaping when the string itself is enclosed in single quotes.

## 5. If you don’t want to put `\n` in your string, how can you write a string with newlines in it?
**Answer:** Use triple-quoted strings (`''' ... '''` or `""" ... """`).  
**Explanation:** Triple quotes preserve line breaks directly.

## 6. What do the following expressions evaluate to?

- `'Hello world!'[1]`  
  **Answer:** `'e'`

- `'Hello world!'[0:5]`  
  **Answer:** `'Hello'`

- `'Hello world!'[:5]`  
  **Answer:** `'Hello'`

- `'Hello world!'[3:]`  
  **Answer:** `'lo world!'`

## 7. What do the following expressions evaluate to?

- `'Hello'.upper()`  
  **Answer:** `'HELLO'`

- `'Hello'.upper().isupper()`  
  **Answer:** `True`

- `'Hello'.upper().lower()`  
  **Answer:** `'hello'`

## 8. What do the following expressions evaluate to?

- `'Remember, remember, the fifth of November.'.split()`  
  **Answer:** `['Remember,', 'remember,', 'the', 'fifth', 'of', 'November.']`

- `' - '.join('There can be only one.'.split())`  
  **Answer:** `'There - can - be - only - one.'`

## 9. What string methods can you use to right‑justify, left‑justify, and center a string?
**Answer:** `rjust()`, `ljust()`, and `center()`  
**Explanation:** These methods pad the string with spaces (or a chosen character).

## 10. How can you trim whitespace characters from the beginning or end of a string?
**Answer:** Use `strip()`, `lstrip()`, or `rstrip()`.  
**Explanation:** They remove whitespace (or a specified character) from both sides, the left side, or the right side, respectively.
