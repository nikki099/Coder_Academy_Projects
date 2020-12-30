
# Table of Contents
______________________________________________________________________________________________________________

* [Project Title](#Project-Title)
* [Project Synopsis](#Project-Synopsis)
  * [Key Questions Answered through Analysis](#Key-Questions-Answered-through-Analysis)
  * [Project Scope](#Project-Scope)
  * [Project Analysis Files](#Project-Analysis-Files)
* [Data Sets](#Data-Sets)
* [Recommendation](#Recommendation)



## Project Title 
* “Finding the Affordable Suburbs to Buy in SE Brisbane Area”

## Project Synopsis 
This project aims to help a young couple, who is planning to purchase a 3-4 bedroom house in the South Eastern area of Brisbane based on an analysis of the historical house prices sold in 10 selected suburbs over the last decade but mainly between 2017-2020.

### Key Questions Answered through Data Analysis 
1.	Over the last 10 years (2011-2020), how many properties are sold yearly by the top 3 property types?
2.	Over the last 4 years (2017-2020), how many houses were sold by bedroom numbers? And what's the overall trend among these suburbs?
3.	What is the min, max and median sold price for House with 3 or 4 bedrooms in each suburb?
4.	What's the trend of the number of houses sold and the sold median price for 3 and 4 bedroom houses?
5.	Are there any correlations between the house sold price and other factors?

### Project Scope
* Compared the summary median price data of the sold houses from each suburb between Nov 2019-Dec 2020 on [REA](https://www.realestate.com.au/sold/) and [Domain](https://www.domain.com.au/) to understand the price differences between these 2 sites.
* Compared with the website traffic and [Canstar domain ratings](https://www.canstarblue.com.au/stores-services/real-estate-vs-domain/) between the 2 sites, to decide which site to pull the sold property listing details for in-depth analysis.<br>
* Upon selecting REA as the data source, we dived deeper to analyze the total number of properties sold between 2006-2020.<br>
* However, due to some of the key suburbs, which the clients is interested in, doesn't have data captured before 2017, we focused on analyzing the number of sold properties and the median price for 3-4 bedroom houses between 2017-2020.<br>
* Next we switched back to examine all data collected over past 14 years, to explore what factors may have a (linear) correlation with the house price.<br>
* Finally, based on the above analysis, a selection of suburbs is recommended to the couple, to assist them make an informed decision on which suburb(s) they should focus on exploring for their house purchase next year.<br>
</font>

### Project Analysis Files
* The analysis script and the related data visualizations can be found in the **"Analysis"** Jupyter Notebook in this Github Repository.
* The data cleaning and prep script can be found in the **"Data_Cleaning"** Jupyter Notebook in this Github Repository.

## Data Sets

This project collected 4 sets of data for analysis purpose:<br>
1. REA - Suburb based median house price (summary data)<br>
 * Direct data access from a Jason file through [REA](https://realestate.com.au) API
 * How to access: the API query script is included in the **"Data_Cleaning"** Jupyter Notebook in this Github Repository.


2.	Domain - Suburb based median house price (summary data)<br>
 * Data scraped from [Domain.com.au](https://www.domain.com.au/) to compare with REA data
 * How to access: this data is stored in the Excel file "[domain_market_trend.xlsx](https://docs.google.com/spreadsheets/d/1Bp3Ufrkx_YNkrzFG0Fo8glmVHHkjc6rOXsNbw13BJds/edit?usp=sharing)" in the [Google Drive “Data” folder](https://drive.google.com/drive/folders/12qFycpdnDk8_SrNtqTyAVV8o0O0o-wPf?usp=sharing).


3.	Website Traffic and Overall Domain Rating Data<br>
 * Web traffic data (REA vs Domain) collected from [SEMRUSH](https://www.semrush.com/)
 * Overall Domain Rating (REA vs Domain) collected from [Canstar](https://www.canstarblue.com.au/stores-services/real-estate-vs-domain/)
 * Through comparing the summary house median prices, web traffic and overall domain rating data between these 2 sites, the project finally chose REA as the source to explore the detailed sold house listing information for project analysis. 
 * How to access: this data is stored in the Excel file “[Traffic_Rating.xlsx](https://docs.google.com/spreadsheets/d/1XQYlDbTnuqz_YNu0iszhu9sh3PqkX1u9778QthOYeAI/edit?usp=sharing)" in the [Google Drive “Data” folder](https://drive.google.com/drive/folders/12qFycpdnDk8_SrNtqTyAVV8o0O0o-wPf?usp=sharing).


4.	REA – Sold Houses Price Data (2011-2020, mainly focusing on 2017-2020)<br>
 * Sold house data scraped from the [Sold section on realestate.com.au](https://www.realestate.com.au/sold/) from 10 SE Brisbane Suburbs.
 * The collected data includes fields such as the property address, property size, sold prices, sold date, bedroom, bathroom and car park number and etc..
 * How to access: this data is stored the following csv files (one file for each suburb), in the [Google Drive “Data” folder](https://drive.google.com/drive/folders/12qFycpdnDk8_SrNtqTyAVV8o0O0o-wPf?usp=sharing).
:<br>

         *[realestate.com.au_SOLD_Algester.csv](https://docs.google.com/spreadsheets/d/1TPHdKGY-VXani8OVQuFE-68Gg6mc06Hc_gTsltQXpjw/edit?usp=sharing)*<br>
         *[realestate.com.au_SOLD_Calamvale.csv](https://docs.google.com/spreadsheets/d/1KRQfJ4rNB-3YFZOW1glmdcAWQ0d7PBmtGiZGp1lA_RY/edit?usp=sharing)*<br>
         *…*<br>
         *[realestate.com.au_SOLD_Wishart.csv](https://docs.google.com/spreadsheets/d/1mbTzczhl0dZ9_6XDZ8KXy4O219DF9tDMFNwb0Pn-snk/edit?usp=sharing)*<br>

## Recommendation

Through analyzing the number of sold houses and the median prices of 3 and 4 bedrooms across 10 suburbs between 2017-2020, the project provided answers to the 5 questions listed in the Project Synopsis section, and also recommended a list of suburbs for the couple to consider for their next house purchase.

**Note**: The recommendation shown above is only based on 
a preliminary inference by observing the trend with limited sets of data, and will need to examine further factors (such as the number of houses on sale, the average days on the market, the council development plan, investment policies etc.) to make a proper conclusion.
   

