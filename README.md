# Rename Duplicated Column Names

This UiPath project identifies duplicate column names in an Excel file, renames them to be unique by adding round brackets and numbers. 

## How It Works

1. The workflow reads the header row of table based on the provided path, sheet name, and header row.
2. It identifies any duplicate column names.
3. Duplicate column names are renamed to unique names to ensure clarity and ease of use For example as; Name (1) Name (2)
4. The updated column names are saved back to the Excel file.
5. After execution, the Excel file's column headers will have unique, readable names.

## Input Parameters

![inputs](https://github.com/user-attachments/assets/11d92dd0-e17e-4d4b-95bb-bd5051a37064)

- **ExcelFilePath** (String): The path to the Excel file where the columns will be renamed.
- **Sheetname** (String): The name of the sheet that contains the table.
- **Header Row** (Integer): The starting row of the table headers. For example, 1 is the first row of the Excel sheet.

## Example

Suppose you have an Excel sheet with the following setup:
- File Path: `C:\Users\Example\Documents\Test.xlsx`
- Sheet Name: `Sheet1`
- Header Row: 1

![example1](https://github.com/user-attachments/assets/bc831fdc-42b0-4c5a-b78a-70e216e3236b)

If the file contains duplicate columns like `Name`, `Name`, the workflow will rename these columns to `Name (1)`, `Name (2)` to make them unique.

![image](https://github.com/user-attachments/assets/896874a4-704f-4597-b3ae-32d540a17c8e)

---


