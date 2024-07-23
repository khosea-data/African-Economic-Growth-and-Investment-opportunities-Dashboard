# Dashboard for Analyzing Economic Growth and Investment in Africa

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
This project offers a comprehensive analysis and interactive visualization of the economic landscape across African nations, with a special focus on how sectoral investment opportunities have contributed to GDP growth and overall economic development. By leveraging data visualization tools like Tableau and SQL for data manipulation, this project highlights the impact of key sectors such as agriculture, manufacturing, renewable energy, and technology on the economic prosperity of African countries. Through detailed datasets and insightful visualizations, we aim to provide a valuable resource for understanding the dynamics of sectoral contributions to GDP and the potential for future investments in Africa.



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


[OpenAI](https://www.openai.com)
