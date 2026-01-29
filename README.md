# MIS-311
## Introduction to Business Analytics
*Data Analysis and Insight*
### **Data Overview**
- Description: The Cost of Living dataset provides information on living expenses and income levels across different countries and regions over time. It includes key indicators such as average monthly income, cost of living index, year of observation, and geographic region.
- Source of data:Provided by MIS 311 course materials (EIU Moodle). The dataset appears to be compiled from publicly available sources such as cost-of-living databases (e.g., Numbeo) and international statistical sources for income data (e.g., IMF/OECD/World Bank), but the original source is not specified in the dataset file.
- Number of rows: **201 rows**  
- Number of columns: **5 columns**
- The variables include both numerical data (average monthly income and cost of living index) and categorical data (country and region), making the dataset suitable for descriptive and exploratory data analysis.
- The context: Cost of living data basically tells us how much it really costs to live in a certain place. It's not just about rent; it's about groceries, transportation, and all the stuff that makes up daily life. This info is super important for everyone from governments trying to keep the economy healthy to companies deciding where to set up shop, and even for us regular folks figuring out where we can afford to live comfortably. It's all about understanding how far your money goes, and what kind of life you can build in a particular city or town.  

### **Data Cleaning**
* Missing values: **4 values**
  - _Average monthly income column_: 2 missing values ( C162, C178)  
  - _Region column_: 2 missing values ( E26, E39)  
**Handling missing values:**
- The 2 missing values in the average monthly income column were removed because they represent a very small proportion of the dataset (less than 2%) and could bias affordability calculations if imputed.
- The 2 missing values in the region column were removed due to insufficient information for accurate classification.
- Overall, the 4 missing values account for approximately **1.99% of the total 201 observations**, which is unlikely to significantly affect the analysis.
* Duplicate row: **2 duplicate rows** were found and removed
=> Handling duplicate rows: delete the 2 duplicate rows because they do not carry additional information and do not affect the analysis. The two duplicate rows account for about 0.99% of the total 201 rows. Duplicate rows cause statistical bias, degrade machine learning model performance due to redundant data learning, and disrupt record uniqueness while consuming storage space. Therefore, removing them is necessary to ensure accurate and efficient analysis.  
=> After  handling missing values and duplicate records, there are 195 rows and 5 columns left.  
 
### **Descriptive Statistics**
<img width="525" height="296" alt="image" src="https://github.com/user-attachments/assets/bbacf540-6949-4bdd-b62a-efbc0e127a84" />

## Average Monthly Income ##
The descriptive statistics show that the **mean monthly income** is **4264.53**, while the median is **4270.40**. Since the mean and median are very close, this suggests the income distribution is **relatively balanced** and not heavily skewed. However, the **standard deviation** is high **(2124.11)**, indicating that monthly income levels vary substantially across different countries and years. The income values range widely from **a minimum of 534.74** to a **maximum of 7976.56**, highlighting significant economic differences among the observations.
## Cost of living ##
The descriptive statistics show that the **mean cost of living** is **3703.59**, while the median is **3649.03**, indicating a **relatively balanced distribution** without strong skewness. However, the standard deviation is high **(1983.30)**, suggesting that living expenses vary considerably across different countries and regions. The cost of living ranges from a **minimum of 464.49** to a **maximum of 6981.02**, highlighting substantial differences in living standards and economic conditions worldwide.

## Key Insights
**Insight 1:**  
<img width="757" height="430" alt="image" src="https://github.com/user-attachments/assets/0629b2dc-b8ba-4004-bcb2-7b8f97622dd0" />

The chart shows clear regional differences in both **average cost of living** and **average disposable margin**, highlighting that affordability depends strongly on geographic location. For example, **Africa has the highest average cost of living (~3,960)**, while **Europe has the lowest (~3,555)**, and **North America has the smallest disposable margin (~90)** compared to **Europe (~950)**. This implies that relocation decisions and compensation planning should account for regional affordability rather than relying only on cost-of-living levels.
=> Companies may need location-based salary adjustments or allowances to maintain employee purchasing power across regions.

**Insight 2:**  
<img width="1048" height="501" alt="image" src="https://github.com/user-attachments/assets/14751ad5-7657-46f2-afd8-97e5a9d89c63" />

Some countries show **very low or negative disposable margins**, meaning living costs can consume most of the average monthly income and create affordability pressure. For example, the **Canada and  the United States has a negative disposable margins (-607.1 and −102.83)**, while **Germany (1211.16)** and **France (1022.58)** have much higher margins, indicating stronger affordability. This suggests that living standards should be assessed using income-minus-cost measures rather than cost-of-living values alone when making location and budgeting decisions.

## Tools Used
- Microsoft Excel
