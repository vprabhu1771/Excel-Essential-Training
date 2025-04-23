Perfect! Combining `HLOOKUP` with `MATCH` works similarly to `VLOOKUP + MATCH`, but for **horizontal** data layouts. It lets you dynamically find the **row number** to return based on a header value.

---

### 🔹 Scenario:
Use `HLOOKUP` when your data is laid out **horizontally** and you want to **look up a row by name** instead of hardcoding the row number.

---

### 🧠 Example:

|     | A       | B       | C        |
|-----|---------|---------|----------|
| 1   | ID      | 1       | 2        |
| 2   | Name    | Alice   | Bob      |
| 3   | Age     | 25      | 30       |
| 4   | Salary  | 50K     | 60K      |

You want to:
- Look up the value for **ID = 2**
- Return the data from a row name like `"Salary"` — typed in a separate cell

---

### ✅ Suppose:
- `G1`: `2` (lookup ID)
- `G2`: `"Salary"` (row label)

Use this formula:

```excel
=HLOOKUP(G1, B1:C4, MATCH(G2, A1:A4, 0), FALSE)
```

### 🔍 What happens:
- `MATCH(G2, A1:A4, 0)` → finds the row number of `"Salary"` → returns `4`
- `HLOOKUP(G1, B1:C4, 4, FALSE)` → finds the value in row 4 and the column where ID = 2 → returns **60K**

---

### 🔥 Why it’s cool:
- You can easily change `"Salary"` to `"Age"` or `"Name"` in G2 and the formula still works.
- No need to manually count rows anymore!

Would you like me to share a downloadable `.xlsx` sample file with this in action?