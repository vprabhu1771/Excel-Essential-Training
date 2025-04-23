Great! `HLOOKUP` is similar to `VLOOKUP`, but instead of searching **vertically** in columns, it searches **horizontally** in rows.

---

### 🔹 HLOOKUP Syntax:
```
HLOOKUP(lookup_value, table_array, row_index_num, [range_lookup])
```

### ✅ Parameters:
- **`lookup_value`** – The value you want to search for (in the first row).
- **`table_array`** – The range of cells that contains the data.
- **`row_index_num`** – The row number in the table from which to return the value.
- **`[range_lookup]`** – Optional. TRUE (approximate match) or FALSE (exact match).

---

### 🧠 Example:

|      | A     | B      | C      |
|------|-------|--------|--------|
| 1    | ID    | 1      | 2      |
| 2    | Name  | Alice  | Bob    |
| 3    | Age   | 25     | 30     |

If you want to find the **Name** of the person with **ID = 2**:

```
=HLOOKUP(2, A1:C3, 2, FALSE)
```

➡️ This returns **Bob**, since 2 is found in the first row and the 2nd row has the name.

---

### ⚠️ Tips:
- Use **HLOOKUP** when your data is arranged in **rows**.
- Like `VLOOKUP`, you should use **FALSE** for exact matches.
- `XLOOKUP` can replace both `VLOOKUP` and `HLOOKUP` in Excel 365 and Excel 2019+.

Want a quick comparison of `VLOOKUP` vs `HLOOKUP` or a sample sheet?