git commit --allow-empty -m "Trigger fresh deployment"
git push


# Business Analyst

#### Technical Skills: Python, Tableau, R, Excel, SQL, PowerBI, Pandas, Microsoft Office Suite

## Education
- B.S., Business Analytics | University of California, Riverside (June 2025)

## Work Experience
**Project Assistant @ Campus Business Services (_August 2023 - Present_)**
- Streamlined fiscal year data reporting using advanced Excel formulas, leading to a 20% reduction in update time.
- Improved candidate fit by 20% and reduced time-to-hire by enhancing the student worker selection process with analytical - screening and structured interviews.
- Improved process adherence by 35% and reduced training time by standardizing operational efficiency through detailed SOP reports based on analysis of existing procedures.

**Peer Mentor @ Victor Valley College (_February 2023 - August 2023_)**
- Increased first-year student enrollment for orientation by 25% by assisting with copywriting email advertising campaigns focused on student outreach.
- Created and delivered PowerPoint decks showcasing the impact of social media campaigns on the School of Business's web presence
- Achieved a 25% increase in orientation sign-ups by optimizing email advertising campaigns with data-driven insights, demonstrating the power of targeted content and analytics.

**Marketing and Public Relations Assistant @ Victor Valley College (_May 2021 - February 2023_)**
- Streamlined fiscal year data reporting using advanced Excel formulas, leading to a 20% reduction in update time.
- Improved candidate fit by 20% and reduced time-to-hire by enhancing the student worker selection process with analytical - screening and structured interviews.
- Improved process adherence by 35% and reduced training time by standardizing operational efficiency through detailed SOP reports based on analysis of existing procedures.

### Projects
## AirBnB Real Estate Market Analysis

<embed src="assets/img/AirBnB Full Project.pdf" width="600" height="500" alt="pdf">

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

### Methodologies & Key Queries

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










