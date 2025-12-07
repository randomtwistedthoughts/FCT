# Reading and Writing Files — Practice Questions & Answers

## 1. What is the difference between `shutil.copy()` and `shutil.copytree()`?
**Answer:**  
- `shutil.copy()` copies a single file.  
- `shutil.copytree()` copies an entire folder and all of its contents.  
**Explanation:** `copy()` works on individual files, while `copytree()` recursively copies directories.

## 2. What function is used to rename files?
**Answer:** `os.rename()`  
**Explanation:** This function renames a file or moves it to a new location.

## 3. What is the difference between the delete functions in the `send2trash` and `shutil` modules?
**Answer:**  
- `send2trash` moves files to the Recycle Bin/Trash.  
- `shutil` delete functions (`shutil.rmtree()`, `os.remove()`) permanently delete files.  
**Explanation:** `send2trash` is safer because it allows recovery.

## 4. ZipFile objects have a close() method just like file objects. What ZipFile method is equivalent to file objects’ open() method?
**Answer:** `zipfile.ZipFile()`  
**Explanation:** Opening a ZIP archive with `zipfile.ZipFile('file.zip', 'r')` is like opening a file with `open()`.
