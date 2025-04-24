Absolutely! The combination of **`INDEX()` + `MATCH()`** is one of the most **powerful and flexible lookup techniques** in Excel — especially before `XLOOKUP()` became available. Here's a clear breakdown with an example:

---

### 🔍 **Use Case**: Look up the price of a product (like `XLOOKUP()`)

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

### ✅ **Formula Using INDEX + MATCH**

```excel
=INDEX(B2:B5, MATCH("Orange", A2:A5, 0))
```

---

### 🔍 **Explanation**

- `MATCH("Orange", A2:A5, 0)` → looks for "Orange" in `A2:A5`, returns the **position** (in this case, 3)
- `INDEX(B2:B5, 3)` → returns the **3rd item** in `B2:B5`, which is `60`

✅ **Result**: `60`

---

### 📌 **Why it's powerful**

- Works with **data in any direction** (not just left-to-right like `VLOOKUP`)
- Supports **dynamic ranges**
- Easily handles **2D lookups** with nested `MATCH()` functions (row + column)

---

### 📘 **Bonus: Cell Reference Example**

If `D1` contains `"Orange"`:

```excel
=INDEX(B2:B5, MATCH(D1, A2:A5, 0))
```

---

Want to see a 2D lookup example or compare it with `VLOOKUP`?
