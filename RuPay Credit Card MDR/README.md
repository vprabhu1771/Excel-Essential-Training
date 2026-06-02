If you're asking **what percentage 997.99 is of 42,500**:

$$
\frac{997.99}{42500} \times 100 \approx 2.35\%
$$

**Answer: 997.99 is approximately 2.35% of 42,500.**

If you meant something different (for example, *42,500 minus 997.99 and the percentage decrease*), the decrease is also about **2.35%**.


# Excel Formula

If:

* **A1** = Amount (e.g., 42500)
* **B1** = Percentage (e.g., 2.35)

To get the result amount from the percentage:

```excel
=A1*B1/100
```

Example:

```excel
=42500*2.35/100
```

Result: **998.75**

If your percentage is already stored as an Excel percentage value (e.g., 2.35%), use:

```excel
=A1*B1
```

If you want to calculate the percentage from two amounts (e.g., 997.99 out of 42500):

```excel
=997.99/42500*100
```

Result: **2.3482%** (≈ 2.35%).
