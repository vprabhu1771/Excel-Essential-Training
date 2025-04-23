The `MATCH` function in Excel is used to **find the position** of a value in a row or column — it returns the index (position), not the value itself.

---

### 🔹 MATCH Syntax:
```
MATCH(lookup_value, lookup_array, [match_type])
```

### ✅ Parameters:
- **`lookup_value`** – The value you want to find.
- **`lookup_array`** – The range (row or column) to search.
- **`[match_type]`** – Optional. 
  - `0` for exact match,
  - `1` for less than or equal to (ascending order),
  - `-1` for greater than or equal to (descending order).

---

### 🧠 Example:

| A     |
|-------|
| Apple |
| Banana|
| Cherry|

To find the **position** of `"Banana"` in A1:A3:

```
=MATCH("Banana", A1:A3, 0)
```

➡️ Returns **2**, because "Banana" is the second item in the list.

---

### ⚠️ Tips:
- `MATCH` is **case-insensitive**.
- Combine with `INDEX` for powerful lookups (`INDEX` returns value, `MATCH` returns position).
- Use `0` for most real-world cases where you need an exact match.

Would you like an example combining `INDEX` and `MATCH`?