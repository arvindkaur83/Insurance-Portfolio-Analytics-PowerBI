# Insurance Portfolio Analytics Dashboard

An interactive Power BI dashboard designed to analyze insurance portfolio performance across premiums, maturity values, protection amounts, policy tenure, sales hierarchy, geography, occupations, and product categories.

The project demonstrates how policy-level insurance data can be transformed into actionable business insights using Power Query, DAX, data modeling, and interactive Power BI visualizations.

> This project was independently implemented for educational and portfolio purposes. The dashboard concept was inspired by publicly available learning material, while the analytical interpretation, documentation, and project presentation were prepared independently.

---

## Table of Contents

- [Project Overview](#project-overview)
- [Business Objective](#business-objective)
- [Key Portfolio Metrics](#key-portfolio-metrics)
- [Dashboard Pages](#dashboard-pages)
- [Tools and Technologies](#tools-and-technologies)
- [Data Preparation](#data-preparation)
- [Data Modeling](#data-modeling)
- [DAX Measures](#dax-measures)
- [Interactive Features](#interactive-features)
- [Key Business Insights](#key-business-insights)
- [Screenshots](#screenshots)
- [Repository Structure](#repository-structure)
- [How to Use the Project](#how-to-use-the-project)
- [Future Enhancements](#future-enhancements)
- [Disclaimer](#disclaimer)

---

## Project Overview

Insurance companies manage policies with different durations, premium structures, protection values, maturity benefits, payment frequencies, and sales channels.

Analyzing this information in raw tables can make it difficult to understand portfolio performance and identify important business trends.

This Power BI project converts insurance policy data into an interactive analytical dashboard that helps users evaluate:

- Policy volume
- Premium collection
- Premium payable exposure
- Maturity value
- Protection value
- Annualized ROI
- Policy-type contribution
- State-wise performance
- Occupation-based segmentation
- Sales-agent performance
- Regional and organizational performance

The dashboard contains multiple report pages with interactive filters, KPI cards, charts, drillable hierarchies, and dynamic financial measures.

---

## Business Objective

The objective of this project is to create a centralized reporting solution for monitoring and analyzing insurance portfolio performance.

The dashboard helps business users answer questions such as:

- How many policies are present in the portfolio?
- What is the total premium value?
- How much premium has already been collected?
- How much premium remains payable?
- Which policy types contribute the most premium?
- How does investment value compare with maturity value?
- How does annual premium compare with protection value?
- Which states and occupations generate the highest premium contribution?
- Which sales agents perform most strongly?
- How does performance vary across the sales hierarchy?
- How do premium values change across different policy durations?

---

## Key Portfolio Metrics

| Metric | Value |
|---|---:|
| Number of Policies | 7,299 |
| Total Premium Amount | 39,096.58M |
| Total Annual Premium | 2,161.60M |
| Total Premium Paid | 10,686.35M |
| Total Premium Payable | 28,410.24M |
| Underwriting Expense | 38.66M |

These metrics provide an executive-level summary of the insurance portfolio before users move into detailed analysis.

---

## Dashboard Pages

### 1. Insurance Overview

The Insurance Overview page provides a high-level summary of the insurance portfolio.

It includes:

- Number of policies
- Total premium amount
- Total annual premium
- Total premium paid
- Total premium payable
- Underwriting expense
- Premium paid by policy type
- Premium paid by policy name
- Premium paid by sales agent
- Premium paid by state
- Premium paid by occupation
- Premium paid by year

### Why this page was designed this way

KPI cards are used to communicate the most important portfolio metrics immediately.

Charts are used to explain how the portfolio is distributed across products, locations, occupations, agents, and time periods.

Interactive slicers allow users to filter the entire page by:

- Policy type
- Policy name
- Sales agent
- Year
- State
- Occupation

This design allows users to move from a complete portfolio overview to a focused business segment without changing the underlying report.

---

### 2. Investment Value vs. Maturity Value

This page compares investment or premium value with maturity value across policy years.

The visual includes:

- Total investment or premium value
- Total maturity value
- Average annualized ROI
- Policy or maturity year

A combination chart is used, where:

- Columns represent financial values.
- The line represents annualized ROI.

### Why a combination chart was used

Investment value and maturity value are monetary measures, while ROI is a percentage.

Using the same axis for all three values would make the ROI trend difficult to interpret because the scales are different.

A combination chart with a secondary axis makes it possible to view:

- Absolute financial values through columns.
- Return behavior through the ROI line.
- Year-by-year changes in one visual.

The displayed analysis shows that maturity values generally exceed the corresponding investment values, while the annualized ROI changes across policy years.

---

### 3. Annual Premium vs. Protection Value

This page compares annual premium with the protection or sum-assured value across policy years.

The visual includes:

- Total annual premium
- Total protection value
- Average annualized ROI
- Policy year
- Tenure or duration selection

### Why this analysis is important

Premium value alone does not represent the complete customer benefit of an insurance policy.

Comparing annual premium with protection value helps evaluate the relationship between:

- Customer contribution
- Insurance coverage
- Policy duration
- Potential return

This analysis helps users understand whether higher annual premiums are associated with higher protection values.

### Why a tenure slicer was used

Insurance outcomes can vary significantly according to policy duration.

A tenure slicer allows users to compare different policy periods and analyze questions such as:

- Which tenure provides the highest protection value?
- How does annual premium change across durations?
- Does ROI vary by policy tenure?
- How does the premium-to-protection relationship change over time?

---

### 4. Premium Analysis

The Premium Analysis page examines premium behavior across different payment durations, including the five-to-twenty-year horizon.

It includes:

- Total premium paid
- Total premium payable
- Premium paid percentage
- Premium payable percentage
- Maturity amount
- Annualized ROI
- Year-wise premium analysis
- Sales-agent comparison

### Why this analysis was used

The difference between premium paid and premium payable is important for monitoring collection progress and future financial exposure.

- **Premium paid** represents the amount already collected.
- **Premium payable** represents the amount still expected or outstanding.
- **Maturity amount** represents the future benefit associated with the policies.
- **Annualized ROI** provides a return-oriented view of the selected policies.

For the displayed five-year analysis, the dashboard reports:

- Total premium amount: 4,005.23M
- Total annual premium: 370.87M
- Total premium paid: 2,556.17M
- Total premium payable: 1,449.06M
- Premium paid percentage: 63.82%
- Premium payable percentage: 36.18%

### Why sales-agent analysis was included

The sales-agent visual connects financial performance with commercial ownership.

It helps identify:

- Agents contributing the highest premium values.
- Agents associated with larger payable amounts.
- Potential areas for sales coaching.
- Opportunities for target setting and incentive planning.

---

### 5. Sales Hierarchy

The Sales Hierarchy page analyzes performance through multiple organizational and product levels.

The hierarchy includes:

- Zonal Manager
- Regional Manager
- Sales Agent
- Policy Type
- Policy Name

The page analyzes:

- Total annual premium
- Total premium amount
- Total premium paid
- Profit or gain

### Why a hierarchical matrix was used

Sales organizations naturally operate across multiple levels of responsibility.

A hierarchical matrix allows users to move from a summarized organizational view to detailed policy-level performance.

Users can analyze:

1. Zonal Manager performance.
2. Regional Manager contribution.
3. Sales Agent performance.
4. Policy Type contribution.
5. Policy Name performance.

This structure avoids creating separate pages for every level of the sales organization.

### Business value

The Sales Hierarchy page supports:

- Regional performance reviews
- Agent productivity analysis
- Product-mix evaluation
- Profitability analysis
- Sales accountability
- Identification of high-performing segments

The inclusion of profit or gain is important because premium volume alone does not necessarily represent profitability.

---

## Tools and Technologies

- Microsoft Power BI
- Power Query
- DAX
- Data modeling
- Interactive dashboard design
- KPI development
- Financial analysis
- Hierarchical reporting
- Business intelligence
- Data visualization

---

## Data Preparation

Power Query was used to prepare the source data before creating visualizations and calculations.

The data preparation process included:

- Removing duplicate records.
- Standardizing column names.
- Correcting data types.
- Converting date fields into valid date formats.
- Handling blank and null values.
- Cleaning inconsistent category labels.
- Converting financial fields into numeric formats.
- Preparing policy tenure categories.
- Validating premium-related columns.
- Preparing sales hierarchy fields for drill-down analysis.

### Why Power Query was used

Power Query provides a repeatable and auditable data preparation process.

The transformation steps are saved within the Power BI file and can be executed again when the data is refreshed.

Separating data preparation from DAX calculations improves:

- Maintainability
- Data quality
- Report performance
- Calculation clarity
- Refresh reliability

---

## Data Modeling

A structured data model is important because the dashboard contains multiple filters, calculations, and cross-visual interactions.

The model supports analysis across:

- Policies
- Products
- Customers
- Dates
- Geography
- Occupations
- Sales agents
- Regional managers
- Zonal managers

A star-schema approach is recommended for a production implementation.

The central policy fact table stores policy-level financial information, while dimension tables describe:

- Dates
- Customers
- Products
- Geography
- Occupations
- Sales organization

This approach reduces redundancy and improves the reliability of filtering and aggregation.

---

## DAX Measures

The dashboard uses DAX measures instead of hard-coded values wherever dynamic calculations are required.

Measures respond automatically to slicers and filters applied by the report user.

### Number of Policies

```DAX
Number of Policies =
DISTINCTCOUNT(Insurance[Policy ID])
```

### Total Premium Amount

```DAX
Total Premium Amount =
SUM(Insurance[Total Premium Amount])
```

### Total Annual Premium

```DAX
Total Annual Premium =
SUM(Insurance[Total Annual Premium])
```

### Total Premium Paid

```DAX
Total Premium Paid =
SUM(Insurance[Total Premium Paid])
```

### Total Premium Payable

```DAX
Total Premium Payable =
SUM(Insurance[Total Premium Payable])
```

### Total Underwriting Expense

```DAX
Total Underwriting Expense =
SUM(Insurance[Underwriting Expense])
```

### Total Maturity Amount

```DAX
Total Maturity Amount =
SUM(Insurance[Maturity Amount])
```

### Total Protection Value

```DAX
Total Protection Value =
SUM(Insurance[Sum Assured])
```

### Premium Paid Percentage

```DAX
Premium Paid Percentage =
DIVIDE(
    [Total Premium Paid],
    [Total Premium Paid] + [Total Premium Payable],
    0
)
```

### Premium Payable Percentage

```DAX
Premium Payable Percentage =
DIVIDE(
    [Total Premium Payable],
    [Total Premium Paid] + [Total Premium Payable],
    0
)
```

### Profit or Gain

```DAX
Profit or Gain =
SUM(Insurance[Profit/Gain])
```

### Maturity Uplift

```DAX
Maturity Uplift =
[Total Maturity Amount] - [Total Premium Amount]
```

### Maturity-to-Premium Ratio

```DAX
Maturity-to-Premium Ratio =
DIVIDE(
    [Total Maturity Amount],
    [Total Premium Amount],
    0
)
```

### Average Annualized ROI

```DAX
Average Annualized ROI =
AVERAGEX(
    Insurance,
    Insurance[Annualized ROI]
)
```

> Column names may need to be adjusted if the names in the Power BI model are different.

---

## Why Measures Were Used

DAX measures were used for portfolio-level calculations because they:

- Recalculate dynamically according to filters.
- Work consistently across multiple report pages.
- Support analysis by year, state, agent, occupation, and policy type.
- Avoid storing unnecessary repeated calculations.
- Improve the reusability of business logic.

Calculated columns are more suitable for row-level classifications such as:

- Tenure category
- Payment bucket
- Policy duration group
- Customer segment
- Policy status
- Year label

---

## Interactive Features

### Slicers

The report includes slicers for:

- Policy type
- Policy name
- Sales agent
- Year
- State
- Occupation
- Tenure
- Payment duration

Slicers allow users to investigate specific segments of the portfolio.

### Cross-Filtering

Selecting a value in one visual filters related visuals.

For example, selecting a state can update:

- Policy-type contribution
- Agent performance
- Occupation distribution
- Premium trends

This creates a connected analytical experience across the report.

### Field Parameters

Field parameters allow users to switch between different measures within the same visual.

Possible measures include:

- Total premium paid
- Total annual premium
- Total premium payable
- Maturity amount
- Protection value
- Profit or gain

### Drillable Hierarchies

The Sales Hierarchy page allows users to move between:

- Zonal Manager
- Regional Manager
- Sales Agent
- Policy Type
- Policy Name

This supports both executive-level summaries and detailed operational analysis.

### Matrix and Chart Views

The Sales Hierarchy page provides different ways to view the data.

- Matrix view is useful for detailed values and hierarchy analysis.
- Chart view is useful for ranking and visual comparison.

---

## Key Business Insights

### Portfolio Size

The portfolio contains 7,299 policies, providing a broad basis for analyzing insurance products, customers, regions, occupations, and sales channels.

### Premium Collection

The Premium Analysis page distinguishes between premium paid and premium payable.

This helps stakeholders monitor:

- Collection progress
- Future payment exposure
- Outstanding premium levels
- Potential cash-flow requirements

### Policy-Type Contribution

Premium-paid contribution is distributed across Endowment, Universal, and Whole policy categories.

This helps identify whether the portfolio is balanced across multiple products or concentrated in selected policy types.

### Geographic Contribution

The state-level analysis highlights the locations contributing the highest premium values.

This can support:

- Regional sales planning
- Market prioritization
- Campaign targeting
- Sales-resource allocation

### Occupation-Based Contribution

The occupation analysis provides an additional customer-segmentation perspective.

Occupation-based analysis can support:

- Targeted marketing
- Product positioning
- Customer profiling
- Portfolio segmentation
- Underwriting analysis

### Maturity and Investment Comparison

The Investment Value vs. Maturity Value page allows users to assess whether maturity values exceed the corresponding investment amounts.

The ROI trend adds a return-oriented perspective to the financial comparison.

### Sales Performance

The Sales Hierarchy page connects financial results with organizational ownership.

It helps managers compare performance across zones, regions, agents, policy types, and policy names.

---

## Data Quality Considerations

Before using the dashboard for production decision-making, the following validation checks should be completed:

- Confirm that policy IDs are unique.
- Verify the correct grain of the policy data.
- Check whether premium paid and premium payable reconcile to the expected premium amount.
- Validate maturity values.
- Confirm the definition and calculation of annualized ROI.
- Check whether recent-year data is complete.
- Confirm the currency and unit scaling.
- Validate sales hierarchy assignments.
- Review blank and unknown category values.
- Confirm the meaning of all date fields.

These checks are important because incorrect data definitions can lead to misleading business conclusions.

---

## Screenshots

### Insurance Overview

![Insurance Overview](screenshots/insurance-overview.png)

### Investment Value vs. Maturity Value

![Investment Value vs Maturity Value](screenshots/investment-vs-maturity.png)

### Annual Premium vs. Protection Value

![Annual Premium vs Protection Value](screenshots/annual-premium-vs-protection.png)

### Premium Analysis

![Premium Analysis](screenshots/premium-analysis.png)

### Sales Hierarchy

![Sales Hierarchy](screenshots/sales-hierarchy.png)

---

## Repository Structure

```text
Insurance-Portfolio-Analytics-PowerBI/
│
├── README.md
├── Insurance_Portfolio_Analytics.pbix
│
├── screenshots/
│   ├── insurance-overview.png
│   ├── investment-vs-maturity.png
│   ├── annual-premium-vs-protection.png
│   ├── premium-analysis.png
│   └── sales-hierarchy.png
│
└── documentation/
    ├── dax-measures.md
    ├── data-dictionary.md
    └── business-insights.md
```

---

## How to Use the Project

1. Download the `Insurance_Portfolio_Analytics.pbix` file.
2. Install Microsoft Power BI Desktop.
3. Open the `.pbix` file in Power BI Desktop.
4. Navigate through the report pages.
5. Use the slicers to filter the data.
6. Select data points in charts to cross-filter other visuals.
7. Expand the Sales Hierarchy matrix to view detailed performance.
8. Change the selected tenure or duration to compare different policy segments.

---

## Future Enhancements

Possible future improvements include:

- Policy renewal analysis
- Policy lapse analysis
- Customer retention analysis
- Claim frequency analysis
- Claim severity analysis
- Loss ratio analysis
- Cohort analysis by policy issue year
- Forecasting of future premium collections
- Regional target-versus-actual analysis
- Row-level security for different business users
- Drill-through pages for agents and policies
- Automated refresh through Power BI Service

---

## Skills Demonstrated

This project demonstrates practical experience with:

- Power BI dashboard development
- Power Query transformations
- DAX calculations
- Data modeling
- Financial KPI design
- Time-based analysis
- Sales hierarchy reporting
- Interactive filtering
- Business-focused data storytelling
- Data quality validation
- Portfolio performance analysis

---

## Disclaimer

This project is intended for educational and portfolio purposes.

The dashboard concept was inspired by publicly available learning material. The implementation, calculations, documentation, business interpretation, and repository presentation were independently prepared.

No confidential, private, or personally identifiable information is included in this project.
