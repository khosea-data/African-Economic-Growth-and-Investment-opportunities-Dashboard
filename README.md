# Dashboard for Analyzing Economic Growth and Investment opportunities in African Countries 2024

## Repository Contents

1. [Project Overview](#project-overview).

2. [Data Sources](#data-sources).

3. [Data Collection](#data-collection)
   

4. [Data Analysis Tools that I used](#data-analysis-tools-that-i-used).

5. [Excel](#excel)

6. [SQL (postgresql)](#sql (postgresql)).
7. [TABLEAU](#tableau)

   

   


9. 

10. 

11. [Findings](#findings).

12. [Recommendations](#recommendations).

13. 

14. [Limitations](#limitations).

15. [References](#references).




### Project Overview
Due to current rise in global finance and increase in inflation rates all over the world,individual entrepreneurs, businesses and companies have opted to spread their risks by diversifying to various sectors in order to protect themselves from going bankrupt by depending on one source of income and for this reason I have laveraged data analysis to find markets and investment opportunities that companies and startups may get into to diversify their investment portfolios. In this project I have particularly chosen African nations where markets are still young and fast growing to investigate which sectors are suitable for investment and provide hope for future growth and also which countries are suitable for investing in various sectors. To get these insights I had to dive into knowing the 2023 GDP contribution of each sector of economy in different African countries because GDP contribution of a sector is a suitable indicator of whether there is growth which is signified by high contribution of the sector or whether there is stagnation signified by low contribution of the sector towards the overall GDP of the country, this will help investors and other entrepreneurs to get to know which sectors are suitable for investing. In order to understand which country is suitable, I used the GDP contribution of the past 3 years 2021,2022 and 2023 of each country in order to understand which countries are experiencing economic growth which is signified by a high GDP which might be a suitable place for investing in because a higher GDP of a nation indicates a growing economy which possibly provides a suitable environment for investors to look for opportunities and invest in the country while experiencing a positive growth in their businesses. I also grouped the countries into regions in order to know which regions are suitable for investment in Africa where the higher contribution of certain sector in a region indicates a suitable market and opportunities for investment growth. This project is important because it will help investors, entrepreneurs and startups who wish to get into African market which is growing so fast due to it's population increase to pinpoint those sutable sectors and countries where they can diversify into and grow their investment portfolio for their growth. It also helps for those who are planning for future investing to get more insights on how the market will be and how the current growth will influence the future growth of certain sectors. In order to accomplish this goal I came up with the following Business questions that will enable me get the insights and have the best suitable decisions about investing in Africa.


#### 1)Which country has the highest GDP in 2023?

Reason for asking this question; Understanding which country had the highest GDP contribution indicates large economic size which helps to identify potential markets for investment or expansion, it also indicates economic power and potential for regional investment.


#### 2)How does the GDP of the top 5 African economies have changed from 2021 to 2023?

Reason for asking this question; This helps in analysing growth trajectory of leading economies highlighting which countries are expanding faster or which may be facing economic stagnation.


#### 3)Which sector contributes the most to the GDP in each country?

Reason for this Question; Identifying the dominant sectors provides insights into the economic drivers of each country helping business focus on industry specific strategies for market entry.


#### 4)How does the contribution of agriculture sector to GDP vary across region?

Reason for this Question; Agriculture plays a crucial role in many African countries especially in rural areas, understanding its contribution helps target investments,aid and innovation in those areas.


#### 5)What is the total contribution of Renewable Energy to GDP in each region?

Reason for this Question; Renewable Energy is a fast-growing sector in Africa especially in countries aiming to diversify their energy mix. Understanding its contribution to GDP can highlight growth markets.


#### 6)Which regions has the highest cumulative GDP as of 2023?

Reason for asking this question;Identifying the region with the higher cumulative GDP as of 2023 helps businesses prioritize regions for market entry and expansion.

In order to get the insights and answers to these questions I laveraged data analysis tools EXCEL, SQL and TABLEAU which helped me get my final findings about investment opportunities in Africa.

# Data Sources

The primary dataset used for this analysis is the "Africa_Economies.csv" file containing detailed information about each country and sectors.



# Data Collection

In Data Sourcing and collection I did manual research by searching for and gathering data from different websites and public databases like WorldBank Data since complete dataset was not readily available. I manually researched and recorded each piece of data by ensuring accuracy and reliability of the information by cross-referrencing different sources. Inputing data into Excel, I entered each data point manually ensuring that the information was organized correctly. This involved creating columns for different variables for example country, region, agriculture, renewable energy and filling in each row with the appropriate data. I structured the data in tabular format where each row represented a specific entry and each column represented a variable or a parameter.

# Data Analysis Tools that I used.


## EXCEL
download [here](https://www.microsoft.com/en/microsoft-365/excel)


I chose Excel for this project because it is a versatile and accessible tool that offers powerful features for data Exploration, Cleaning and Visualization. With Pivot tables I was able to summarize and analyze the data quickly by creating visualizations that enabled me to present my findings in a clear and impactful way making it easy to communicate insights that can be understood by  both technical and non technical individuals.

I did the following using Excel in preparation of the data for Analysing

#### Handling Missing Values

I used conditional formating to highlight missing values and selected Blanks. I deleted some of the missing values after filtering them. I also filled some missing values with appropriate data based on the collection.

#### Data Cleaning

I did data cleaning by removing duplicates using the remove duplicates option in the data tab. I standardized the data by changing the text cases using UPPER for upper case LOWER for lower case and PROPER to make the first letter to be in upper case. I also did CONCATENATION to combine texts especially in countries and those that had splitted during entry, I also did splitting using text to columns in data tab and finally I did data types conversion by using the excel inbuilt power query.

#### Data Formating

I did data Formating to improve readability and usability of the data where I did number formating for currencies and putting them in $ dollar form together with custom to large numbers which was specifically Billions.

Finally I used Excel Pivot tables Pivot tables to do quick summary to allow flexibility in analysis, I also created reports using Pivot charts and included use of slicers for interactive data exploration where I can quickly narrow down results to a specific region and country, through this I was able to make it easier to analyse and draw insights from my data. I was able to create a dashboard where I joined all the pivot charts and applied the slicer to connect to all charts for easy analysis and reporting. 

Below are some of the Visualizations that I made using pivot charts to communicate insights.


## A bar chart of Regional agricultural GDP contribution where Western Africa is the leading in agriculture sectorwise with $572.7B

![image](https://github.com/user-attachments/assets/8e1ebc17-e923-4852-986c-f4546bf4b44f)
### A bar chart of 2023 GDP of each country where Algeria is at the top with the highest GDP among all the other countries by having $621B.

![image](https://github.com/user-attachments/assets/e418c67d-ff72-4fc6-9c1c-86579f5cdb73)

### A line graph of GDP growth of Top 5 countries from 2021 to 2023, Algeria and Cameroon have experienced high economic growth in between the years as shown by their rise in GDP while Nigeria, South Africa and Egypt have shown slow economic growth in between the years as shown by their slight increase in the GDP.

![image](https://github.com/user-attachments/assets/2754eb95-4543-4ecd-bd3a-511f32f0ef67)

### A pie chart of Renewable Energy sector contribution per REGION, The result show that Northen Africa is the leading among all the five regions with a total contribution of $44.2B.

![image](https://github.com/user-attachments/assets/a13d90f9-b012-4c86-bcca-ea0f3c830fda)


### A line graph of Sum of Regional 2023 GDP contribution where Northen Africa is seen to be the leading among the five regions with a total sum of $1382B.

![image](https://github.com/user-attachments/assets/2847965a-feb1-4e8b-bb7b-34fb2539c5de)

#### To check the intractive dashboard click on the link below,

##### [Excel interactive dashboard](C:\Users\hosea\Downloads\African Countries Economy investment opportunities analysis Dashboard.xlsx)


## sql (postgresql)

download [here](https://www.postgresql.org/download/)

I chose SQL as a tool for my project because it allowed me to write custom queries to efficiently extract, manipulate and aggregate data from the table, sql provided scalability and flexibility I needed to derive meaningful insights.


I used SQL to do Exploratory data analysis in order to get insights of the Business questions about investing in Africa.

Before analysis, I first saved my data in Excel in csv comma delimited format, then I imported the data to postgresql pgadmin with correct columns and appropriate data types to prevent any difficulties of importing the data and to ensure data accuracy. 
Then I explored the dataset to understand them by viewing the table structure.

Finally, I performed the following queries that I have detailed below to get the insights and solve the problem.


1.
```sql

SELECT Country, GDP_2023
FROM africa_economies
ORDER BY GDP_2023 DESC
LIMIT 1;
```
#### Algeria comes at the top from the query indicating a higher potential for investments since it has a stronger economy followed by Nigeria closely.

2.
```sql
SELECT Country, GDP_2021, GDP_2022, GDP_2023
FROM Africa_economies
ORDER BY GDP_2023 DESC
LIMIT 5;
```
#### The query returns Algeria at the top followed by nigeia then Egypt thus signifying a higher growth rate between 2021 and 2023 in Algeria as compared to other countries.


3.
```sql
SELECT Country, 
       GREATEST(Agriculture, Renewable_Energy, Real_Estate, Telecommunications, Financial_Services, Infrastructure, Manufacturing, Mining_Natural_Resources, Tourism_Hospitality, IT_Startups, Healthcare_Pharmaceuticals, Education_Training, Transportion_Logistics, Water_Sanitation, Retail_Consumer_Goods, Agribusiness_Agro_processing, Banking_Microfinance, Oil_Gas, Fisheries_Aquaculture, Media_Entertainment, Food_Beverage_Processing, Construction_Building_Materials, Automotive_Industry, Fashion_Textile_Industry, Biotechnology, Aviation, Shipping_Maritime_Services, Insurance, Sports_Recreation_Facilities) AS Max_Sector_Contribution
FROM Africa_economies;
```
#### Different countries returns different sectors therefore an investor can choose his/her suitable opportunity in chosen country to invest in but most countries are indicating among the following to be the highest GDP contributor; Agriculture,Banking, Telecommunication, Renewable energy and Financial services.

4.

```sql
SELECT Region, AVG(Agriculture) AS Avg_Agriculture_Contribution
FROM Africa_economies
GROUP BY Region
ORDER BY Avg_Agriculture_Contribution DESC;
```
#### query returns western Africa at the top while at the boottom is southern Africa indicating high chances of investment possibility in agricultural sector in the western Africa region as also been indicated that the region receives rainfall most of the times of the year due to its strategic location at the equator therefore Agricultural investments drive in the region very well.

5.

```sql
SELECT Region, SUM(Renewable_Energy) AS Total_Renewable_Energy_Contribution
FROM Africa_economies
GROUP BY Region
ORDER BY Total_Renewable_Energy_Contribution DESC;
```
#### query returns Northen Africa at the top wwhile at the bottom is southern Africa indicating more opportunities for renewable energy at the northen part of Africa due to the presence of sahara desert in the northen Africa where there is enough wind which is the key source of Renewable Energy.

6.

```sql
     SELECT Region, SUM(GDP_2023) AS Cumulative_GDP_2023
FROM Africa_economies
GROUP BY Region
ORDER BY Cumulative_GDP_2023 DESC
LIMIT 1;
```

#### Northen Africa comes at the top from the query with the highest cumulative GDP indicating a positive economic growth in the region while the lowest at middle Africa indicates not fast growing economy therefore investors may opt to choose countries in northen regions for investment since there is high chances of enough market and also Government subsidies that will make the business going.

#### Above are the findings that I got from running SQL queries in order to answer the questions and derive insights.


## TABLEAU

download [here](https://public.tableau.com/en-us/s/)

Finally I used Tableau to create reports and visualizations to communicate the insights in a easy manner that can be easily understood by both technical and non technical investors who want to get into the African countries growing markets for investment options and growth of Businesses.



I chose tableau for my project because it excels at creating dynamic and interactive visualizations. Tableau drag and drop interface makes it easy to quickly build and customize charts, graphs and dashboards which was crucial for effectively communicating the insights from my data.


I used Tableau to create reports by first connecting to my data that I had cleaned and prepared using excel then I explored the data and visualized it to ensure that it is complete without any missing values. I created visualization by dragging and dropping fields from the data pane onto the Rows and Columns shelves to create charts. I created map chart for the continent of Africa that displays different african countries, I also did the same to create the bubble charts in the show me pane to display different regions of African continent, I also created a tree map where the reports are easily understood.I also used the marks card to adjust the details of my visualization such as color size and labels.

Finally I assembled all the charts into one interactive dashboard, adjusted the layout and size of the Dashboard. I made the Dashboard interactive by using the filters that allow to drill down into specific subsets of data especially the countries to get specific data. I formated the reports using the format in the menu where I changed fonts, borders and shading to make the reports more visually appealing. Then finally I published the report on Tableau public for easy view.

Here are the charts that I made using Tableau to communicate the insights and give reports.


#### The Map Chart below gives report of the question about which country had the highest GDP 2023, in the map the coloring indicates the GDP of each country the darker the color indicates the highest GDP which is clearly shown that Algeria was the country with the highest GDP as of 2023 reports because the color in algeria is darker followed by Nigeria closely.
![gdp 2023 african countries](https://github.com/user-attachments/assets/bca5a9c6-2b86-41eb-9a82-80cdfcb1d910)


#### The Bar Chart below shows  the report of regional cumulative GDP of 2023 that has been recorded for the past three years 2021,2022,2023 and the report shows that Northen Africa Region is the one with the highest cumulative GDP as of 2023.

![2023 regional cumulative GDP](https://github.com/user-attachments/assets/f7fabb58-9b82-4b89-8dce-de3f2cbc96c9)


#### The Chart below indicates sectoral GDP  contribution in each country where the focus was on which sector has contributed highest to the GDP of the country as of 2023 and for this case we have for Nigeria where it can be clearly seen that Agriculture is the sector that has immense support and contribution to the GDP of the country as of 2023.

![sectoral GDP contribution of each country](https://github.com/user-attachments/assets/6fc223f0-8219-4788-92a5-62ccc897f9dd)


#### The packed Bubbles chart below gives a detailed report of regional agricultural contribution to the GDP of different regions of African continent, from the report it can be seen that Western Africa region is the leading in terms of GDP contribution followed by Eastern , Middle , Northen then lastly southern africa region has the lowest contribution of Agriculture towards the GDP maybe due to the hot climates of the southern Hemisphere.

![Agricultural GDP contribution](https://github.com/user-attachments/assets/74ffad7f-6410-4b9b-b43d-09c9da45316a)


#### Tree map below brings the reports of the contribution of Renewable Energy regionally where it can be seen that North Africa region is the leading in terms of renewable energy sectors followed closely by central then west then south and finally eastern Africa region being the lowest indicating any investments related to renewable energy should be tied to Northen Africa to realise a positive growth in the Business.

![Renewable energy contribution regionally](https://github.com/user-attachments/assets/622f9f6d-a8ec-4421-835e-e22c62d20cbb)


#### Below is a Link to the interactive dashboard that I have Published in Tableau Public where more reports for individual sets can be got.
#### [TABLEAU INTERACTIVE DASHBOARD FOR AFRICAN COUNTRIES' ECONOMY AND INVESTMENT OPPORTUNITIES ANALYSIS](https://public.tableau.com/app/profile/kim.ho2712/viz/AFRICANCOUNTRIESECONOMYANALYSIS/Dashboard1?publish=yes)


## Findings

1. Algeria is the country which had the highest GDP 2023.

2. In the Top 5 economic countries; Algeria, Nigeria, South Africa, Egypt and Cameroon the GDP from 2021 to 2023 has been increasing in the different countries signifying a positive economic growth.


3. According to the analysis Agriculture, Oil and gas, Renewable energy and banking and financial services has contributed the most to the GDPs of different countries with other sectors showing a potential growth and more contribution to the GDPs from 2021 to 2023.


4. From the analysis Northen Africa is the region where Agriculture has the highest contribution to GDP followed by Western Africa, Eastern Africa, Middle Africa then lastly South Africa.

5. Renewable Energy sector contributes the following amount to the GDP of the 5 regions; Northen Africa 44.2 Billion Dollars, Western Africa 24.0 Billion Dollars, Eastern Africa 16.7 Billion Dollars, Middle Africa 34.7 Billion Dollars and Southern Africa 17.5 Billion Dollars.

6. Northen Africa has the highest GDP contribution for the year 2023 with a total GDP of 1.33980 trillion Dollars.


### Recommendations

1.	Prioritize High-Growth Economies: Focus on Algeria, Nigeria, South Africa, Egypt, and Cameroon for their strong GDP growth and economic stability.

2.  Invest in Key Sectors: Target sectors with significant contributions to GDP, including agriculture, oil and gas, renewable energy, and banking and financial services.


3. 	Explore Regional Opportunities:
    
   .     Northern Africa: Major opportunities in agriculture and renewable energy, oil and gas, Telecommunicatioin and banking.
   	
   .     Western Africa: Promising for agriculture, Fishing, Infrustructure, Healthcare and Pharmaceuticals and renewable energy.
   	
   .     Eastern Africa: Growing potential in renewable energy and infrastructure, Technology, Fintech, Healthcare and Pharmaceuticals and Shipping.
   	
   .      Middle Africa: Opportunities in agriculture, Mining, Banking, Technology, Infrastructure, Aviation and renewable energy.
   	
   .      Southern Africa: Focus on renewable energy, Aviation, Construction, Infrastructure, shipping and mining.

5.  Focus on Agriculture and Renewable Energy: Invest in agricultural technologies and renewable energy projects, especially in Northern and Western Africa, where these sectors have high contributions to GDP.

6. 	Consider Financial Services Innovations: Look into fintech and expanding banking services in countries with stable economies.

7. 	Diversify Investments: Spread investments across different sectors and regions to minimize risk and maximize growth potential.



### Limitations.

My analysis of GDP sector contributions in African countries acknowledges some limitations such as potential data inaccuracies, gaps, and varying sector contributions across countries, which can complicate comparisons. Delays in reporting and the presence of informal sectors may also affect the data's relevance. To address these issues, I have used multiple data sources. Despite these challenges, the analysis aims to offer valuable insights into Africa’s economic potential and sector-specific investment opportunities.


### References

[World Bank Open Data](https://data.worldbank.org)



