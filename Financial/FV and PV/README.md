To calculate **Future Value (FV)** and **Present Value (PV)** in Excel for a payment of ₹5,00,000 INR, you can use the built-in Excel functions `FV()` and `PV()`.

Let’s break down both:

---

### 🧮 1. **Future Value (FV)** Formula:
```
=FV(rate, nper, pmt, [pv], [type])
```

#### Example:
Assume:
- Rate = 8% annual interest (i.e., 0.08)
- NPER = 5 years
- PMT = 0 (if you're investing once)
- PV = -500000 (₹5,00,000 is a one-time investment)

```excel
=FV(0.08, 5, 0, -500000)
```

**Result**: ₹7,34,664.03 (approx)

---

### 🧮 2. **Present Value (PV)** Formula:
```
=PV(rate, nper, pmt, [fv], [type])
```

#### Example:
Assume:
- You want ₹5,00,000 in the future
- Rate = 8%
- NPER = 5 years
- FV = 500000

```excel
=PV(0.08, 5, 0, 500000)
```

**Result**: ₹3,40,278.19 (approx)

---

### Quick Notes:
- Use **negative sign** for money paid/invested (`PV`), and positive for amount you will receive (`FV`)
- `PMT` is set to 0 because this is a **one-time payment**, not a recurring one.

Want to try this with monthly payments or change the interest compounding frequency? Let me know!
