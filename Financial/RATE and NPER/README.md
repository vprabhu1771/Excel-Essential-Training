Let’s walk through examples using **`RATE()`** and **`NPER()`** functions in Excel to calculate:

- **`RATE()`**: Find the **interest rate** when you know the payment, loan amount, and term.
- **`NPER()`**: Find the **number of periods** (months) when you know the payment, loan amount, and interest rate.

---

### 🔹 Example 1: `RATE()` – Find the Interest Rate

**Scenario**:  
You are paying ₹15,000 per month for a ₹5,00,000 loan for 4 years. What is the annual interest rate?

#### Inputs:
- **PMT** = ₹15,000  
- **Loan Amount (PV)** = ₹5,00,000  
- **Loan Term (Years)** = 4 → 4 × 12 = 48 months  
- **FV** = 0 (fully paid off)

#### Formula:
```excel
=RATE(48, -15000, 500000) * 12
```

> Multiply by 12 to get **annual rate** from monthly rate.

---

### 🔹 Example 2: `NPER()` – Find the Number of Months

**Scenario**:  
You took a ₹8,00,000 loan with an annual interest rate of 7%, and you pay ₹12,000 per month. How many months will it take to repay?

#### Inputs:
- **PMT** = ₹12,000  
- **Loan Amount (PV)** = ₹8,00,000  
- **Interest Rate per Month** = 7% / 12 = 0.5833%  
- **FV** = 0

#### Formula:
```excel
=NPER(7%/12, -12000, 800000)
```

> Result gives number of **months** required to repay.

---

### Notes:
- Payments (`PMT`) should be **negative** if you're paying out money.
- Loan amount (`PV`) should be **positive** if it's money you receive.
- Future Value (`FV`) is usually 0 for fully paid loans.

Let me know if you'd like a template or sample Excel file too!