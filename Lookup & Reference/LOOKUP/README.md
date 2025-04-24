The older version of Excel (before Excel 2007) used the `LOOKUP()` function as one of the primary ways to search for values in a range. It’s a bit different from the more powerful and flexible `VLOOKUP()` or `XLOOKUP()` functions we commonly use now.

### Syntax of `LOOKUP()` (Legacy function):

```excel
LOOKUP(lookup_value, lookup_vector, [result_vector])
```

#### There are two forms of `LOOKUP()`:

1. **Vector Form:**
   ```excel
   LOOKUP(lookup_value, lookup_vector, result_vector)
   ```
   - `lookup_value`: The value you want to search for.
   - `lookup_vector`: A one-row or one-column range to search.
   - `result_vector`: A one-row or one-column range from which to return a value.

2. **Array Form (less common):**
   ```excel
   LOOKUP(lookup_value, array)
   ```
   - `array`: A range with at least two columns or rows. LOOKUP searches the first row or column.

### Limitations:
- Requires the `lookup_vector` to be **sorted in ascending order**.
- It only returns the **last exact match** or the **largest value less than or equal to** the lookup value.
- No ability to search in reverse order.
- Less error handling compared to `VLOOKUP()`, `HLOOKUP()`, or `XLOOKUP()`.

### Example:

```excel
=LOOKUP(40, A1:A5, B1:B5)
```

If column A has ages and column B has names, this formula looks for age 40 in A1:A5 and returns the corresponding name from B1:B5.

---

Would you like to see how this compares to `VLOOKUP()` or `XLOOKUP()` in a sample sheet?
