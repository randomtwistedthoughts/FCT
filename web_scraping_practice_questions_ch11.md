# Web Scraping — Practice Questions & Answers (Chapter 11)

## 1. Briefly describe the differences between the webbrowser, requests, BeautifulSoup, and selenium modules.
**Answer:**  
- `webbrowser` opens web pages in a browser.  
- `requests` downloads web content.  
- `BeautifulSoup` parses and extracts data from HTML.  
- `selenium` automates a real browser and interacts with web pages.

## 2. What type of object is returned by `requests.get()`? How can you access the downloaded content as a string?
**Answer:**  
It returns a `Response` object.  
Use `.text` to get the content as a string.

## 3. What Requests method checks that the download worked?
**Answer:** `raise_for_status()`

## 4. How can you get the HTTP status code of a Requests response?
**Answer:** Using `response.status_code`

## 5. How do you save a Requests response to a file?
**Answer:**  
```python
with open('file.html', 'wb') as f:
    for chunk in response.iter_content(100000):
        f.write(chunk)
```

## 6. What is the keyboard shortcut for opening a browser’s developer tools?
**Answer:**  
- Windows/Linux: `Ctrl + Shift + I`  
- Mac: `Cmd + Option + I`

## 7. How can you view (in developer tools) the HTML of a specific element on a web page?
**Answer:** Right-click the element → **Inspect**.

## 8. What is the CSS selector string that would find the element with an id attribute of `main`?
**Answer:** `#main`

## 9. What is the CSS selector string that would find the elements with a CSS class of `highlight`?
**Answer:** `.highlight`

## 10. What is the CSS selector string that would find all the `<div>` elements inside another `<div>` element?
**Answer:** `div div`

## 11. What is the CSS selector string that would find the `<button>` element with a value attribute set to `favorite`?
**Answer:** `button[value="favorite"]`

## 12. Say you have a Beautiful Soup Tag object stored in `spam` for `<div>Hello world!</div>`. How could you get the string `Hello world!` from the Tag object?
**Answer:** `spam.getText()` or `spam.text`

## 13. How would you store all the attributes of a Beautiful Soup Tag object in a variable?
**Answer:** `tag.attrs`

## 14. Running `import selenium` doesn’t work. How do you properly import the selenium module?
**Answer:**  
```python
from selenium import webdriver
```

## 15. What’s the difference between the `find_element_*` and `find_elements_*` methods?
**Answer:**  
- `find_element_*` returns one element  
- `find_elements_*` returns a list of elements

## 16. What methods do Selenium’s WebElement objects have for simulating mouse clicks and keyboard keys?
**Answer:**  
- Mouse click: `.click()`  
- Keyboard input: `.send_keys()`

## 17. You could call `send_keys(Keys.ENTER)` on the Submit button’s WebElement object, but what is an easier way to submit a form with Selenium?
**Answer:** Use the `.submit()` method.

## 18. How can you simulate clicking a browser’s Forward, Back, and Refresh buttons with Selenium?
**Answer:**  
```python
driver.forward()
driver.back()
driver.refresh()
```
