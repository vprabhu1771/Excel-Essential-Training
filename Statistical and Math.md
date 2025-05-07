Here's a breakdown and examples of each Excel function you listed, explained clearly with formulas you can try directly in Excel:

---

### 🔢 **Conditional Aggregation**

#### **`SUMIFS()` / `COUNTIFS()` / `AVERAGEIFS()`**

These functions calculate totals **based on multiple conditions**.

| A    | B     | C      |
| ---- | ----- | ------ |
| Name | Score | Status |
| John | 80    | Pass   |
| Jane | 70    | Fail   |
| John | 90    | Pass   |

* **`=SUMIFS(B2:B4, A2:A4, "John")`** → Sums scores where name is John → `170`
* **`=COUNTIFS(C2:C4, "Pass")`** → Counts how many "Pass" → `2`
* **`=AVERAGEIFS(B2:B4, C2:C4, "Pass")`** → Averages scores with status "Pass" → `(80+90)/2 = 85`

---

### 🏅 **Ranking Numbers**

#### **`RANK.EQ()` / `RANK.AVG()`**

| A  |
| -- |
| 85 |
| 70 |
| 85 |
| 60 |

* **`=RANK.EQ(A2, A2:A5)`** → Ranks 85 → `1` (same rank for same values)
* **`=RANK.AVG(A2, A2:A5)`** → Averages rank for duplicates → `1.5`

---

### 📊 **Nth Largest/Smallest**

#### **`LARGE()` / `SMALL()`**

| A   |
| --- |
| 45  |
| 100 |
| 70  |
| 85  |

* **`=LARGE(A2:A5, 2)`** → 2nd largest → `85`
* **`=SMALL(A2:A5, 3)`** → 3rd smallest → `85`

---

### ➗ **Rounding Functions**

#### **`ROUND()`, `ROUNDUP()`, `ROUNDDOWN()`**

* **`=ROUND(3.456, 2)`** → `3.46`
* **`=ROUNDUP(3.456, 2)`** → `3.46`
* **`=ROUNDDOWN(3.456, 2)`** → `3.45`

---

### 🧮 **Integer, Modulo, Truncate**

#### **`INT()`, `MOD()`, `TRUNC()`**

* **`=INT(5.9)`** → `5` (round down to nearest integer)
* **`=MOD(10, 3)`** → `1` (remainder of division)
* **`=TRUNC(5.678, 1)`** → `5.6` (cuts after 1 decimal place)

---

### ✅ **Conditional Totals**

#### **`SUBTOTAL()`**

| A   |
| --- |
| 100 |
| 200 |
| 300 |

* **`=SUBTOTAL(9, A1:A3)`** → `600` (9 = SUM; 1 = AVERAGE, 2 = COUNT, etc.)
* Works well when rows are **filtered**.

---

### 🧠 **Advanced Aggregation**

#### **`AGGREGATE()`**

* **`=AGGREGATE(9, 6, A1:A3)`** → `600`

  * 9 = SUM
  * 6 = Ignore errors
* Can be used to calculate things like MAX, MIN, etc. with filtered rows or ignoring errors.

---

### 🔢 **Round to Multiples**

#### **`FLOOR()`, `CEILING()`**

* **`=FLOOR(7.8, 0.5)`** → `7.5` (round down to nearest 0.5)
* **`=CEILING(7.8, 0.5)`** → `8.0` (round up to nearest 0.5)

---

Would you like a downloadable Excel file with these examples filled in?
