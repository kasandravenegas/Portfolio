# Business Analyst

#### Technical Skills: Python, Tableau, R, Excel, SQL, PowerBI, Pandas, Microsoft Office Suite

## Education
- B.S., Business Analytics | University of California, Riverside (June 2025)

## AirBnB Real Estate Market Analysis
<embed src="assets/img/AirBnB%20Full%20Project.pdf" width="600" height="500" alt="pdf">

<p>If the PDF does not display, you can download it directly <a href="assets/img/AirBnB%20Full%20Project.pdf">here</a>.</p>

#### Objectives
- Analyze the average price per bedroom and price per zipcode for a real estate market
- Examine the distribution of bedroom counts in the market
- Visualize the revenue trends over time for the real estate market

#### Methodologies
- Plotted average price per bedroom and price by zipcode on charts to identify market trends.
- Analyzed the distinct count of bedroom listings to understand the distribution of property sizes.
- Charted the revenue over time to identify growth patterns in the real estate market. 

#### Key Insights
- The average price per bedroom is $188.8, indicating a relatively high-end real estate market.
- Prices vary significantly by zip code, with the most expensive areas costing over $200 per zipcode.
- The market has a diverse mix of property sizes, with a concentration of 1-4 bedroom listings.
- Revenue has steadily increased over the years, showing a growing and thriving real estate market.

## Exploratory Data Analysis on Company Layoffs
<embed src="assets/img/Exploratory%20Data%20Analysis%20on%20Company%20Layoffs%20(2).pdf" width="600" height="500" alt="pdf">

<p>If the PDF does not display, you can download it directly <a href="assets/img/Exploratory%20Data%20Analysis%20on%20Company%20Layoffs%20(2).pdf">here</a>.</p>

### Objectives
The main objective of this analysis is to understand the impact and trends of layoffs across companies, industries, and regions through key statistics like maximum layoffs and percentage impact. 

#### Methodologies & Key Queries

#### 1. Maximum Layoff Metrics
- This query calculates the maximum number of total layoffs and the highest percentage of layoffs.
- (_SELECT MAX(total_laid_off) AS max_total_laid_off, MAX(percentage_laid_off) AS max_percentage_laid_off
FROM layoffs_staging2;_)

#### 2. Company-wise Layoff Totals
- This query aggregates total layoffs by each company, displaying the companies with the most layoffs.
- (_SELECT company, SUM(total_laid_off) AS total_layoffs
FROM layoffs_staging2
GROUP BY company
ORDER BY total_layoffs DESC;_)

#### 3. Data Time Range
- This query identifies the earliest and latest dates in the layoff data, defining the time period covered by the dataset.
- (_SELECT MIN(date) AS start_date, MAX(date) AS end_date
FROM layoffs_staging2;_)

#### 4. Country-wise Layoff Totals
- This query summarizes the total layoffs by country, showing which countries experienced the most layoffs.
- (_SELECT country, SUM(total_laid_off) AS total_layoffs
FROM layoffs_staging2
GROUP BY country
ORDER BY total_layoffs DESC;_)

#### Key Insights
- The maximum total number of layoffs recorded in a single entry is 12000.0
- The highest percentage of workforce layoffs in an entry is 1.0. This indicates significant impacts on specific companies during layoffs.
- The company with the most layoffs is Amazon, with a total of 18150.0 layoffs. This highlights Amazon as a significant player in overall layoff numbers during the observed period.
- The dataset covers layoff data from 2020-03-11 to 2023-03-06, encompassing critical periods that align with global economic events, including the COVID-19 pandemic.
- The United States records the highest total layoffs, emphasizing its significant role in contributing to the overall layoff numbers.

## Excel Bike Analysis
<embed src="assets/img/Excel%20Pivot-Dashboard.pdf" width="600" height="500" alt="pdf">

<p>If the PDF does not display, you can download it directly <a href="assets/img/Excel%20Pivot-Dashboard.pdf">here</a>.</p>

#### Objectives
- Analyze the demographic factors that influence the decision to purchase a bike.
- Identify patterns based on income, age, marital status, and other factors related to bike purchases.
- Segment the customer base by key characteristics (e.g., region, education, occupation) to identify target audiences.

#### Methodologies & Key Formulas

#### 1. Data Segmentation and Conditional Analysis
- COUNTIFS: Count bike purchases by region and marital status.
- (_=COUNTIFS(F2:F1000, "Pacific", E2:E1000, "Yes")_)
- SUMIFS: Sum total income of married individuals who bought bike
- (_=SUMIFS(D2:D1000, E2:E1000, "Yes", B2:B1000, "M")_)

#### 2. Lookup & Referencing
- XLOOKUP: Lookup income by customer ID.
- (_=XLOOKUP(A2, IDRange, IncomeRange)_)
- INDEX-MATCH: Retrieve income using a flexible lookup
- (_=INDEX(D2:D1000, MATCH(A2, A2:A1000, 0))_)

#### 3. Pivot Table Extraction
- GETPIVOTDATA: Extract total income for bike purchasers by region.
- (_=GETPIVOTDATA("Sum of Income", PivotTable!$A$3, "Region", "Pacific")_)

#### 4. Dynamic Analysis
- OFFSET: Calculate cumulative income for N entries.
- (_=SUM(OFFSET(D2, 0, 0, N))_)

#### Key Insights
- Higher income individuals are more likely to purchase bikes, with a notable increase in bike ownership among those earning over $50,000.
 - Single individuals without children show a higher propensity for bike purchases compared to married individuals with children.
- Professionals and clerical workers have a greater tendency to buy bikes, likely due to shorter commute needs and lifestyle preferences.
 - Those with shorter commutes (0-1 miles) are more likely to purchase bikes, highlighting convenience as a key factor.

## PowerBI Project
<embed src="assets/img/Power%20BI%20Project%20(2).pdf" width="600" height="500" alt="pdf">

<p>If the PDF does not display, you can download it directly <a href="assets/img/Power%20BI%20Project%20(2).pdf">here</a>.</p>
#### Objectives
- Analyze the demographics, salaries, and job satisfaction of data professionals.
- Identify salary trends by job title and programming language preferences.
- Explore geographic distribution and work-life balance satisfaction.

#### Methodologies

#### 1. Data Preparation: 
- Import and clean the dataset in Power BI.

#### 2. Data Modeling:
- Create relationships between tables for analysis, linking job titles, geographic locations, and salary information.
- Use calculated columns and measures to compute key statistics such as average salary, job satisfaction, and work-life balance ratings.

#### 3. Visualizations:
- Use bar charts, pie charts, and gauges to analyze salary, job satisfaction, and geographic distribution.

#### 4. Dashboard:
- Use slicers to allow users to explore the dataset based on various parameters, such as age, job title, and region.

#### Key Insights
- Data Scientists and Engineers have the highest average salaries.
- Python is the most popular programming language.
- Most respondents are from the US, India, and the UK.
- Work-life balance is moderate (average 5.74/10).
- Breaking into the field is generally seen as neither too easy nor too difficult.
