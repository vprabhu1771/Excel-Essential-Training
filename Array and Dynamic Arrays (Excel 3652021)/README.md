Here’s a breakdown with **Excel 365/2021** dynamic array function examples that you can copy and test directly in Excel:

---

### 🔍 **1. `FILTER()` – Filter array based on criteria**

**Example:**

| A    | B     |
| ---- | ----- |
| Name | Score |
| John | 85    |
| Jane | 70    |
| John | 90    |

```excel
=FILTER(A2:B4, A2:A4="John")
```

➡ Filters only rows where Name = "John"

---

### 🔢 **2. `SORT()` / `SORTBY()` – Sort dynamically**

**`SORT()` Example:**

```excel
=SORT(A2:B4, 2, -1)
```

➡ Sorts range A2\:B4 by **Score** in descending order.

**`SORTBY()` Example:**

```excel
=SORTBY(A2:B4, B2:B4, 1)
```

➡ Sorts A2\:B4 **by the Score column in ascending order**, but lets you sort based on columns not included in the result too.

---

### 🆔 **3. `UNIQUE()` – Extract unique values**

**Example:**

```excel
=UNIQUE(A2:A5)
```

If column A has names like John, Jane, John, it returns:

```
John
Jane
```

---

### 📈 **4. `SEQUENCE()` – Generate sequential numbers**

**Example:**

```excel
=SEQUENCE(5)
```

➡ Returns a vertical array from 1 to 5:

```
1  
2  
3  
4  
5
```

```excel
=SEQUENCE(3, 2, 10, 5)
```

➡ Creates a 3×2 array starting at 10, step 5:

```
10   15  
20   25  
30   35
```

---

### 🎲 **5. `RANDARRAY()` – Generate random array**

**Example:**

```excel
=RANDARRAY(3, 2, 1, 100, TRUE)
```

➡ 3 rows × 2 columns of random **integers** from 1 to 100

---

### 🧮 **6. `LET()` – Define variables in formulas**

**Example:**

```excel
=LET(x, 5, y, 10, x + y)
```

➡ Sets `x = 5`, `y = 10`, result is `15`.

---

### 🔧 **7. `LAMBDA()` – Create custom functions**

**Example (inside a named formula):**

```excel
=LAMBDA(x, x^2)(4)
```

➡ Returns `16`, squares the number.

Or use with `LET()` for clarity:

```excel
=LET(Square, LAMBDA(x, x^2), Square(5))
```

To reuse a LAMBDA, define it in **Formulas > Name Manager**, then call it like a normal function:

```excel
=MySquare(6)
```

---

Would you like these examples in a pre-made Excel workbook?
