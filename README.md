# Elevate_Health_Analysis
Founded in 2016, Elevate Health is a medical insurance company that serves thousands of customers throughout the United States. In 2019, they launched a new set of marketing campaign categories spanning topics such as wellness tips, plan affordability, and preventative care. Elevate Health customers can sign up for 4 different plans: bronze, silver, gold, and platiunum, each with different premiums and claim coverage rates.

Elevate Health has hired a new data team to assist them in strategizing their marketing budget for the year. The company aims to build a more robust understanding of these campaign categories and how they relate to signups and subsqeutent patient claims.

As a data analyst contracting with Elevate Health, this analysis will be hinged on providing a dynamic visual deliverable to enable the marketing team to self-serve insights and regular-cadence reporting. In this particular report, the data team was tasked with investigating a relationship between existing cutomer behavior, and marketing campaigns, i.e. the relationship between customer claims and marketing. 

There are three main tables referenced, with the Entity Relationship Diagram (ERD) below:

![image](https://github.com/stephaniegoodman/Elevate_Health_Analysis/assets/65201326/462cfbbc-8856-4822-91d2-7901ebfef569)

## Process-Driven Documentation and Deliverables
- Completed Tableau dashboard can be accessed [here].<https://public.tableau.com/views/ElevateHealthClaimsInvestigation/ClaimsInvestigationDashboard?:language=en-US&:sid=&:display_count=n&:origin=viz_share_link>)
- High-level and data driven insights can be found below
- In this project, a stakeholder powerpoint was created, and a presentation was arranged for the claims management and marketing teams (full presentation available upon request)
<img width="786" alt="Screen Shot 2024-04-01 at 2 56 54 PM" src="https://github.com/stephaniegoodman/Elevate_Health_Analysis/assets/65201326/50a3fb20-a084-4317-9a71-5e305f8ec2c2">

## North Star Metrics
- Claims: claim count, claim amount, claim type (includes aggregations such as average claim amount, and most common claim type)
- Campaign type: marketing campaign and type
- Customer profile: signup date, state, plan type

## High Level Insights
- Claim counts peaked in May 2022 with 1.4k claims. There was a steep drop off in July 2023 with 725 claims, a 49% decrease.
- Claim amounts peaked in May 2022 at $425k, July 2023 drop off was $199k, a 53% decrease.
- Compare Health Coverage had the highest claim amount ($3.9M, 30%), and Health for All had the highest claim count (12K, 24%).
- Silver plan and New Jersey customers comprise the majority of claims, 87% and 52% respectively.
<img width="979" alt="Screen Shot 2024-04-01 at 2 58 07 PM" src="https://github.com/stephaniegoodman/Elevate_Health_Analysis/assets/65201326/a8c6879f-1e1e-4629-bc34-8de955270c3f">
<img width="974" alt="Screen Shot 2024-04-01 at 2 57 35 PM" src="https://github.com/stephaniegoodman/Elevate_Health_Analysis/assets/65201326/7cfc8d4f-0014-43e0-9f13-92b66332d69e">

## Key Insights and Takeaways
- After investigating the following metrics: average claim count, claim amount, claims by marketing campaigns, and claims by customer profiles (i.e. customers by state, plan, signup date), it was concluded that a statistical relationship between customer claims and marketing campaigns is highly unlikely, although further statistical analysis is required to confirm this.
- Platinum plans consistently underperform in claim count, amount, and number of customer signups. It is recommended to collaborate with the marketing team on a further analysis to determine recommendations for either improving platinum customer signups, or to dissolve the plan altogether to focus on more successful offerings.
- Claims steadily rose until a respective peak in 2022, and have been declining notably since then. Further analysis is recommended to determine potential reasons for this change, and collaboration with marketing is indicated to promote more customer engagement.
<img width="971" alt="Screen Shot 2024-04-01 at 2 56 06 PM" src="https://github.com/stephaniegoodman/Elevate_Health_Analysis/assets/65201326/2af7b10b-44ef-4d51-aead-daab32d2f52a">


## Technical Process and Caveats
- It is recommended to make the following adjustments to the available data to promote more robust and statistically significant analyses in the future:
     - Provide start and end dates for marketing campaigns
     - Include dimensions for plan types (ex: coverage rate) to develop a more robust customer profile across different 
        offerings
     - Consider splitting customers of the same demographic profiles into "control" and "test" groups for marketing campaigns to more clearly compare the effects of campaigns
- Brief overview of the technical process:
      - **Dataset stats**:
            - **33 unique campaigns** were analyzed across 12 different campaign types
            - **16,338 customers** were attributed to campaigns
            - Data ranges from **2019 to 2023**
       - **Data points involved**:
            - **Campaigns**: campaign category, campaign type (33 total records)
            - **Customers**: customer identification (ID), plan, signup date, and state (16,338 total records)
            - **Claims**: claim amount, claims (49,998 total records)
       - **The technical process included**:
            - Loading data into **Tableau** from **Excel**
            - Building a **self-service dashboard** for visualization in Tableau
            - **Use filters to alternate views** based on plan, state, and campaign type
            - **Minimal data cleaning was needed** for this dataset, but could involve: checking for nulls and   
                nonsensical values, aligning date types, and augmenting missing data


