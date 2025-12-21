# Debugging — Practice Questions & Answers

## 1. What is a bug?
**Answer:** A bug is an error or defect in a program that causes it to behave incorrectly or crash.

## 2. What are the three main types of errors?
**Answer:**  
- Syntax errors  
- Runtime errors  
- Logic errors

## 3. What is a syntax error?
**Answer:** An error caused by invalid Python grammar that prevents the program from running.

## 4. What is a runtime error?
**Answer:** An error that occurs while the program is running, often causing it to crash.

## 5. What is a logic error?
**Answer:** An error where the program runs without crashing but produces incorrect results.

## 6. What does the traceback show?
**Answer:** It shows the sequence of function calls that led to the error and where the error occurred.

## 7. What is an exception?
**Answer:** An error detected during execution that interrupts the normal flow of the program.

## 8. What does `try` / `except` do?
**Answer:** It allows the program to handle errors gracefully instead of crashing.

## 9. What does the `assert` statement do?
**Answer:** It checks that a condition is true and raises an error if it is not.

## 10. Why should you avoid using `assert` for input validation?
**Answer:** Because assertions can be disabled, making them unreliable for validating user input.

## 11. What is logging?
**Answer:** Logging records information about program execution for debugging and monitoring.

## 12. What are the five logging levels?
**Answer:** DEBUG, INFO, WARNING, ERROR, CRITICAL

## 13. What does `logging.debug()` do?
**Answer:** Logs low-level information useful for debugging.

## 14. What is the benefit of using logging instead of print()?
**Answer:** Logging can be enabled or disabled easily and provides more control over output.

## 15. What does `pdb.set_trace()` do?
**Answer:** Pauses program execution and opens the interactive debugger.
