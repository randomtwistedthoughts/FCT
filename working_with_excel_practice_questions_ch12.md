# Working with Excel Spreadsheets — Practice Questions & Answers (Chapter 12)

## 1. What does the `openpyxl.load_workbook()` function return?
**Answer:** A `Workbook` object.

## 2. What does the `get_sheet_names()` workbook method return?
**Answer:** A list of worksheet names.

## 3. How would you retrieve the Worksheet object for a sheet named `'Sheet1'`?
**Answer:**  
```python
wb['Sheet1']
```

## 4. How would you retrieve the Worksheet object for the workbook’s active sheet?
**Answer:**  
```python
wb.active
```

## 5. How would you retrieve the value in cell C5?
**Answer:**  
```python
sheet['C5'].value
```

## 6. How would you set the value in cell C5 to `"Hello"`?
**Answer:**  
```python
sheet['C5'] = 'Hello'
```

## 7. How would you retrieve the cell’s row and column as integers?
**Answer:**  
```python
cell.row, cell.column
```

## 8. What do the `get_highest_column()` and `get_highest_row()` sheet methods return, and what is the data type of these return values?
**Answer:**  
They return the highest used column and row numbers as **integers**.

## 9. If you needed to get the integer index for column `"M"`, what function would you call?
**Answer:**  
```python
openpyxl.utils.column_index_from_string('M')
```

## 10. If you needed to get the string name for column 14, what function would you call?
**Answer:**  
```python
openpyxl.utils.get_column_letter(14)
```

## 11. How can you retrieve a tuple of all the Cell objects from A1 to F1?
**Answer:**  
```python
sheet['A1':'F1']
```

## 12. How would you save the workbook to the filename `example.xlsx`?
**Answer:**  
```python
wb.save('example.xlsx')
```

## 13. How would you set a formula in a cell?
**Answer:**  
```python
sheet['A1'] = '=SUM(B1:B5)'
```

## 14. If you want to retrieve the result of a cell’s formula instead of the cell’s formula itself, what must you do first?
**Answer:** Open the workbook with `data_only=True`.

## 15. How would you set the height of row 5 to 100?
**Answer:**  
```python
sheet.row_dimensions[5].height = 100
```

## 16. How would you hide column C?
**Answer:**  
```python
sheet.column_dimensions['C'].hidden = True
```

## 17. Name a few features that OpenPyXL 2.1.4 does not load from a spreadsheet file.
**Answer:** Images, charts, comments, pivot tables, macros.

## 18. What is a freeze pane?
**Answer:** A frozen row/column that stays visible when scrolling.

## 19. What five functions and methods do you have to call to create a bar chart?
**Answer:**  
```text
openpyxl.chart.BarChart()
openpyxl.chart.Reference()
chart.add_data()
sheet.add_chart()
wb.save()
```
