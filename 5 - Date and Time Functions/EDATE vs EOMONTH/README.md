In Excel, both `EDATE()` and `EOMONTH()` are functions used to add (or subtract) a number of months to a date. Here's how they differ and how to use them:

---

### ✅ `EDATE(start_date, months)`
- **Purpose**: Adds or subtracts a specific number of months to a date.
- **Returns**: A date that is the same day of the month, `n` months before or after the start date.

**Example**:
```excel
=EDATE("2024-01-15", 3)
```
🔹 Result: `2024-04-15`  
(Adds 3 months to Jan 15, 2024)

You can also subtract months:
```excel
=EDATE("2024-01-15", -2)
```
🔹 Result: `2023-11-15`

---

### ✅ `EOMONTH(start_date, months)`
- **Purpose**: Returns the last day of the month, `n` months before or after the start date.
- **Returns**: The **end of month** date.

**Example**:
```excel
=EOMONTH("2024-01-15", 2)
```
🔹 Result: `2024-03-31`  
(Returns last day of March)

```excel
=EOMONTH("2024-01-15", -1)
```
🔹 Result: `2023-12-31`

---

### 🔄 Summary:
| Function     | Adds Months | Returns               |
|--------------|-------------|------------------------|
| `EDATE()`    | ✅           | Same day of month     |
| `EOMONTH()`  | ✅           | End of resulting month|

Let me know if you want to use these with cell references or auto-fill a column!
