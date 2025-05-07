Here’s a practical example using Excel **logical and conditional functions** with **student results**, where subjects include **English, Tamil, Math, Social, and Science**.

---

### 🎓 **Sample Data**

| Student | English | Tamil | Math | Social | Science |
| ------- | ------- | ----- | ---- | ------ | ------- |
| John    | 65      | 58    | 80   | 70     | 55      |
| Priya   | 45      | 38    | 50   | 42     | 39      |
| Arjun   | 90      | 88    | 91   | 85     | 87      |
| Divya   | 30      | 40    | 25   | 38     | 35      |
| Ravi    | 60      | 65    | 70   | 68     | 62      |

---

### ✅ **1. IF()** — Basic pass/fail check per subject

**Formula (for English pass/fail):**

```excel
=IF(B2>=40, "Pass", "Fail")
```

---

### ✅ **2. IFS()** — Grade based on average

**Formula (average grade logic):**

```excel
=IFS(AVERAGE(B2:F2)>=90, "A+", AVERAGE(B2:F2)>=75, "A", AVERAGE(B2:F2)>=60, "B", AVERAGE(B2:F2)>=40, "C", TRUE, "Fail")
```

---

### ✅ **3. IFERROR()** — Handle errors (e.g., division by zero)

**Formula (safe average calculation):**

```excel
=IFERROR(AVERAGE(B2:F2), "Error in Marks")
```

---

### ✅ **4. SWITCH()** — Map grade letter to description

**Formula (assuming grade is in G2):**

```excel
=SWITCH(G2, "A+", "Excellent", "A", "Very Good", "B", "Good", "C", "Average", "Fail", "Needs Improvement")
```

---

### ✅ **5. AND() / OR() / NOT()** — Combine multiple logic conditions

**Formula (Check if student passed all subjects):**

```excel
=IF(AND(B2>=40, C2>=40, D2>=40, E2>=40, F2>=40), "Pass", "Fail")
```

**Formula (Check if failed at least one subject):**

```excel
=IF(OR(B2<40, C2<40, D2<40, E2<40, F2<40), "Fail", "Pass")
```

**Formula (Using NOT):**

```excel
=IF(NOT(B2<40), "Passed English", "Failed English")
```

---

### ✅ **6. XOR()** — Exclusive OR (e.g., failed in exactly one subject)

**Formula (fail in exactly one subject):**

```excel
=XOR(B2<40, C2<40, D2<40, E2<40, F2<40)
```

🔹 This returns `TRUE` only if an **odd number** of conditions are true. For exactly one fail, you'd do a more complex count:

```excel
=IF(COUNTIF(B2:F2,"<40")=1, "One Subject Fail", "Other Case")
```

---

Would you like a downloadable Excel file with this example filled in?
