# Data Dictionary

This document describes the main fields used in the Insurance Portfolio Analytics Dashboard.

| Field | Description |
|---|---|
| Policy ID | Unique identifier assigned to an insurance policy |
| Customer ID | Identifier associated with the policyholder |
| Policy Holder Name | Name of the policyholder |
| Policy Type | Broad category of the insurance policy |
| Policy Name | Specific insurance product name |
| Sales Agent | Agent responsible for the policy |
| Regional Manager | Regional owner of the sales activity |
| Zonal Manager | Zonal owner of the sales activity |
| State | Geographic location associated with the policy |
| Occupation | Occupation category of the policyholder |
| Gender | Gender category recorded in the source data |
| Tenure | Duration of the policy |
| Premium Duration | Period over which premiums are paid |
| Payment Frequency | Frequency of premium payment |
| Premium Amount | Premium value associated with the policy |
| Annual Premium | Annualized premium value |
| Total Premium Amount | Total premium value associated with the policy |
| Total Premium Paid | Premium amount already collected |
| Total Premium Payable | Premium amount expected or remaining payable |
| Maturity Amount | Expected maturity value of the policy |
| Sum Assured | Protection value provided by the policy |
| Underwriting Expense | Expense associated with underwriting the policy |
| Profit/Gain | Profit or gain associated with the policy |
| Policy Date | Date associated with the insurance policy |
| Annualized ROI | Return indicator calculated for the policy |

## Data Validation Considerations

The following checks should be completed before using the report for production purposes:

- Confirm that Policy ID values are unique.
- Verify the correct grain of the source data.
- Check that financial fields use consistent units.
- Validate premium paid and premium payable values.
- Confirm the definition of maturity amount.
- Validate the annualized ROI calculation.
- Check for missing or inconsistent categories.
- Confirm sales hierarchy assignments.
- Verify the meaning of all date fields.
