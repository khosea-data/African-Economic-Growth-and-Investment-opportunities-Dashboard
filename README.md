# Dashboard for Analyzing Economic Growth and Investment opportunities in Africa

## Repository Contents

1. [Project Overview](#project-overview).

2. [Objectives](#objectives).

3. [Features](#features)
   

4. [Data Sources](#data-sources).

5. [Data Sets](#data-sets)

6. [Tools](#tools).

7. [Data Cleaning and Preparation](#data-cleaning-and-preparation).

8. [Excel Interactive Dashboard](#excel-interactive-dashboard)


9. [Exploratory Data Analysis](#exploratory-data-analysis).

10. [Data Analysis](#data-analysis).

11. [Findings](#findings).

12. [Recommendations](#recommendations).

13. [Tableau Dashboard](#tableau-dashboard)

14. [Limitations](#limitations).

15. [References](#references).




### Project Overview
Due to current rise in global finance and increase in inflation rates all over the world,individual entrepreneurs, businesses and companies have been forced to spread their risks by diversifying to various sectors in order to protect themselves from going bankrupt by depending on one source of income. In this project I have particularly chosen African nations where markets are still young and fast growing to investigate which sectors are suitable for investment and provide hope for future growth and also which countries are suitable for investing in various sectors. To get these insights I had to dive into knowing the 2023 GDP contribution of each sector of economy in different African countries because GDP contribution of a sector is a suitable indicator of whether there is growth which is signified by high contribution of the sector or whether there is stagnation signified by low contribution of the sector, this will help investors and other entrepreneurs to get to know which sectors are suitable for investing. In order to understand which country is suitable, I used the GDP contribution of the past 3 years 2021,2022 and 2023 in order to understand which countries are experiencing economic growth which is signified by a high GDP which might be a suitable place for investing. I also grouped the countries into regions in order to know which regions are suitable for investment in Africa. This project is important because it will help investors, entrepreneurs and startups who wish to get into African market which is growing so fast due to it's population increase to pinpoint those sutable sectors and countries where they can diversify into and grow their investment portfolio for their growth. It also helps for those who are planning for future investing to get more insights on how the market will be and how the current growth will influence the future growth of certain sectors. In order to accomplish this goal I came up with the following Business questions that will enable me get the insights and have the best suitable decisions about investing in Africa.


1)Which country has the highest GDP in 2023?

Reason for asking this question; Understanding which country had the highest GDP contribution indicates large economic sze which helps to identify potential markets for investment or expansion, it also indicates economic power and potential for regional investment.


2)How does the GDP of the top 5 African economies have changed from 2021 to 2023?

Reason for asking this question; This helps in analysing growth trajectory of leading economies highlighting which countries are expanding faster or which may be facing economic stagnation.


3)Which sector contributes the most to the GDP in each country?

Reason for this Question; Identifying the dominant sectors provides insights into the economic drivers of each country helping business focus on industry specific strategies for market entry.


4)How does the contribution of agriculture sector to GDP vary across region?

Reason for this Question; Agriculture plays a crucial role in many African countries especially in rural areas, understanding its contribution helps target investments,aid and innovation in those areas.


5)What is the total contribution of Renewable Energy to GDP in each region?

Reason for this Question; Renewable Energy is a fast-growing sector in Africa especially in countries aiming to diversify their energy mix. Understanding its contribution to GDP can highlight growth markets.


6)Which regions has the highest cumulative GDP as of 2023?

Reason for asking this question;Identifying the region the higher cumulative GDP helps businesses prioritize regions for market entry and expansion.

In order to get these insights and answers to these questions I laveraged data analysis tools EXCEL, SQL and TABLEAU which helped me get my final findings about investment opportunities in Africa.

# Data Collection

In Data Sourcing and collection I did manual research by searching for and gathering data from different websites and public databases like WorldBank Data since complete dataset was not readily available. I manually researched and recorded each piece of data by ensuring accuracy and reliability of the information by cross-referrencing different sources. Inputing data into Excel, I entered each data point manually ensuring that the information was organized correctly. This involved creating columns for different variables for example agriculture, renewable energy and filling in each row with the appropriate data. I structured the data in tabular format where each row represented a specific entry and each column represented a variable or a parameter.

# Data Analysis Tools that I used.


## EXCEL

I chose Excel for this project because it is a versatile and accessible tool that offers powerful features for data Exploration, Cleaning and Visualization. With Pivot tables I was able to summarize and analyze the data quickly by creating visualizations that enabled me to present my findings in a clear and impactful way making it easy to communicate insights to both technical and non technical stakeholders.

I did the following using Excel in preparation of the data for Analysing

#### Handling Missing Values

I used conditional formating to highlight missing values and selected Blanks. I deleted some of the missing values after filtering them. I also filled some missing values with appropriate data based on the collection.

#### Data Cleaning

I did data cleaning by removing duplicates using the remove duplicates option in the data tab. I standardized the data by changing the text cases using UPPER for upper case LOWER for lower case and PROPER to make the first letter to be in upper case. I also did CONCATENATION to combine texts especially in countries and those that had splitted during entry, I also did splitting using text to columns in data tab and finally I did data types conversion by using the excel inbuilt power query.

#### Data Formating

I did data Formating to improve readability and usability of the data where i did number formating for currencies and putting them in $ dollar form together with custom to large numbers which was specifically Billions.

Finally I used Excel Pivot tables Pivot tables to do quick summary to allow flexibility in analysis, I also created reports using Pivot charts and included use of slicers for interactive data exploration where i can quickly narrow down results to a specific region and country, through thus i was able to make it easier to analyse and draw insights from my data. I was able to create a dashboard where i joined all the pivot charts and applied the slicer to connect to all charts. 

Below are some of the Visualizations that I made using pivot charts to communicate insights.


## a bar chart of Regional agricultural contribution where Western Africa is the leading in agriculture sectorwise with $572.7B ![image](https://github.com/user-attachments/assets/8e1ebc17-e923-4852-986c-f4546bf4b44f)
## a bar chart of 2023 GDP of each country where Algeria is at the top with the highest GDP among all the other countries by having $621B.![image](https://github.com/user-attachments/assets/e418c67d-ff72-4fc6-9c1c-86579f5cdb73)
### a line graph of GDP growth of Top 5 countries from 2021 to 2023, Algeria and Cameroon have experienced high economic growth in between the years as shown by their rise in GDP while Nigeria, South Africa and Egypt have shown slow economic growth in between the years as shown by their slight increase in the GDP![image](https://github.com/user-attachments/assets/2754eb95-4543-4ecd-bd3a-511f32f0ef67)
## a pie chart of Renewable Energy sector contribution per REGION, The result show that Northen Africa is the leading among all the five regions with a total contribution of $44.2B![image](https://github.com/user-attachments/assets/8ff3cbe3-9b39-49f2-a679-2560c27e3cb4)
## a line graph of Sum of Regional 2023 GDP contribution where Northen Africa is seen to be the leading among the five regions with a total sum of $1382B![image](https://github.com/user-attachments/assets/2847965a-feb1-4e8b-bb7b-34fb2539c5de)

#### To check the intractive dashboard click on the link below,

##### Excel interactive dashboard


## sql (postgresql)



I chose SQL as a tool for my project because it allowed me to write custom queries to efficiently extract, manipulate and aggregate data from the table, sql provided scalability and flexibility i neede to derive meaningful insights.


I used SQL to do Exploratory data analysis in order to get insights of the Business questions about investing in Africa.

Before analysis, I first saved in Excel in csv comma delimited format, then I imported the data to postgresql pgadmin with correct columns to ensure easy importing and data accuracy. 
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
#### query returns Algeria thus signifying a higher growth rate between 2021 and 2023 in the country.


3.
```sql
SELECT Country, 
       GREATEST(Agriculture, Renewable_Energy, Real_Estate, Telecommunications, Financial_Services, Infrastructure, Manufacturing, Mining_Natural_Resources, Tourism_Hospitality, IT_Startups, Healthcare_Pharmaceuticals, Education_Training, Transportion_Logistics, Water_Sanitation, Retail_Consumer_Goods, Agribusiness_Agro_processing, Banking_Microfinance, Oil_Gas, Fisheries_Aquaculture, Media_Entertainment, Food_Beverage_Processing, Construction_Building_Materials, Automotive_Industry, Fashion_Textile_Industry, Biotechnology, Aviation, Shipping_Maritime_Services, Insurance, Sports_Recreation_Facilities) AS Max_Sector_Contribution
FROM Africa_economies;
```
#### Different countries returns different sectors therefore an investor can choose his/her suitable opportunity in chosen country to invest in.

4.

```sql
SELECT Region, AVG(Agriculture) AS Avg_Agriculture_Contribution
FROM Africa_economies
GROUP BY Region
ORDER BY Avg_Agriculture_Contribution DESC;
```
#### query returns western Africa at the top while at the boottom is southern Africa indicating high chances of investment possibility in agricultural sector in the western Africa region.

5.

```sql
SELECT Region, SUM(Renewable_Energy) AS Total_Renewable_Energy_Contribution
FROM Africa_economies
GROUP BY Region
ORDER BY Total_Renewable_Energy_Contribution DESC;
```
#### query returns Northen Africa at the top wwhile at the bottom is southern Africa indicating more opportunities for renewable energy at the northen part of Africa.

6.

```sql
     SELECT Region, SUM(GDP_2023) AS Cumulative_GDP_2023
FROM Africa_economies
GROUP BY Region
ORDER BY Cumulative_GDP_2023 DESC
LIMIT 1;
```

#### Northen Africa comes at the top from the query with the highest cumulative GDP indicating a positive economic growth in the region while the lowest at middle Africa indicates not fast growing economy therefore investors may opt to choose countries in northen regions for investment

#### Above are the findings that I got from running SQL queries in order to answer the questions and derive insights.


## TABLEAU

Finally I used Tableau to create reports and visualizations to communicate the insights in a easy manner that can be easily understood by both technical and non technical staff.



I chose tableau for my project because it excels at creating dynamic and interactive visualizations. Tableau drag and drop interface makes it easy to quickly build and customize charts, graphs and dashboards which was crucial for effectively communicating the insights from my data.


I used Tableau to create reports by first connecting to my data that I had cleaned and prepared using excel then I explored the data and visualized it to ensure that it is complete without any missing values. I created visualization by dragging and dropping fields from the data pane onto the Rows and Columns shelves to create charts. I created map chart for the continent of Africa that displays different african countries, I also did the same to create the bubble charts in the show me pane to display different regions of African continent, I also created a tree map where the reports are easily understood.I also used the marks card to adjust the details of my visualization such as color size and labels.

Finally I assembled all the charts into one interactive dashboard, adjusted the layout and size of the Dashboard. I made the Dashboard interactive by using the filters that allow to drill down into specific subsets of data. I formated the reports using the format in the menu where I changed fonts, borders and shading to make the reports more visually appealing. Then finally I published the report on Tableau public for easy view.

Here are the charts that I made using Tableau to communicate the insights.






















### Objectives
  -Offer a detailed view of economic and socio-political conditions in African countries.


  -Support researchers, investors, and businesses in making informed decisions based on reliable data.

  -Enhance understanding of African economies through accessible and interactive data visualizations.



  ### Features

  -  Country-Specific Information: Access detailed information on political stability, tax rates, climate, and infrastructure for each country. This information provides context to the economic data and helps in understanding the broader environment in which the economies operate.

  -  Sectoral GDP Analysis: Examine contributions from various sectors like agriculture, manufacturing, and renewable energy. The analysis highlights the impact of different sectors on the overall GDP, showcasing key areas of economic activity and growth.

   -  Excel Data Analysis: Utilize the provided Excel file for detailed data analysis and further exploration. The Excel file contains raw data that can be used for various analyses, providing a flexible tool for data-driven decision-making.


   -  SQL Data Analysis: Perform complex queries to extract meaningful insights from the dataset. The SQL scripts included in the repository allow for detailed data manipulation and retrieval, making it easier to analyze economic trends and sectoral contributions.

   -  Interactive Tableau Dashboard: Visualize key economic indicators such as GDP, population, tax rates, and more for African countries. The dashboard provide an intuitive and interactive way to explore and analyse the data.

   -  Trend Analysis: Track economic growth and changes over time with historical data from 2021 to 2023. This allows for identification of trends and patterns in economic performance helping in forecasting strategic planning.




    



### Data Sources

africa_economies: The dataset used for this analysis “Africa_economies.csv”. Contains economic data including GDP, population, and sectoral contributions for each African country.



country_data: The dataset “country_data.csv” includes country-specific information such as capital cities, political stability, tax rates, climate, dominant language in the nation and key infrastructure details.

### Data Sets
[Africa_economies](https://github.com/khosea-data/African-Economic-Growth-and-Investment-opportunities-Dashboard/blob/main/Africa_economies.csv)


[Country_data](https://github.com/khosea-data/African-Economic-Growth-and-Investment-opportunities-Dashboard/blob/main/country_data.csv)


### Tools

-Excel- Used for Data Cleaning  [Download Here](https://www.office.com/launch/excel) 

-postgresql- Used for Data Analysis  [Download Here](postgresql.org/download/)

-Tableau- Used for Creating Reports  [Download Here](tableau.com/products/public/download)

### Data Cleaning and Preparation

During the beginning of data preparation phase,I did the following using excel;

1. Data Loading and Inspecting.
2. Handling Missing Values.
3. Data Cleaning and Formatting.

### Excel Interactive Dashboard

Explore Interactive Dashbosrd here

[download excel file](https://github.com/khosea-data/African-Economic-Growth-and-Investment-opportunities-Dashboard/blob/main/Excel%20Data%20Analysis%20Dashboard%20Project.xlsx)

### Exploratory Data Analysis

Exploratory Data Analysis involved exploring the African_Economy_Data and Country_Data to answer questions below that are important to know investment opportunities in African Nations.

1.Which African country has the highest GDP in 2023?

2.How has the GDP of the top 5 African economies changed from 2021 to 2023?

3.Which sector contributes the most to the GDP in each country?

4.How does political stability correlate with GDP growth in different countries?



5.How does the contribution of the Agriculture sector to GDP vary across regions?

6.What is the total contribution of Renewable Energy to GDP for each region?

7.Which region has the highest cumulative GDP in 2023?

### Data Analysis

I worked with the following codes to answer the questions and derive the insights.

1.
```sql

SELECT Country, GDP_2023
FROM africa_economies
ORDER BY GDP_2023 DESC
LIMIT 1;
```




2.
```sql
SELECT Country, GDP_2021, GDP_2022, GDP_2023
FROM Africa_economies
ORDER BY GDP_2023 DESC
LIMIT 5;
```

3.
```sql
SELECT Country, 
       GREATEST(Agriculture, Renewable_Energy, Real_Estate, Telecommunications, Financial_Services, Infrastructure, Manufacturing, Mining_Natural_Resources, Tourism_Hospitality, IT_Startups, Healthcare_Pharmaceuticals, Education_Training, Transportion_Logistics, Water_Sanitation, Retail_Consumer_Goods, Agribusiness_Agro_processing, Banking_Microfinance, Oil_Gas, Fisheries_Aquaculture, Media_Entertainment, Food_Beverage_Processing, Construction_Building_Materials, Automotive_Industry, Fashion_Textile_Industry, Biotechnology, Aviation, Shipping_Maritime_Services, Insurance, Sports_Recreation_Facilities) AS Max_Sector_Contribution
FROM Africa_economies;
```

4.

```sql
SELECT c.Country, c.GDP_2023 - c.GDP_2021 AS GDP_Growth, i.Political_Stability
FROM Africa_economies c
JOIN country_info i ON c.Country = i.Country
ORDER BY GDP_Growth DESC;
```



5.


```sql
SELECT Region, AVG(Agriculture) AS Avg_Agriculture_Contribution
FROM Africa_economies
GROUP BY Region
ORDER BY Avg_Agriculture_Contribution DESC;
```

6.


```sql
SELECT Region, SUM(Renewable_Energy) AS Total_Renewable_Energy_Contribution
FROM Africa_economies
GROUP BY Region
ORDER BY Total_Renewable_Energy_Contribution DESC;
```

7.

```sql
     SELECT Region, SUM(GDP_2023) AS Cumulative_GDP_2023
FROM Africa_economies
GROUP BY Region
ORDER BY Cumulative_GDP_2023 DESC
LIMIT 1;
```
## Findings

1. Algeria is the country which had the highest GDP 2023.

2. In the Top 5 economic countries; Algeria, Nigeria, South Africa, Egypt and Cameroon the GDP from 2021 to 2023 has been increasing in the different countries signifying a positive economic growth.


3. According to the analysis Agriculture, Oil and gas, Renewable energy and banking and financial services has contributed the most to the GDPs of different countries with other sectors showing a potential growth and more contribution to the GDPs from 2021 to 2023.


4. In countries that have fair and good political stability like Algeria, Burkina Faso, Cameroon, Nigeria, Angola, Egypt, Benin, South Africa, Chad, Kenya and Ethiopia with many other countries have shown a positive change in GDP growth from 2021 to 2023.


5. From the analysis Northen Africa is the region where Agriculture has the highest contribution to GDP followed by Western Africa, Eastern Africa, Middle Africa then lastly South Africa.

6. Renewable Energy sector contributes the following amount to the GDP of the 5 regions; Northen Africa 44.2 Billion Dollars, Western Africa 35.10 Billion Dollars, Eastern Africa 24.6 Billion Dollars, Middle Africa 20.3 Billion Dollars and Southern Africa 17.5 Billion Dollars.

7. Northen Africa has the highest GDP contribution for the year 2023 with a total GDP of 1.33980 trillion Dollars.


### Recommendations

1.	Prioritize High-Growth Economies: Focus on Algeria, Nigeria, South Africa, Egypt, and Cameroon for their strong GDP growth and economic stability.

2.  Invest in Key Sectors: Target sectors with significant contributions to GDP, including agriculture, oil and gas, renewable energy, and banking and financial services.

3.  Leverage Political Stability: Choose countries with stable political environments such as Algeria, Burkina Faso, Cameroon, Nigeria, Angola, Egypt, Benin, South Africa, Chad, Kenya, and Ethiopia.

4. 	Explore Regional Opportunities:
        o	Northern Africa: Major opportunities in agriculture and renewable energy.
        o	Western Africa: Promising for agriculture and renewable energy.
        o	Eastern Africa: Growing potential in renewable energy and infrastructure.
        o	Middle Africa: Opportunities in agriculture and renewable energy.
        o	Southern Africa: Focus on renewable energy and mining.

5.  Focus on Agriculture and Renewable Energy: Invest in agricultural technologies and renewable energy projects, especially in Northern and Western Africa, where these sectors have high contributions to GDP.

6. 	Consider Financial Services Innovations: Look into fintech and expanding banking services in countries with stable economies.

7. 	Diversify Investments: Spread investments across different sectors and regions to minimize risk and maximize growth potential.

### Tableau Dashboard
Explore interactive Dashboard here
[African Economic Growth and Investment Opportunities Dashboard](https://public.tableau.com/app/profile/kim.ho2712/viz/africaneconomicdata/Dashboard1?publish=yes)


### Limitations.

My analysis of GDP sector contributions in African countries acknowledges some limitations such as potential data inaccuracies, gaps, and varying sector contributions across countries, which can complicate comparisons. Delays in reporting and the presence of informal sectors may also affect the data's relevance. To address these issues, I have used multiple data sources. Despite these challenges, the analysis aims to offer valuable insights into Africa’s economic potential and sector-specific investment opportunities.


### References

[World Bank Open Data](https://data.worldbank.org)



