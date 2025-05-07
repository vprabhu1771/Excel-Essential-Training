In Excel 2010, you can **create a new custom function** (called a **User Defined Function** or **UDF**) using **VBA (Visual Basic for Applications)**. Here's how you can do it:

---

### 🔧 Steps to Create a New Function in Excel 2010:

1. **Open Excel 2010** and press `ALT + F11` to open the **VBA Editor**.

2. In the VBA editor, go to `Insert` > `Module`.

3. In the new module window, type your custom function. Example:

   ```vba
   Function AddTwoNumbers(a As Double, b As Double) As Double
       AddTwoNumbers = a + b
   End Function
   ```

4. Press `CTRL + S` to save your workbook as **Macro-Enabled Workbook (`.xlsm`)**.

5. Go back to Excel. In any cell, you can now use your new function like this:

   ```
   =AddTwoNumbers(5, 3)
   ```

   ➜ This will return `8`.

---

### 📌 Notes:

* UDFs **cannot access Excel's built-in features** like formatting or inserting rows—only calculations.
* Make sure macros are **enabled** in Excel (via File > Options > Trust Center).

Would you like help writing a specific function?
