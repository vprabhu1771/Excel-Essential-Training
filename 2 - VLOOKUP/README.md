The `VLOOKUP` function in Excel is used to **search for a value in the first column of a range** and return a value in the same row from a specified column.

### 🔹 VLOOKUP Syntax:
```
VLOOKUP(lookup_value, table_array, col_index_num, [range_lookup])
```

### ✅ Parameters:
- **`lookup_value`** – The value you want to search for.
- **`table_array`** – The range of cells that contains the data.
- **`col_index_num`** – The column number in the range from which to return the value.
- **`[range_lookup]`** – Optional. TRUE (approximate match) or FALSE (exact match).

---

### 🧠 Example:

| ID | Name     | Age |
|----|----------|-----|
| 1  | Alice    | 25  |
| 2  | Bob      | 30  |
| 3  | Charlie  | 28  |

If you want to find the **Age** of the person with **ID = 2**:

```
=VLOOKUP(2, A2:C4, 3, FALSE)
```

➡️ This returns **30**, which is Bob’s age.

---

### ⚠️ Tips:
- Make sure the **lookup column is the first column** in your `table_array`.
- Use **FALSE** if you need an exact match.
- For modern Excel versions, `XLOOKUP` is recommended as it's more flexible.

Would you like a real-world use case or an Excel file demo?