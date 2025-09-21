# Exploratory-Analysis-on-Real-Estate
This analysis seeks to create insights into different property types, the associated cost, property assessment among others over the period 2001 to 2020
Background 
The Office of Policy and Management maintains a listing of all real estate sales with a sales price of $2,000 or greater that occur between October 1 and September 30 of each year. For each sale record, the file includes town, property address, date of sale, property type (residential, apartment, commercial, industrial, or vacant land), sales price, and property assessment.

## Problem Statement:  Exploring Property Assessment and Sales Data for Informed Decision-Making. 
In our quest for informed decision-making in real estate, we are presented with a comprehensive dataset encompassing various attributes related to property assessment and sales transactions. 
This dataset includes information such as the assessed value, sale amount, sales ratio, property type, and more, offering a rich source of insights into the real estate landscape.

## Objectives 
1. Assessment Accuracy Evaluate the accuracy of property assessments by comparing assessed 
values with actual sale amounts, and identify any discrepancies.

2. Market Trends Analyze sales ratios to uncover trends in property market values, 
understanding how sale amounts relate to the assessed values across different property types and 
residential classifications.

3. Geographical Analysis Investigate variations in assessed values, sales amounts, and market 
ratios across different towns, providing a localized understanding of real estate dynamics.

4. Property Type Impact Examine the impact of property type on assessment accuracy and 
market trends, exploring whether certain types (e.g., residential, commercial) exhibit distinct 
patterns.

5. Non-Use Code Insights Explore the significance of non-use codes in property assessment, 
investigating how these codes influence assessed values and sales transactions.

6. Assessor and OPM Remarks Analyze remarks provided by assessors and the Office of Policy 
and Management (OPM) to identify factors influencing assessment decisions and potential areas 
for improvement.

The data provided has 997213 rows × 14 columns

The data provides the following columns: Serial Number', 'List Year', 'Date Recorded', 'Town', 'Address', 'Assessed Value', 'Sale Amount', 'Sales Ratio', 'Property Type','Residential Type', 'Non Use Code', 'Assessor Remarks', 'OPM remarks', 'Location'
The information provided shows that serial number, List Year, Town,  Assessed value, Sale Amount and Sales Ratio do not have any missing values,
However the remaining data variables i.e.Date recorded, Address,Property Type, Residential Type, Non use code, Assessor Remarks, OPM remarks and Location all have missing values with OPM remarks recording the highest missing values of 987,279 and date recorded just 2 missing values.
The numerical columns in the data provided are the following 'Serial Number', 'List Year', 'Assessed Value', 'Sale Amount', 'Sales Ratio'

Missing values for Property Type, Residential Type, Assessor Remarks, OPM remarks, Address, DateRecorded, Location and Non Use Code were replaced using the mode method for the null values
The total number of records for each variable is 997,213. The mean Assessed value, Sales Amount and Sales Ratio is 279,143.7, 391,151.2 and 10.44 respectively. The maximum Assessed value and Sales Amount is 881,510,000 and 5,000,000,000 respectively. The earliest date of transaction is 2001 while the latest date is 2020

Overall, the histograms provide insights into the distributions of the three numerical columns, helping to understand the typical values and variability within each variable.¶
Assessed Value: The histogram for 'Assessed Value' shows that the majority of properties have assessed values between  $50,000 𝑎𝑛𝑑 $100,000, with a peak around $75,000. There is a relatively small number of properties with higher assessed values. Sale Amount:
The 'Sale Amount' histogram indicates that most properties were sold at prices ranging from 80,000 to 160,000. The distribution appears slightly skewed to the right, with a peak around $120,000. There are fewer properties with sale amounts at the lower end of the scale. 
Sales Ratio:The histogram for 'Sales Ratio' displays the distribution of the ratio between the sale amount and assessed value. A sales ratio of 1.0 indicates a sale at the assessed value. In this case, the distribution is centered around a sales ratio of 1.0, but there is some variability. It seems that a majority of properties have sales ratios close to 1.0, indicating sales close to their assessed values. There are a few properties with higher sales ratios, suggesting they were sold at a premium compared to their assessed values
The top 5 serial numbers 20200091, 160387, 160394, 160393 and 160389 have a total sales amount of 5,001,321,600; 408,974,700; 408,341,556; 408,058,727; and 406,441,967 respectively
Union is the town with the least number of properties i.e 261 whilst Bridgeport was seen to be the town with the highest number of properties i.e 34,201

