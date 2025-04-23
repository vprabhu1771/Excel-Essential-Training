Using `VLOOKUP` with `MATCH` is a powerful combo when the **column index** in your `VLOOKUP` needs to be **dynamic** — especially useful if your data layout might change or you want to look up columns by name.

---

### 🔹 Why combine them?
Instead of hardcoding the column index in `VLOOKUP`, use `MATCH` to **automatically find the column number** based on the header name.

---

### 🧠 Example:

| A     | B        | C       | D      |
|-------|----------|---------|--------|
| ID    | Name     | Age     | Salary |
| 1     | Alice    | 25      | 50K    |
| 2     | Bob      | 30      | 60K    |
| 3     | Charlie  | 28      | 55K    |

Suppose you want to look up Bob's **Salary**, but you want to dynamically specify the column (e.g. by typing "Salary" somewhere).

---

### ✅ Step-by-step:

Let’s say:

- Lookup value is in `G1`: `2` (Bob’s ID)
- Column name is in `G2`: `"Salary"`

Then use:

```excel
=VLOOKUP(G1, A2:D4, MATCH(G2, A1:D1, 0), FALSE)
```

### 🔍 What happens:
- `MATCH(G2, A1:D1, 0)` finds the **column number** of `"Salary"` → returns `4`.
- `VLOOKUP` uses that 4 as its column index → returns **"60K"**.

---

### 🔥 Bonus Tip:
This setup is super flexible — you can change the column you're fetching (Age, Name, etc.) just by editing one cell (`G2` in this case)!

Want me to make an editable Excel file with this example?