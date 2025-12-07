---
assignment: Flow Control
---

# Practice Questions

Answers

1.  Problem 1
    -   Answer: `True` and `False`

    -   Explanation:

        ``` text
        Boolean values represent truth values and are written with capitalized first letters: True, False.
        ```
2.  Problem 2
    -   Answer: `and`, `or`, `not`

    -   Explanation:

        ``` text
        These are the three logical operators used to combine or modify Boolean expressions.
        ```
3.  Problem 3 --- Truth Tables
    -   Answer:

            AND:
            True and True   -> True
            True and False  -> False
            False and True  -> False
            False and False -> False

            OR:
            True or True   -> True
            True or False  -> True
            False or True  -> True
            False or False -> False

            NOT:
            not True  -> False
            not False -> True
4.  Problem 4 --- Evaluate Expressions
    -   Answer:

            (5 > 4) and (3 == 5)          -> False
            not (5 > 4)                    -> False
            (5 > 4) or (3 == 5)            -> True
            not ((5 > 4) or (3 == 5))      -> False
            (True and True) and (True == False) -> False
            (not False) or (not True)      -> True
5.  Problem 5 --- Comparison Operators
    -   Answer: `==`, `!=`, `<`, `>`, `<=`, `>=`
6.  Problem 6 --- Equal vs Assignment
    -   Answer:

        ``` text
        == checks equality between two values.
        = assigns a value to a variable.
        ```
7.  Problem 7 --- What is a Condition?
    -   Answer:

        ``` text
        A condition is a Boolean expression used in flow control statements to decide which code executes.
        ```
8.  Problem 8 --- Identify the Blocks
    -   Answer:

            Block 1: The "if spam == 10:" block
            Block 2: The nested "if spam > 5:" block
            Block 3: The "else:" block
9.  Problem 9 --- Print Based on spam
    -   Answer:

        ``` python
        if spam == 1:
            print("Hello")
        elif spam == 2:
            print("Howdy")
        else:
            print("Greetings!")
        ```
10. Problem 10 --- Breaking Infinite Loop\

-   Answer: `Ctrl + C`

11. Problem 11 --- break vs continue\

-   Answer:
    `text      break stops the entire loop.      continue skips the rest of the current iteration and moves to the next.`

12. Problem 12 --- range Variants\

-   Answer:
    `text      range(10)     -> 0 to 9      range(0, 10)  -> 0 to 9      range(0, 10, 1) -> 0 to 9, step 1      They all produce the same sequence.`

13. Problem 13 --- Print 1 to 10\

-   Answer:

    ``` python
    # for loop
    for i in range(1, 11):
        print(i)

    # equivalent while loop
    i = 1
    while i <= 10:
        print(i)
        i += 1
    ```

14. Problem 14 --- Calling bacon() from spam module\

-   Answer: `python      import spam      spam.bacon()`