The number of unique Property Types is 11 
 and they are as follows: 'Commercial' 'Residential' 'Vacant Land' nan 'Apartments' 'Industrial' 'Public Utility' 'Condo' 'Two Family' 'Three Family' 'Single Family' 'Four Family'
 The data shows that the single family property type was the most available property type followed by the condo and residential. The two, three and four family, property types recorded 26408, 12586 and 12586 market representation respectively. Public Utility was the least constructed property type
 The least purchases were made in 2001, followed by 2011, 2012,2008,2009 and 2013 in that order. Highest sales were recorded in the year 2005 followed by 2004 and 2020
 
## Insights into Distribution:
The radar chart provides insights into the distribution of Assessed Values among the top 10 towns. The radar chart visually identifies the top 10 towns with the highest cumulative Assessed Values.Towns with longer spokes have higher Assessed Values. These are the towns towards the outer edges of the radar chart.For example, the chart shows that GreenwichTown has an Assessed Value of $50,000 which is the least valued whist the town of Danbury has the higest Assessed Value of $160,000
 The chart displays different categories of Property Types, such as Residential, Commercial, Industrial etc. The percentages indicate the cumulative Non Use Code values for the respective Property Type. The data show that cumulatively commercial property types has the highest non use of 15.5% implying less patronage for this while the four family property type has the least non use  of 6.2% indicating more person were interested in this property type
 
 Assessed Value vs. Sales Ratio (Positive Correlation):  A positive correlation coefficient indicates a tendency for both variables to move in the same direction. As the Assessed Value increases, there is a positive correlation with the Sales Ratio. This suggests that properties with higher assessed values tend to have higher sales ratios, potentially indicating a positive relationship between the assessed value and the ratio of the sale amount to the assessed value. 
Assessed Value vs. Sale Amount (Positive Correlation):
Similar to the Assessed Value vs. Sales Ratio, there is a positive correlation between Assessed Value and Sale Amount. This implies that properties with higher assessed values are more likely to have higher sale amounts. Sales Ratio vs. Sale Amount (Negative Correlation):The negative correlation coefficient suggests an inverse relationship between the Sales Ratio and Sale Amount. As the Sales Ratio increases, the Sale Amount tends to decrease, and vice versa. This might indicate that properties with higher sale ratios have lower sale amounts. In general, correlation coefficients close to +1 or -1 indicate strong relationships, while values close to 0 suggest weaker or no linear relationship. However, correlation does not imply causation, and other factors may influence the observed relationships.
Assessed Value vs. Non Use Code (Positive Correlation):
The positive correlation coefficient suggests a tendency for both variables to move in the same direction. As the Assessed Value increases, there is a positive correlation with the Non Use Code. This could indicate that properties with higher assessed values are associated with higher non-use code values. Assessed Value vs. Sale Amount (Positive Correlation):
Similar to the Assessed Value vs. Non Use Code, there is a positive correlation between Assessed Value and Sale Amount. This implies that properties with higher assessed values tend to have higher sale amounts. Non Use Code vs. Sale Amount (Weak Positive Correlation):
The positive correlation coefficient between Non Use Code and Sale Amount suggests a weak positive relationship. This could indicate that as the non-use code increases, there might be a slight tendency for higher sale amounts, but the correlation is not strong.

## Recommendations

It can be seen that among the property types, more of the single family property type was constructed as seen from the propert count chart. Again, the public utility type was the least constructed and hence the least available on the market - this maybe as a result of high cost incurred for the construction. Interestingly from the non use code, the data shows that after the commercial property type, the single family property type is the next least patronized while the four family property type is most patronized as it has the least non use code. To increase revenue, price discrimination can be applied to the four family property type so this can be sold at a premium as there is high demand. On the other hand to encourage patronage of the commercial property type, discounts or promotions can be offered to make this property type more attractive.
The data shows that in 2005 the highest number of property purchases was recorded. From 2007 to 2017 the data records very low property purchase figures. This was the period where the effects of the global financial crisis was still being felt. This shows that in periods of financial instability the housing/property sector is negatively affected. As a precautionary measure - flexible payment structures can be put in place during times of financial instability to encourage patronage. Moratorium on repayment can also be introduced to give housing owners a financial breather

## Challenges Faced
It took a long while to figure out the insight required and what codes needed to be generated to derive the necessary insights.


