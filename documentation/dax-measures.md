# DAX Measures

This document contains the main DAX measures used in the Insurance Portfolio Analytics Dashboard.

> The table and column names may need to be adjusted according to the final Power BI data model.

## Number of Policies

```DAX
Number of Policies =
DISTINCTCOUNT(Insurance[Policy ID])
```

Counts unique insurance policies instead of counting rows. This prevents duplicate records from inflating the policy count.

## Total Premium Amount

```DAX
Total Premium Amount =
SUM(Insurance[Total Premium Amount])
```

Calculates the total premium amount within the current filter context.

## Total Annual Premium

```DAX
Total Annual Premium =
SUM(Insurance[Total Annual Premium])
```

Calculates the total annual premium associated with the selected policies.

## Total Premium Paid

```DAX
Total Premium Paid =
SUM(Insurance[Total Premium Paid])
```

Calculates the premium already paid by policyholders.

## Total Premium Payable

```DAX
Total Premium Payable =
SUM(Insurance[Total Premium Payable])
```

Calculates the premium amount expected or payable according to the selected policy records.

## Premium Paid Percentage

```DAX
Premium Paid Percentage =
DIVIDE(
    [Total Premium Paid],
    [Total Premium Paid] + [Total Premium Payable],
    0
)
```

Measures the proportion of total paid and payable premium that has already been collected.

## Premium Payable Percentage

```DAX
Premium Payable Percentage =
DIVIDE(
    [Total Premium Payable],
    [Total Premium Paid] + [Total Premium Payable],
    0
)
```

Measures the proportion of total paid and payable premium that remains payable.

## Total Maturity Amount

```DAX
Total Maturity Amount =
SUM(Insurance[Maturity Amount])
```

Calculates the total maturity amount for the selected policies.

## Total Protection Value

```DAX
Total Protection Value =
SUM(Insurance[Sum Assured])
```

Calculates the total protection or sum-assured value.

## Underwriting Expense

```DAX
Total Underwriting Expense =
SUM(Insurance[Underwriting Expense])
```

Calculates the underwriting expense associated with the selected policies.

## Profit or Gain

```DAX
Profit or Gain =
SUM(Insurance[Profit/Gain])
```

Calculates the total profit or gain for the selected policies.

## Maturity Uplift

```DAX
Maturity Uplift =
[Total Maturity Amount] - [Total Premium Amount]
```

Calculates the difference between maturity value and total premium amount.

## Maturity-to-Premium Ratio

```DAX
Maturity-to-Premium Ratio =
DIVIDE(
    [Total Maturity Amount],
    [Total Premium Amount],
    0
)
```

Compares the maturity value with the total premium amount.

## Average Annualized ROI

```DAX
Average Annualized ROI =
AVERAGEX(
    Insurance,
    Insurance[Annualized ROI]
)
```

Calculates the average annualized ROI across the selected policy records.
