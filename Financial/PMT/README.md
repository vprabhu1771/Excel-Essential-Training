The `PMT()` function in Excel is used to calculate the monthly payment for a loan based on constant payments and a constant interest rate. Here's how you can set up an example for a housing loan calculation:

### Formula Syntax:
```
=PMT(rate, nper, pv, [fv], [type])
```

- **rate**: The interest rate for each period. For a monthly payment, it's the annual interest rate divided by 12.
- **nper**: The number of periods (months) for the loan.
- **pv**: The present value, or the total loan amount.
- **fv** (optional): The future value (remaining loan balance after the last payment). Default is 0.
- **type** (optional): 0 if payments are due at the end of the period (default), 1 if payments are due at the beginning.

### Example: Housing Loan
Suppose you have the following loan details:
- **Loan Amount (Principal)**: ₹5,00,000
- **Annual Interest Rate**: 6% per year
- **Loan Term**: 20 years (240 months)

### Steps:
1. **Interest Rate per Month**: `6% / 12 = 0.5%` (monthly rate)
2. **Number of Payments (Months)**: `20 years * 12 = 240 months`
3. **Loan Amount**: ₹5,00,000

#### In Excel:

1. Enter the following data:
   - Cell A1: **Loan Amount**: 500000
   - Cell A2: **Interest Rate (Annual)**: 6%
   - Cell A3: **Loan Term (Years)**: 20

2. In cell A4, calculate the **monthly interest rate**:
   ```
   =A2 / 12 / 100
   ```
   
3. In cell A5, calculate the **number of months**:
   ```
   =A3 * 12
   ```

4. In cell A6, calculate the **monthly payment** using the `PMT()` function:
   ```
   =PMT(A4, A5, -A1)
   ```

The result in A6 will give you the monthly loan payment.

### Example Calculation:
For a loan amount of ₹5,00,000 at an annual interest rate of 6% for 20 years:

- Monthly Interest Rate = 6% / 12 = 0.5%
- Number of Payments = 20 * 12 = 240 months

The formula in A6 will return a monthly payment of approximately **₹3,597.99**.

This formula can be used for any loan amount, interest rate, or term by changing the values in the relevant cells.