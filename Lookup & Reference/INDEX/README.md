Sure! Here's a simple and clear example to help you understand how **`INDEX()`** works in Excel.

---

### 📊 **Sample Data**

| A        | B     |
|----------|-------|
| Product  | Price |
| Apple    | 100   |
| Banana   | 40    |
| Orange   | 60    |
| Mango    | 80    |

---

### ✅ **Basic `INDEX()` Formula**

```excel
=INDEX(B2:B5, 2)
```

---

### 🔍 **Explanation**

- `B2:B5` → the range you're indexing into
- `2` → the row number (within the selected range)

So, this formula returns the **2nd value** in the range `B2:B5`.

✅ **Result**: `40` (which is the price of Banana)

---

### 🧠 Pro Tip: `INDEX()` with 2D Range

If you have a table like:

|        | A        | B      |
|--------|----------|--------|
| 1      | Product  | Price  |
| 2      | Apple    | 100    |
| 3      | Banana   | 40     |
| 4      | Orange   | 60     |
| 5      | Mango    | 80     |

This formula:

```excel
=INDEX(A2:B5, 3, 2)
```

Means:
- 3rd row of the range → Orange
- 2nd column of the range → Price

✅ **Result**: `60`

---

Want to try `INDEX()` with `MATCH()` or inside a dynamic dropdown list next?
