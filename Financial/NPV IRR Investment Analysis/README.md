Sure! Here's a simple Excel example in **INR format** showing how to use `NPV()` and `IRR()` functions for **investment return analysis**.

---

### 🧮 Scenario:
You are investing ₹1,00,000 in a project today. The expected cash inflows over the next 5 years are:

| Year | Cash Flow (INR) |
|------|-----------------|
| 0    | -1,00,000       |
| 1    | 20,000          |
| 2    | 25,000          |
| 3    | 30,000          |
| 4    | 35,000          |
| 5    | 40,000          |

You want to calculate:
1. **NPV** at a discount rate of **10%**
2. **IRR** of the investment

---

### 📊 Excel Setup:

| A        | B             |
|----------|---------------|
| **Year** | **Cash Flow** |
| 0        | -100000       |
| 1        | 20000         |
| 2        | 25000         |
| 3        | 30000         |
| 4        | 35000         |
| 5        | 40000         |
|          |               |
| Discount Rate | 10%     |
| NPV      | =NPV(B8, B3:B7) + B2 |
| IRR      | =IRR(B2:B7)   |

> **Note**:
- `B2` is the initial investment (`Year 0`)
- `B3:B7` are future cash flows from Year 1 to 5
- `B8` is the discount rate (10%)

---

### 🧮 Calculation Explained:

- **NPV Formula**:  
  `=NPV(10%, 20000, 25000, 30000, 35000, 40000) + (-100000)`  
  This gives the **Net Present Value**.

- **IRR Formula**:  
  `=IRR({-100000, 20000, 25000, 30000, 35000, 40000})`  
  This gives the **Internal Rate of Return**.

---

Would you like a downloadable `.xlsx` file with this example already built in?
