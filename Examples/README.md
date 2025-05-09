# GST

```vb
Function gst(amount As Double, percentage As Double) As Double
    gst = (amount * (percentage / 100))
End Function
```

---

### 💡 Example:

If you call `=gst(1000, 18)` in an Excel cell, it will return:

```
1000 * (18 / 100) = 180
```

Would you like a version that returns the **total amount including GST** instead of just the GST value?
