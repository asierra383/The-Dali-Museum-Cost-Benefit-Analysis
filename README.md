# The Dali Museum Cost Benefit Analysis

## Introduction
The purpose of this deliverable is to conduct a cost-benefit analysis on the DAM (Digital Asset Management) & Digital Preservation Systems that was researched on for my Summer 2025 internship project at The Dalí Museum. This analysis allows for the museum to understand which system vendors are most cost-effective for implementation. The calculations & visualizations are already provided in the Google Colab file, but I have included the calculation results in here in case a viewer of this repository would prefer to have the top-level information from this research.

This deliverable used 8 staff members as the sample size to calculate the Cost-Benefit Analysis of SaaS vendors for digital asset management & digital preservation systems. In total, there are 51 users of digital assets, according to a statement given by the Systems Administrator of the IT/AV department.

In order to get the Cost-Benefit Analysis, I imported Python libraries like Numpy, Pandas, & Matplotlib. They are relevant for providing the charts & graphs that are shown in the Google Colab file. Since I need to perform math & data visualizations, the following libraries were used.

## Background & Context
In order to better understand how the calculations are done, there is information that must be given.

The fixed numbers given is to set a benchmark for simplified calculations:
- Staff has a varying amount of vacation weeks, so I set the number of weeks working to 48 to create a scenario where all staff from the sample receive 4 weeks of vacation
- I set the hours of working per week to 40 since all staff in the sample size are considered full-time
- When comparing sunk hours & cost with system savings, I applied the Pareto Principle, also called the 80/20 Rule, to state that there would be an 80% in time & wage savings from a system implementation

There is 2 types of staff information that was collected differently in order to use them in the calculations with the fixed numbers
- The number of sunks hours was collected based on the total number of passing hours from 5 given scenarios that are provided on [Canto's DAM ROI calculator](https://www.canto.com/dam-roi/)
- Salaries were given based on the [Association of Art Museum Directors (AAMD) 2023 Salary Survey](https://thedali-my.sharepoint.com/my?id=%2Fpersonal%2Fasierra%5Fthedali%5Fonmicrosoft%5Fcom%2FDocuments%2FAttachments%2FAAMD%5FSalary%20Survey%202023%2Epdf&parent=%2Fpersonal%2Fasierra%5Fthedali%5Fonmicrosoft%5Fcom%2FDocuments%2FAttachments&ga=1) report, specifically, the mean salary of the Southeast region was used

In order to get the given prices of the system vendors, there were steps taken & vendors also needed certain information to give a quote
- An initial meeting was usually conducted first in order to follow up with a product demonstration, & then pricing was discussed
- Vendors usually asked for storage needs (hot & cold), storage type, numbers of users (concurrent and/or admin users), & needed vendor native integrations
  - Vendor integrations through their APIs were not included in the cost-benefit analysis due to project constraints since I could not receive all of those figures & have them added before the end of the project timeline
  - Terentia &  Filecamp are exceptions because Terentia did include integrations into the quote, while Filecamp has no public API to allow integrations at this point

Finally, please keep in mind that Initial Setup Cost & Total Start Cost mean the same thing if you are also referencing the System Evaluation Matrix & Feature Comparison Chart spreadsheets.

## Staff Information Calculations
Calculations must be made to find the hourly wage of staff members to understand how much the museum spends of staff wages on the current state of digital asset workflows. This would lead to understanding what is the annual sunk cost & annual sunk time.

Calculation Results:
- Average Annual Sunk Hours Yearly = 645
- Average Annual Sunk Cost Yearly = $22936.87
- Total Annual Sunk Hours Yearly = 5160
- Total Annual Sunk Cost Yearly = $183495
- Left-skewed distribution​; most data points fall on the right side

## System Vendor Calculations
By applying the 80/20 Rule, a benchmark can be established for the hours and costs that can be saved on a yearly basis by implementing this type of system. With having the prices given by the system vendors, we can have an understanding for what the industry standard looks like, and therefore we can proceed to a cost benefit analysis.

Calculation Results:
- Total Annual Hours Saved Yearly = 4128
- Total Annual Savings Yearly = $146796
- Average System Annual Cost = $23612.64
- Average System Initial Setup Cost = $29171.38
- Right-skewed distribution​; most data points fall on the left side​
  - Outlier present in upper quartile

## Final Calculations
Now we can proceed with doing the calculations for the cost benefit analysis:
- Net Present Value = ∑ Present Value of Expected Benefits - ∑ Present Value of Future Costs
- Cost Benefit Ratio = ∑ Present Value of Expected Benefits / ∑ Present Value of Future Costs

Calculation Results:
- Net Present Value (NPV)
  - Minimum/Maximum Range: [$95882, $133164]
  - Average Net Present Value = $123183.35
  - Left-skewed distribution; most data points fall on the right side
    - Outlier present in lower quartile
- Cost Benefit Value (CBV)
  - Minimum/Maximum Range: [2.88, 10.77]
  - Average Cost Benefit Ratio = 6.68
  - Right-skewed distribution; most data points fall on the left side
    - Outlier present in upper quartile

## Top 5 Cost-Effective Systems for Initial Setup Cost:
1. Pics.io
2. Piction
3. Soutron Global
4. Archivematica
5. ResourceSpace

# Thank you for reading!
