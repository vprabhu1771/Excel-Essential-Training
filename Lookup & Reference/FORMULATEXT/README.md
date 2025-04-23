The **`FORMULATEXT()`** function in Excel is used to display the formula that is in a specific cell as a text string. This is particularly useful when you want to see the actual formula behind the value in a cell without having to edit it.

---

### **Syntax:**

```excel
FORMULATEXT(reference)
```

| Parameter    | Description                                   |
|--------------|-----------------------------------------------|
| `reference`  | The cell containing the formula you want to display |

---

### **Example 1: Simple Formula Display**

Let's say you have a formula in cell `B2` that adds two numbers:

```excel
= A2 + A3
```

Now, if you want to display the formula used in `B2` in another cell (let’s say `C2`), you would use the `FORMULATEXT()` function:

#### **Formula in `C2`:**
```excel
=FORMULATEXT(B2)
```

- This will return the formula **`= A2 + A3`** as a text string in cell `C2`, rather than showing the result of the calculation (which would be the sum of `A2` and `A3`).

---

### **Example 2: Display Formula in a Range**

If you want to show the formula for each cell in a column that contains a formula, you can use `FORMULATEXT()` alongside a range. For example, if column `B` contains formulas, and you want to display those formulas in column `C`:

#### **Formula in `C2`:**
```excel
=FORMULATEXT(B2)
```

- When copied down, this will show the formulas from column `B` as text in column `C`.

---

### **Important Notes:**
- If the reference cell does not contain a formula, `FORMULATEXT()` will return the **`#N/A`** error.
- This function is useful when documenting or auditing your spreadsheets, as it helps you keep track of the formulas used.

---

Would you like to see an example of using `FORMULATEXT()` in a more advanced setup, like auditing multiple formulas or combining it with other functions?