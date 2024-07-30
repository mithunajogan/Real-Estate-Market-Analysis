# Real-estate-market-analysis
# Data Preprocessing
The initial stage involves cleaning and preparing the data for real estate analysis, including handling missing values, correcting inconsistencies, and transforming data types if necessary. I cleaned and preprocesed the customers and property tables, ensure column names are in order and that missing values appear correctly, and applied any column data type changes I see fit. Finally,I combined the properties and customers tables into one unified real estate dataset using the shared customer_id column. I consolidated inconsistencies or missing values to perform the following analysis and obtain the correct results.

Properties and Customers
I reviewed the list and preprocessed and cleaned both datasets accordingly.

Descriptive Statistics: I started the analysis with descriptive statistics of the data and checked for any missing values.

Datatypes: I evaluated the datatypes of the columns and decided whether some of the datatypes needed to be changed.

Column Names: I checked if there were any issues with the column names and renamed them if necessary.

Categorical to Numerical: I changed categorical values to numerical when possible and needed.

Case: If there were inconsistencies with capital and lowercase letters, I unified them using the lowercase convention.

Missing Values: I ensured that missing values were correctly indicated.

Date Variables: I made sure to handle and transform the date variables correctly.

Preliminary Checks

Visually Inspect the Datasets: I visually inspected the two datasets and decided which variable to merge. Since both datasets shared only one column, I opted for the customer ID column.

Initial Merge Attempt: I leveraged pandas' functionality to combine the two tables without initial preprocessing. I considered what kind of join would make sense in the context of the given problem.

Resolving Merge Issues: When the initial attempt to merge the data did not yield the correct DataFrame, I examined and preprocessed the data further.

# Descriptive Statistics
Now that I had successfully merged the two datasets, I turned my attention to the next part of the analysis: descriptive statistics. I conducted a comprehensive statistical analysis to understand the distribution of the key variables.

I examined the main characteristics of each variable, specifically the numerical ones.

I analyzed the sales and overall performance by building type.

I also assessed the sales and overall performance by country and state.

# Breakdown by Building
First, I focused on the buildings' variable and their different types. I examined the totals and averages breakdown by building type.

I started by examining how many building types there were in the dataset.

I selected columns of interest to examine the totals by building type. I made a list with those variables, including building as the index variable. The columns of interest were sold and mortgage.

I found the total number of sold properties and how many of them had mortgages per building type.

I selected columns of interest to examine the averages by building type, considering that they might not be the exact columns I used for the totals. The columns of interest were area, price, and deal satisfaction.

I determined the average values of area, price, and deal satisfaction per building type.

# Breakdown by Country

On the country level, I performed the same analysis as I did for the building types by choosing columns of interest and using summary statistics for the totals and averages. I noted that the breakdown of calculations by country gave me the frequency distribution by country.

# Breakdown by State

I determined the frequency distribution by state, as I did for the countries table. In addition, I created a table containing the relative frequency and the cumulative frequency by state.

# Data Analysis
Now that I had successfully merged the two datasets and completed the descriptive statistics, which was a vital part of the project, it was time to focus on the analysis of key variables.

This phase included a more in-depth analysis of the data to uncover trends, correlations, and hidden insights. I started by analyzing the customers' age (and age intervals) and performed the same analysis for the properties' prices. Ultimately, I explored the relationship between age and price to gain deeper insights.

# Analyzing Age

Calculate Age at the Time of Purchase: 
The first step of my analysis was determining the age of customers at the time of sale. Since there wasn't such a variable in the data, I worked out the customers' ages from the information given in the data.

Create Age Interval Categories:
After calculating the customers' ages, I created age intervals to evaluate group behavior. I separated the ages into 10 intervals of equal length, or I used the following intervals:

19.0,25.0, (25.0, 31.0], (31.0, 36.0], (36.0, 42.0], (42.0, 48.0], (48.0, 54.0], (54.0, 59.0], (59.0, 65.0], (65.0, 71.0], (71.0, 76.0].

Break Down by Age Intervals: Finally, using summary statistics, I determined how many properties had been sold by age intervals.

# Analyzing Properties

To analyze the properties, I performed similar steps to the age analysis. I created 10 bins for the price intervals to answer the quiz questions successfully. However, I kept in mind that the correct number of bins might vary in real-world situations.

# Relationship between Properties and Age

To conclude this part of the data analysis project, I examined the relationship between the properties and the age variable. I discovered the covariance and correlation between the two variables.

# Data Visualization

The final part of the project was all about data visualization. Here is where all of my hard work paid off! I ensured that I had cleaned and preprocessed the data and completed all the descriptive statistics and data analysis tasks, as they served me well in this part. I was now ready to answer the client's following critical questions regarding the data:

What is the average deal satisfaction for each country? How does it look by state?

What is the monthly revenue of the company?

How many apartments are sold in each state?

What is the age distribution for customers? (I used the same age intervals or number of bins from the data analysis stage.)

What are the yearly sales for each building?

To answer these questions, I created the following visualizations:

Deal Satisfaction by Country:
I created a bar chart or a heat map that represented the average deal satisfaction by country.

Revenue Graph: 
I created a time-series graph showing the total revenue over time.

Apartments Sold by State:
I created a Pareto chart, in which the bar showed the absolute frequency of buildings sold by state, and the line chart displayed the cumulative frequency.

Age Distribution Histogram:
I created a histogram displaying the age distribution of customers.

Sales per Year by Building Type:
I created a stacked bar graph or a line graph showing the yearly sales for each building type.







