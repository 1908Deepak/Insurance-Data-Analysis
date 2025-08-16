# INSURANCE DATA ANALYSIS

### Dashboard Link :https://app.powerbi.com/groups/9dfd857a-796e-4f06-82d4-c4d57ddb57f0/reports/266d70fb-f7e4-45ac-84ef-e7b3ad6fe072/b1562978409a404112cb?experience=power-bi

## Problem Statement
Insurance companies handle huge volumes of data on policies, claims, customers, and premiums. To make informed business decisions, it is critical to track KPIs like premium amount, coverage, claim trends, and customer demographics. This dashboard helps the insurer evaluate performance across claims, gender distribution, and policy status

## Key Objective

To provide insurers with a unified view of policy performance, claim behavior, and customer demographics, enabling risk assessment, fraud detection, and better decision-making.


### Steps followed 

Step 1 – Data Loading

- Loaded card dataset from Excel workbook in into Power BI.

Step 2: Open Power Query Editor and in the View tab under Data Preview, enabled:

- Enabled:

  - Column distribution

  - Column quality

  - Column profile

- Set profiling to "Based on entire dataset".

Also, changed profiling to “Based on entire dataset”.

Step 3 – Data Quality Checks

- No major errors in key fields.
- Some nulls in claim amounts handled by replacing with 0.


Step 5 : Created KPIs in Report View:
Created card visuals with DAX measures:

      Premium Amount = SUM(Insurance[PremiumAmount])

      Coverage Amount = SUM(Insurance[CoverageAmount])

      Claim Amount = SUM(Insurance[ClaimAmount])

      Female Count = CALCULATE(COUNT(Insurance[CustomerID]), Insurance[Gender] = "Female")

      Male Count =  CALCULATE(COUNT(Insurance[CustomerID]), Insurance[Gender] = "Male")


![KPIs](https://github.com/user-attachments/assets/fffd9c52-ffea-4af4-9c74-1178b28e8b41)
![KPIs](https://github.com/user-attachments/assets/210ebe10-319d-46c5-b2c9-bd51ef822361)


Step 5 : Created Visuals:
- Line Chart → Claim Amount trend over time
- Table → Details of Policy Number, Customer ID, Claim Number, Age, Gender, Coverage Amount, Premium Amount, Policy Status, Claim Date.
- Line Chart → Claim Amount trend over time

Step 6 – Slicers Added
- Policy Number
- ClaimAmount
- CustomerID

Step 7 : Inserted branding (company logo, name, tagline).

Step 8 - Publish to Power BI Service 
- Published dashboard for cloud access and sharing with stakeholders.

![Publish_Message](https://github.com/user-attachments/assets/6233aea8-6549-43e7-9bb6-cd4d742a7357)

# Dashboard :   Home Page 

![dashboard_snapo](https://github.com/user-attachments/assets/4770dd98-7aa1-435d-82f4-a634b332792f)

# Dashboard :   Insurance Page

![dashboard_snapo](https://github.com/user-attachments/assets/b1e1eba6-cfeb-403b-8660-0aa13ed18094)

# Dashboard :   Customer Details 

![dashboard_snapo](https://github.com/user-attachments/assets/e1f9b5e1-dd1b-4c53-8b72-037fe53cb653)

 
# Insights

- Majority of policies are active, but inactive claims highlight lapses in follow-ups.

- Claim amounts show seasonal fluctuations, peaking in certain months.

- Gender distribution indicates higher participation from male policyholders.

- Premium vs Coverage analysis shows gaps in risk vs return alignment.



# Conclusion

The Insurance Data Analysis Dashboard provides valuable insights into policy and claim management. By monitoring KPIs and trends, insurers can:

- Track claim frequency and severity
- Improve policy design based on demographic insights
- Enhance customer satisfaction through better coverage strategies
## Resources

[Insurance Dataset](https://drive.google.com/drive/folders/1D9AIpJ6dDawQHDejalNjONBCCptAEYLk?usp=sharing)


## Authors

- [1908Deepak](https://github.com/1908Deepak)


## Feedback

If you have any feedback, please reach out to us at deepaksingh190810@gmail.com

