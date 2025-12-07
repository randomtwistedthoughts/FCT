# Pattern Matching with Regular Expressions — Practice Questions & Answers

## 1. What is the function that creates Regex objects?
**Answer:** `re.compile()`  
**Explanation:** This function compiles a regular expression pattern into a Regex object for reuse.

## 2. Why are raw strings often used when creating regex objects?
**Answer:** To prevent Python from interpreting backslashes as escape characters.

## 3. What does the search() method return?
**Answer:** A Match object if a match is found; otherwise `None`.

## 4. How do you get the actual strings that matched the pattern from a Match object?
**Answer:** Using `.group()` or `.group(n)`.

## 5. In the regex created from `r'(\d\d\d)-(\d\d\d-\d\d\d\d)'`, what does group 0 return? Group 1? Group 2?
- **Group 0:** Entire matched string  
- **Group 1:** First parentheses group (area code)  
- **Group 2:** Second parentheses group (phone number)

## 6. Parentheses can have specific meanings in regex patterns. What is the difference between `\d{3}` and `(\d){3}`?
- `\d{3}` matches **three digits in a row**.  
- `(\d){3}` captures each digit as a group but still matches three digits.

## 7. What does a pipe character (|) signify in a regex?
**Answer:** Alternation — matches one expression OR another.

## 8. What do you mean by “greedy” and “non-greedy” matching?
- **Greedy:** Matches as much text as possible.  
- **Non-greedy (`?`):** Matches as little text as possible.

## 9. What is the character class shorthand for all numbers and lowercase letters?
**Answer:** `[a-z0-9]` or using shorthand: `\w` (includes underscore).

## 10. What is the difference between `\d` and `\D`?
- `\d` matches digits.  
- `\D` matches non-digits.

## 11. What is the difference between `\s` and `\S`?
- `\s` matches whitespace.  
- `\S` matches non-whitespace.

## 12. What is the difference between `\w` and `\W`?
- `\w` matches letters, digits, and underscore.  
- `\W` matches everything else.

## 13. What do the `^` and `$` shorthand characters signify in regex?
- `^` anchors the start of the string.  
- `$` anchors the end of the string.

## 14. How do you make a regular expression case-insensitive?
**Answer:** Use the flag `re.IGNORECASE` or `re.I` when compiling.

## 15. What does the `.` character normally match? What does it not match?
- It matches **any character except newline** unless `re.DOTALL` is used.

## 16. If `numRegex = re.compile(r'\d+')`, what will `numRegex.findall('12 drummers, 11 pipers, five rings, 3 hens')` return?
**Answer:** `['12', '11', '3']`

## 17. What is the difference between `re.search()` and `re.findall()`?
- `search()` returns the **first match**.  
- `findall()` returns **all matches** as a list.

## 18. When dividing a username and domain string at the @ symbol, how do you use the `.split()` method?
**Answer:** `"user@example.com".split('@')` → `['user', 'example.com']`

## 19. How would you write a regex that matches a number with commas for every three digits?
It must match:
- `"42"`
- `"1,234"`
- `"6,368,286"`

But **not**:
- `"12,34"` (incorrect comma placement)
- `"1234"` (no comma)

**Answer:**  
```
r'^\d{1,3}(,\d{3})*$'
```

## 20. How would you write a regex to match the full name of someone whose last name is Nakamoto?
Last name must be capitalized. First name must start with a capital letter.

Matches:
- “Satoshi Nakamoto”
- “Alice Nakamoto”

Not matches:
- “satoshi Nakamoto”
- “Mr. Nakamoto”
- “Nakamoto Satoshi”

**Answer:**  
```
r'^[A-Z][a-zA-Z]* Nakamoto$'
```

## 21. How would you write a regex to detect sentences where the first word begins with a capital letter and ends with a period?
Matches:
- “This is true.”
- “Cats are cool.”

Not matches:
- “this is not.”
- “No period”

**Answer:**  
```
r'^[A-Z][^.]*\.$'
```

## 22. How would you write a regex that matches a sentence where:
• First word is capitalized  
• There are at least three words  
• Ends with a period  
• Words are letters only  

**Answer:**  
```
r'^[A-Z][a-z]+( [a-z]+){2,}\.$'
```
