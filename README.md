# Unlocking Investment potential: Analyzing key growth sectors in African countries.

## Project Contents

1. [Project Overview](#project-overview).

2. [Data Sources](#data-sources).

3. [Data Collection](#data-collection)
   

4. [Data Analysis Tools that I used](#data-analysis-tools-that-i-used).

5. [Excel](#excel)

6. [SQL (postgresql)](#sql (postgresql)).
   
7. [TABLEAU](#tableau)
 
8.   [Findings](#findings).

9. [Recommendations](#recommendations).

10. [Limitations](#limitations).

11. [References](#references).


##  Why this Project?

I chose to undertake this project with the specific goal of helping entrepreneurs and investors who are looking to expand their ambitions into African markets. In the face of rising global financial pressures and increasing inflation rates, many businesses are seeking to diversify their investments as a way to mitigate risk and drive sustainable growth. By expanding into various sectors and regions, companies can better adapt to changing economic conditions and secure long-term success.

Leveraging data analysis, this project aims to uncover promising markets and investment opportunities in African countries. The analysis will focus on identifying high-growth sectors that provide valuable opportunities for diversification, allowing companies and startups to enhance their portfolios while focusing on the dynamic economic landscape of the continent.








### Project Overview
In this project, I analyzed 54 African nations with young and rapidly growing markets to determine which sectors offer the best opportunities for investment and future growth. Additionally, I explored which countries are most favorable for investing in various sectors.

To gain these insights, I focused on the 2023 GDP contribution of each economic sector across different African countries. Sectoral GDP contribution serves as a key indicator of growth, with higher contributions signaling thriving sectors and lower contributions suggesting stagnation. This information provides entrepreneurs and investors with a clear understanding of which sectors are most promising for investment.

To assess which countries are ideal for investment, I analyzed the GDP contributions over the past three years (2021, 2022, and 2023) to identify nations experiencing sustained economic growth. A rising GDP typically reflects a growing economy, offering a more favorable environment for business expansion and investment opportunities.

Furthermore, I grouped the countries into regions to determine which parts of Africa present the best investment potential. Regions with higher contributions from specific sectors signal areas suitable for growth and investment opportunities.

![Screenshot (40)](https://github.com/user-attachments/assets/cab71aeb-23f9-4cab-a1fc-6304f318a787)




## Business Questions


### 1) Which country has the highest GDP in 2023?

#### Reason for asking this question;

 Identifying the country with the highest GDP highlights potential markets for investment, reflecting economic size and strength, and indicating opportunities for expansion.




### 2) How does the GDP of the top 5 African economies have changed from 2021 to 2023?

#### Reason for asking this question;
Analyzing the GDP changes of the top 5 economies reveals growth changes, highlighting which countries are expanding rapidly, which may be facing stagnation, and identifying potential investment opportunities in fast-growing markets.


### 3) Which sector contributes the most to the GDP in each country?

#### Reason for this Question;
Identifying the top contributing sectors reveals the key economic drivers in each country, enabling businesses to develop industry-specific strategies for market entry and investment opportunities

#### 4) How does the contribution of agriculture sector to GDP vary across region?

#### Reason for this Question;
Agriculture plays a crucial role in many African countries especially in rural areas, understanding its contribution helps target investments and innovation in those areas.


### 5) What is the total contribution of Renewable Energy to GDP in each region?

#### Reason for this Question;
Renewable Energy is a fast-growing sector in Africa especially in countries aiming to diversify their energy portfolio. Understanding its contribution to GDP can highlight growth markets.


### 6) Which regions has the highest cumulative GDP as of 2023?

#### Reason for this question;
Identifying the region with the higher cumulative GDP as of 2023 helps businesses prioritize regions for market entry and expansion.


### 7) How does population of each country correlate with cumulative GDP contribution between 2021 and 2023?

#### Reason for this question;
 Understanding the relationship between population and cumulative GDP helps businesses and investors identify which countries offer sufficient market size and potential labor resources for successful investment and operations.

### 8) How does Geographical area coverage of each country correlate with total cumulative GDP?

#### Reason for this question;
 Analyzing the correlation between geographical area and total cumulative GDP provides insights into whether larger countries tend to have higher GDP due to greater resource availability and potential for business expansion, particularly in sectors like agriculture.



To gain insights and answers to these questions, I leveraged the following data analysis tools: Excel, SQL, and Tableau. These tools facilitated my analysis and helped me arrive at comprehensive findings regarding investment opportunities in Africa.





# Dataset

The primary dataset used for this analysis is the "Africa_Economies.csv" file containing detailed information about each country and 
 GDP contribution of each sector.



# Data Sourcing and Collection

In Data Sourcing and collection I did manual research by searching for and gathering data from different websites and public databases like [WorldBankData](https://data.worldbank.org/) since complete dataset was not readily available. I manually researched and recorded each piece of data by ensuring accuracy and reliability of the information by cross-referrencing different sources. Inputing data into Excel, I entered each data point manually ensuring that the information was organized correctly. This involved creating columns for different variables for example country, region, agriculture, renewable energy and filling in each row with the appropriate data. I structured the data in tabular format where each row represented a specific entry and each column represented a variable or a parameter.

# Data Analysis Tools that I used.


## EXCEL



I chose Excel for this project because it is a versatile and accessible tool that offers powerful features for data Exploration, Cleaning and Visualization. With Pivot tables I was able to summarize and analyze the data quickly by creating visualizations that enabled me to present my findings in a clear and impactful way making it easy to communicate insights that can be understood by  both technical and non technical individuals.

I did the following using Excel in preparation of the data for Analysing

#### Handling Missing Values

I used conditional formating to highlight missing values and selected Blanks. I deleted some of the missing values after filtering them. I also filled some missing values with appropriate data based on the collection.

![Screenshot (44)](https://github.com/user-attachments/assets/47403395-940b-4dc9-bec6-b14f10363537)

#### Data Cleaning

I did data cleaning by removing duplicates using the remove duplicates option in the data tab. I standardized the data by changing the text cases using UPPER for upper case LOWER for lower case and PROPER to make the first letter to be in upper case. I also did CONCATENATION to combine texts especially in countries and those that had splitted during entry, I also did splitting using text to columns in data tab and finally I did data types conversion by using the excel inbuilt power query.
![Screenshot (42)](https://github.com/user-attachments/assets/fc0bfce1-4086-4638-bc0c-aaad2f007376)


## 
![Screenshot (43)](https://github.com/user-attachments/assets/6912bcfe-15d2-4e0e-9bb1-f79113b10c90)


## 

![Screenshot (45)](https://github.com/user-attachments/assets/cb752bc6-543d-40d6-8fba-ee7baee9e0c0)


##

![Screenshot (39)](https://github.com/user-attachments/assets/abb37bd1-9d42-48c2-a59c-0eec2159d235)

#### Data Formating

I did data Formating to improve readability and usability of the data where I did number formating for currencies and putting them in $ dollar form together with custom to large numbers which was specifically Billions.

Finally I used Excel Pivot tables to do quick summary to allow flexibility in analysis, I also created reports using Pivot charts and included use of slicers for interactive data exploration where I can quickly narrow down results to a specific region and country, through this I was able to make it easier to analyse and draw insights from my data. I was able to create a dashboard where I joined all the pivot charts and applied the slicer to connect to all charts for easy analysis and reporting. 
# 

![Screenshot (41)](https://github.com/user-attachments/assets/7174c0f6-63f4-4aea-9b56-f579e75094f4)




Below are some of the Visualizations that I made using pivot charts to communicate insights.



![image](https://github.com/user-attachments/assets/f26ae48b-dc72-4986-82a6-f2248ee7c5e6)


#### A bar chart illustrating regional agricultural GDP contributions shows that Western Africa leads the sector with a contribution of $572.7 billion



![image](https://github.com/user-attachments/assets/5f9f1141-6f1c-4307-a4ec-727960f98a99)



#### A bar chart of 2023 GDP by country shows Algeria leading with the highest GDP at $621 Billion, surpassing all other countries.



![image](https://github.com/user-attachments/assets/942055c5-7958-4b26-835f-9a399bd531dd)

#### A line graph of GDP growth for the top 5 countries from 2021 to 2023 shows that Algeria and Cameroon have experienced significant economic growth, as indicated by their sharp rise in GDP. In contrast, Nigeria, South Africa, and Egypt have shown slower economic growth, with only slight increases in GDP over the period




![image](https://github.com/user-attachments/assets/e8e15715-6617-4480-b7fd-88c342d25a61)


#### A horizontal bar chart of renewable energy sector contributions by region shows Northern Africa leading with a total contribution of $44.2 Billion, surpassing the other four regions.





![image](https://github.com/user-attachments/assets/33746f50-9f9e-4f17-9121-976f906908b5)


#### A bar chart illustrating the sum of regional GDP contributions for 2023 shows that Northern Africa leads among the five regions, with a total contribution of $1,382 Billion.



Finally I used Excel Pivot tables to do quick summary to allow flexibility in analysis, I also created reports using Pivot charts and included use of slicers for interactive data exploration where I can quickly narrow down results to a specific region and country, through this I was able to make it easier to analyse and draw insights from my data. I was able to create a dashboard where I joined all the pivot charts and applied the slicer to connect to all charts for easy analysis and reporting. 


#### The following is an image of how the final interactive dashboard looks like.
![Screenshot (29)](https://github.com/user-attachments/assets/28cda1d6-240b-4760-8649-0e686c369d88)



### Kindly Find the Interactive Dashboard on the files that i have uploaded for more visualization.


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
![Screenshot (19)](https://github.com/user-attachments/assets/d7926bd9-3f42-4601-911e-4d124d9b52a5)


#### The Bar Chart below shows  the report of regional cumulative GDP of 2023 that has been recorded for the past three years 2021,2022,2023 and the report shows that Northen Africa Region is the one with the highest cumulative GDP as of 2023.

![Screenshot (22)](https://github.com/user-attachments/assets/a16b1736-21b1-4bf1-b6f5-7c3c5e0441ec)



#### The Chart below indicates sectoral GDP  contribution in each country where the focus was on which sector has contributed highest to the GDP of the country as of 2023 and for this case we have for Nigeria where it can be clearly seen that Agriculture is the sector that has immense support and contribution to the GDP of the country as of 2023.

![Screenshot (13)](https://github.com/user-attachments/assets/496c463f-c86d-4533-a07e-523f143fc20b)


#### The packed Bubbles chart below gives a detailed report of regional agricultural contribution to the GDP of different regions of African continent, from the report it can be seen that Western Africa region is the leading in terms of GDP contribution followed by Eastern , Middle , Northen then lastly southern africa region has the lowest contribution of Agriculture towards the GDP maybe due to the hot climates of the southern Hemisphere.

![Screenshot (25)](https://github.com/user-attachments/assets/4074f25c-cffa-4c9b-9588-a91d426106a0)


#### Tree map below brings the reports of the contribution of Renewable Energy regionally where it can be seen that North Africa region is the leading in terms of renewable energy sectors followed closely by central then west then south and finally eastern Africa region being the lowest indicating any investments related to renewable energy should be tied to Northen Africa to realise a positive growth in the Business.

![Screenshot (21)](https://github.com/user-attachments/assets/12299d89-650c-4939-9b11-4f4bc6501e9e)


#### The Scatter plot below shows the correlation between population in African countries and cumulative GDP of each country where we can clearly see that countries with a higher population have a higher cumulative GDP. This is so important because for investors and businessmen may chooose countries with higher population because there is available market and also availability of labor which will make business operations easy.
![Screenshot (18)](https://github.com/user-attachments/assets/10908e60-a926-4765-ac49-b6e47e06fb08)


### The Scatter plot below shows the correlation between Geographical area coverage and Total Cumulative GDP of each country. From the scatter plot we can see that there are some countries with larger area coverage but wiith a lower cumulative GDP and others with large coverage with a significantly higher GDP, this helps investors to decide which areas they can start their businesses in maybe based on region or even geopolitical issues in the country but mostly they need to invest in countries with large area coverage because of availability of space which will help in future expansion.

![Screenshot (17)](https://github.com/user-attachments/assets/27997872-241e-40cc-883c-b2e42b543c2e)

### The following is a picture of the final interactive dashboard I created using Tableau.

![Screenshot (26)](https://github.com/user-attachments/assets/79dc52ff-2626-4010-aafa-a95c635852a5)


#### Below is a Link to the interactive dashboard that I have Published in Tableau Public where more reports for individual sets can be got.
#### [TABLEAU INTERACTIVE DASHBOARD FOR AFRICAN COUNTRIES' ECONOMY AND INVESTMENT OPPORTUNITIES ANALYSIS](https://public.tableau.com/app/profile/kim.ho2712/viz/AFRICANCOUNTRIESECONOMYANALYSIS/Dashboard1?publish=yes)


## Findings

1. Algeria is the country which had the highest GDP 2023.

2. In the Top 5 economic countries; Algeria, Nigeria, South Africa, Egypt and Cameroon the GDP from 2021 to 2023 has been increasing in the different countries signifying a positive economic growth.


3. According to the analysis Agriculture, Oil and gas, Renewable energy and banking and financial services has contributed the most to the GDPs of different countries with other sectors showing a potential growth and more contribution to the GDPs from 2021 to 2023.


4. From the analysis Northen Africa is the region where Agriculture has the highest contribution to GDP followed by Western Africa, Eastern Africa, Middle Africa then lastly South Africa.

5. Renewable Energy sector contributes the following amount to the GDP of the 5 regions; Northen Africa 44.2 Billion Dollars, Western Africa 24.0 Billion Dollars, Eastern Africa 16.7 Billion Dollars, Middle Africa 34.7 Billion Dollars and Southern Africa 17.5 Billion Dollars.

6. Northen Africa has the highest GDP contribution for the year 2023 with a total GDP of 1.33980 trillion Dollars.

7. Countries that have a higher population are showing a higher economic growth as it is denoted by a higher cumulative GDP.

8. Countries with a larger geographical area coverage are showing a significant higher cumulative GDP therefore showing a fast economic growth.

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

8.   Focus on areas with a higher population because there will be potential readily available market and also source of labor that will actually expedite the operations of the business hence bringing more return.

9.   Put into consideration countries with larger geographical area because this will help for future expansion especially if you are getting into agriculture where you may need a larger piece of land for farming and growing crops.

### Limitations.

My analysis of GDP sector contributions in African countries acknowledges some limitations such as potential data inaccuracies, gaps, and varying sector contributions across countries, which can complicate comparisons. Delays in reporting and the presence of informal sectors may also affect the data's relevance. To address these issues, I have used multiple data sources. Despite these challenges, the analysis aims to offer valuable insights into Africa’s economic potential and sector-specific investment opportunities.


### References

[World Bank Open Data](https://data.worldbank.org)



