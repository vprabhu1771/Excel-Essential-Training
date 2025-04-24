Sure! Here's a simple **`XLOOKUP()`** example in Excel to help you understand how it works.

### 🔍 **Use Case**: Find the price of a product by its name.

---

### 📊 **Sample Data**

| Product   | Price |
|-----------|-------|
| Apple     | 100   |
| Banana    | 40    |
| Orange    | 60    |
| Mango     | 80    |

---

### ✅ **Formula**

To find the price of **"Orange"**, you would use:

```excel
=XLOOKUP("Orange", A2:A5, B2:B5)
```

---

### 🔍 **Explanation**

- `"Orange"` → the value you're searching for
- `A2:A5` → the range to search (lookup array)
- `B2:B5` → the range to return the result from (return array)

✅ **Result**: `60`

---

### Bonus: Using a Cell Reference

If `"Orange"` is in cell `D1`, use:

```excel
=XLOOKUP(D1, A2:A5, B2:B5)
```

Let me know if you'd like an example with `IF_NOT_FOUND`, `MATCH_MODE`, or `SEARCH_MODE`!
