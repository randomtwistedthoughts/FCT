---
assignment: Python Basics
---

# Practice Questions

Answers

1.  Problem 1
    -   Answer:\
        Operators: `*`, `-`, `/`, `+`\
        Values: `'hello'`, `-88.8`, `5`

    -   Explanation:

        ``` text
        Operators perform actions on values (like +, -, *, /). Values are data 
        such as numbers or strings.
        ```
2.  Problem 2 --- Variable vs. String
    -   Answer:\
        Variable: `spam`\
        String: `'spam'`

    -   Explanation:

        ``` text
        Quoted text is a string; unquoted names refer to variables.
        ```
3.  Problem 3
    -   Answer: `int`, `float`, `str`

    -   Explanation:

        ``` text
        These are Python’s basic built-in types for whole numbers, decimals, and text.
        ```
4.  Problem 4
    -   Answer:

        ``` text
        An expression consists of values and operators, and always evaluates to a 
        single resulting value.
        ```
5.  Problem 5
    -   Answer:

        ``` text
        An expression returns a value. A statement performs an action, such as a 
        variable assignment, and may not return a value.
        ```
6.  Problem 6
    -   Answer: `20`

    -   Explanation:

        ``` text
        "bacon + 1" is evaluated but never assigned back to bacon, so bacon stays 20.
        ```
7.  Problem 7
    -   Answer:\
        `'spam' + 'spamspam'` → `'spamspamspam'`\
        `'spam' * 3` → `'spamspamspam'`

    -   Explanation:

        ``` text
        + concatenates strings; * repeats a string multiple times.
        ```
8.  Problem 8
    -   Answer:

        ``` text
        "eggs" is valid; "100" is invalid.
        ```

    -   Explanation:

        ``` text
        Variable names cannot start with digits; they must start with a letter or underscore.
        ```
9.  Problem 9
    -   Answer: `int()`, `float()`, `str()`

    -   Explanation:

        ``` text
        These functions convert values to integer, floating-point, or string types.
        ```
10. Problem 10
    -   Answer:

        ``` text
        'I have eaten ' + str(99) + ' burritos.'
        ```

        or

        ``` text
        f'I have eaten {99} burritos.'
        ```

    -   Explanation:

        ``` text
        Strings cannot be concatenated with integers, so 99 must be converted to a string 
        or placed inside an f-string.
        ```
