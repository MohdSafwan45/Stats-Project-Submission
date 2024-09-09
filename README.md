*Question:-1

Data Handling-

=Question:-How would you handle missing values in a dataset? Describe at least two methods.
Answer:-
Dealing with missing value is important to avoid compromising the quality of the analysis that is being made on the data. Here are two common methods:Here are two common methods: 
 
a) Imputation 
 Imputation is the process of having missing values replaced with values that are most probably generated from the existent data. This method prove useful when it comes to keeping the structure and size of this particular dataset in check. 
 Mean/Median Imputation: For numerical data one can fill missing values with mean value of that particular column or with the median value of that column. When the distribution is normal or close to normal the mean is used while in skewed distributions the median is used if the affected is less due to the outliers. 
 
 Example: When there are missing ages in the given data missing value imputation where missing values are replaced with average keeps the overall distribution intact. 
 Mode Imputation: If variables are categorical, with a lot of cases missing data can be replaced by the Most Frequent Value (mode). This approach is straightforward; however, this can lead to the biases in case the missing data is missing not at random. 
 Example: In a dataset with missing values in a “Region” column then imputing these with the most frequent region in the data retains the balance of categories. 

 b) Deletion 
 Deletion simply means eradicating data that have some missing values. This method is easy and can be a little problematic since it may expose the researcher to bias and can result to loss of data. 
 Listwise Deletion: Blank entries of the rows are eliminated. s applicable if the missing data are negligible or if they are distributed in a random manner. 
 Example: When dealing with a survey and there are say only a few cells which are missing in the entire dataset, then it could be safely assumed that its removal will not affect analysis much. 
 Column Deletion: Missing values can be omitted for entire columns while if the columns contain several missing values, they may be omitted especially if they are not important in the analysis. 
 Example: For example, if in ‘Secondary Contact’ column data 80% are missing then that column may be dropped to avoid any influence on the models. 
 Each of the two methods has its strengths and it is geared by the degree and type of missing data and their impact on a study.

=Question:-Explain why it might be necessary to convert data types before performing an analysis.
Answer:-
Type conversion is one of the important data preprocessing steps that aim at making sure that data is properly processed and understood. Here’s why it’s important: 
a) Correct Numerical Operations 
 Data also contain numbers in text format which makes it impossible to perform any mathematical or statistical calculations on them. To perform a mathematical operation on them it is inevitable to force them into working numeric types, integers or floats, respectively. 
Example: A “Sales” column present in a spreadsheet in the form of text data must further be converted into a numeric data type in order to compute the total sales or the mean, standard deviation, variance or any other statistical measure of dispersion. 

 b) Categorical Data Handling 
 While developing machine learning algorithms and statistical models, categorical data must be in a numerical form. This can be done using methods such as label encoding or one hot encoding methods etc. 
Label Encoding: Turns categories into integers to be used when analyzing ordinal data where there is some sort of natural ranking. 
Example: In ‘Customer Rating,’ if the options are High, medium and low in a tabular format, encoding these charges as 1, 2 and 3 respectively enable the models to read the ordinal data. 
One-Hot Encoding: Generates dummy variables for each category to guard against model’s tendency to assign ordinal relations. 
Example: In the case of categorical data in a “Region” column with options; “North,” “South,” and “East”, it is possible to craft binary columns for each in order for the model to process this data correctly. 

c) Datetime Conversion 
 Dates should be converted to datetime format in order to provided efficient time-based analysis, such as trends and dates. 
 Example: A column labeled ‘Purchase Date’ means that date strings must be parsed to datetime format for time series data handling and extraction of date features such as month or year. 

 d) Memory Optimization 
This also shows that the application of proper data type can also enhance memory efficiency. For example, the transformation of data type from float64 to float32 could minimize data usage while little affects to the accurate degree. 
In conclusion, the data type conversion provides the guarantee of proper processing and analysis of the data; appropriate calculations are made hence enhancing the performance of the analysis.

Statistical Analysis-

=Question:-
What is a T-test, and in what scenarios would you use it? Provide an example based on sales data.
Answer:
The other method is a T-test which is used when comparing the means of two groups to avoid a significant difference. Its application is most appropriate where you are working with small samples, and it assumed that the data is normally distributed. 
 
 Types of T-tests: 
 Independent T-test: The test is used to compare the means of two independent groups in order to determine whether the difference between the means is significant. It is applied if you have two different groups and if you want to determine whether there is significant difference in their means. 
 Example: Let’s assume one has to analyze the difference in the average sales performance of two different sales teams, namely Team A and Team B, in order to know if the average sales figures of Team A differ significantly from that of Team B. In order to perform this test, an independent samples T-test can be conducted. In the equation above, 05, it indicates a statistically significant difference of the mean sales of the two teams. 
 
Paired T-test: Refers to making a comparison of the arithmetic mean of one related group with that of another related group for example before and after some treatment has been carried out. It is applied when samples are related, or matched, in some way, or in matched pairs samples. 
 Example: Independent variables In case you have sales data of individual sales team before and after the intervention then the use of paired T-test will help in determining whether the mean sales have significantly changed after the new strategy has been adopted. 
 
When to Use a T-test:When to Use a T-test: 
 To compare means between the two groupings it is important to follow these steps. 
 Mor to the point, when data is normally distributed. 
 With small sample sizes

=Question:-
Describe the Chi-square test for independence and explain when it should be used. How would you apply it to test the relationship between shipping mode and customer segment?
Answer:
The Chi-square test for independence is applicable where one wishes to settled whether or not two variables are related in a population. It is a statistical method which compares the actual occurrence of the variables in the cross tabulation with the expected occurrence on the basis of the independence of the variables. 
 
 When to Use: 
 For testing whether or not there is an association between two discrete variables. 
 When you wish to know about the cause-effect or in simple terms if the occurrence of one variable is in any way reliant on the occurrence of the other. 
 Steps to Apply the Chi-square Test:Steps to Apply the Chi-square Test: 
 Construct a Contingency Table: Devise a table below where one can display the total number of times each of the categories for the two variables occurs. For example, a table with the frequency of the shipping modes such as Standard, Expedited, Same-Day with the type of customers using the services; Retail, Corporate, Small Business. 
 
 Calculate Expected Frequencies: Since All The Variable Are Assumed To Be Independent Of One Another Calculate The Expected Frequencies Of Each Cell In The Table.This Is Done Using The Formula
 ( 
 Row total 
 × 
 Column total 
 ) 
 Grand total 
 Expected frequency= 
 Grand total 
 (Row total×Column total) 
 ​ 
 where 
 𝑂 
 O is the observed frequency and 
 𝐸 
 Where E is the expected frequency of an event we want to measure, often observed in decision-making processes… 
  Determine the p-value: Now go to the Chi-square distribution table and find the p-value against the Chi-square statistic and degrees of freedom. 
  Interpret Results: Should the p-value be less than the significance level (for instance, if the level of significance is 0. 05), then reject the null hypothesis which suggests that there is a significant relationship between the shipping mode and the customer segment. 
 Example: 
 I will use the contingency table to determine whether the choice of the shipping mode is dependent on the customer segment In this table, distinctions of the shipping mode are made on the rows while the distinction of the customer segment is on the columns. Use the Chi-square test to determine the likelihood of difference on the observed frequency of the mode of shipping in the different customer segments. Such an outcome would mean that some customers prefer using specific shipping modes.

Univariate and Bivariate Analysis:

=Question:-What is univariate analysis, and what are its key purposes?
Answer:-
Descriptive analysis is a family of statistical approaches which includes analyzing one variable only at a given time. The primary approach is again used to present an overview of the data and major characteristics associated with this variable. Such analysis is descriptive in nature and is instrumental in getting an overview of factors under consideration without reference to other factors. 
 
 Key Purposes of Univariate Analysis:Key Purposes of Univariate Analysis: 
 Distribution Examination: It determines the degree of variation in the values of the data or how the values are spread or distributed. Histograms which is also refereed to as frequency tables allows you to determine the nature of the distribution whether it is normal, skewed, or bimodal. For instance, the distribution of age of the employees can be displayed by a histogram and this determines whether most of the employees are within a given age bracket or not. 
Central Tendency Measurement: This include use of measures of central tendency which include the mean median and mode. These statistics give information to about the central tendencies of the variable that is, the most frequent or usual values. For example, use of the mean in establishing the average number of employees’ salary in an organization assists in determining the tendency of earnings. 
 Variability Assessment: Range is one of the measures of variability which offers information on the degree to which the values of a variable need to deviate from theaverage in order to correspond with another variable. For example when one is working in a database of monthly temperatures then the standard deviation is used to show how much the temperatures differ from the average. 
 Outlier Detection: One such purpose is about identifying outliers, that is values which are far from the residual observations. Often an outlier points at an error, or simply it portrays an abnormality. For example, outliers like, a set of exam scores can be analyzed whether they contain very high or very low values that need further assessment. 
 Descriptive statistics reveals information on all the individual variables before moving to the next level of analysis which is the multivariate analyses.

=Question:-Explain the difference between univariate and bivariate analysis. Provide an example of each.
Answer:-
Univariate Analysis 
 Univariate analysis analyses and describes one variableon the basis of its own characteristics and features. They give an opportunity to describe the distribution, central and dispersion tendencies of the variable. This analysis is rather important in order to learn the parameters of every single variable on its own. . 
  Example: Let us discuss an example of the variable “Monthly Sales Revenue” of a retail firm. Using the univariate analysis, one would be required to calculate the mean, mid-point and standard deviation of the sales revenue. A line plot of such figures showing the amount of sales made every month will display trends in sales revealing if the sales are rising, falling, or constant. 
 
Bivariate Analysis 
 On the other hand, there is uni-variate where only one variable is analyzed to see if there is a link between the given variable and the dependent variable. It is used in analyzing the relationship of two or more variables in order to establish whether they are related or not. 
 Example: If we wanted to indentify the correlation between ‘Advertising Spend’ and ‘Sales Revenue’ then it would be a bivariate analysis complete with a Pearson coefficient. If more money were spent on advertising, then the resultant scatter plot of the advertising spend on the x-axis and the sales revenue on the y-axis can point out if the revenues have increased afresh. Furthermore, the measures of relationship are carried out by determining the correlation coefficient, which gives the extent and direction of the association. 
 To sum up, univariate method deals with the description of only one variable at a time while the bivariate method deals with characteristics of two variables which help to understand the nature of association in between them better.

Data Visualization:

=Question:-What are the benefits of using a correlation matrix in data analysis? How would you interpret the results?
Answer:
A correlation matrix is a table used in analyzing correlator data in order to reveal the probability coefficients of the given data set of variance. This tool is invaluable in data analysis for several reasons:This tool is invaluable in data analysis for several reasons: 
Benefits: 
 Identifies Relationships: The matrix shows the magnitude and orientation of the connection of the variables. Correlation coefficients vary from -1 to +1 while 1 shows strong positive relation, -1 represent strong negative relation and 0 represent zero relation. This assists in determining the relationships between variables In other words In this assists in establishing how two or more variables are connected. 
 Example: If the number of the correlation coefficient between the advertise expenses and the selling income is 0. Consequently, it points out to a significant positive correlation, which implies that the more money an organisation spends on advertising; the more sales they record. 
 
Simplifies Data Exploration: Managing more complicated and intricate relationships by consolidating them in a single matrix makes viewing data interaction easier. This is very useful especially while working with large numbers of variables so that the analyst can easily detect the high correlation variables. 
 
Aids Feature Selection: Whereas in the case of selecting the features, correlation is helpful in the context of predictive modeling. High correlation means the features are redundant and this makes it possible to eliminate all but one feature responsible for multicollinearity. 
Example: If two variables, let say, price and discount are dependent on each other then correlation coefficient ‘r’ between the two features shall be 0. 9, one might be excluded to eliminate complementarity as a confounding factor in the contexts of the various predictive modeling. 
 Interpretation: 

Positive Correlation: It is the contingency that explains that variables either both increase or both decrease at the same time. If the coefficient is high and for one variable positive, then this means that if the first variable rises, so does the second one. 
 
Negative Correlation: There is inverted movement of variables. A high negative coefficient indicates that if one variable increases the other variable decreases. 

Near Zero Correlation: It can also be noted that little to no linearity is present between the two variables. 
 Such relations are useful in forming theories, measuring experiments, and constructing theories and proposals.

=Question:-How would you plot sales trends over time using a dataset? Describe the steps and tools you would use.
Answer:
The line graph is valuable for tracking the sales trends over time or depicting his or her sales performance and detect patterns such as the seasonal fluctuations. Here’s a step-by-step approach: 
Steps: 
 Prepare the Data: 
 
 Load Data: Using a library such as Pandas, read the dataset which comprises of sales information. 
 Format Dates: Make sure that the date column is in the datetime type by using the pd. to_datetime() so as to allow time based plotting. 
 Aggregate Sales: After data collection, sales information may be summarized at different levels based on its level of details required such as daily, monthly or even years. For example, use df. groupby(df['Date']. dt. to_period('M')). sum() for monthly aggregation. 
 Choose the Visualization Tool: 
 
 Matplotlib: An all-around library for plotting graphs. Use plt. plot() in order to get the line plots. 
 Seaborn: Offers additional graphs and an improved method of the treatment of data. Use sns. lineplot() for better aesthetics. 
 Plotly: An interactive plotting library which can make an interactive timeseries plot using plotly. graph_objects. 
 Create the Plot: 
 
 Plot Data: Line plot it in order to display the sales to highlight a time period. For example with Matplotlib, plt. The first one is generated by using the command plot(df[‘Date’], df[‘Sales’]) to facilitate the creation of a simple time series plot. 
 Customize Plot: Take time and add the label, title and legend of the plot in order to make the plot comprehensible. For example, plt. xlabel('Date'), plt. ylabel('Sales'), and plt. title('Sales Trends Over Time'). 
 Analyze Trends: 
 
 Seasonality: Search for cycles that follow predictable trends with a certain frequency, like how many customers are likely to be made during festive season. 
 Trends: Recognise general trends, for instance a long term trend that shows a rising or declining sales trend. 
 Anomalies: Look out for any variances in the sales figure; peaks and troughs. 
 In this way, depending on the steps given above, it is possible to enhance the sale trends in the right way which helps to get a vision about the sales performance over the time.

Sales and Profit Analysis:

=Question:How can you identify top-performing product categories based on total sales and profit? Describe the process.
Answer:
 The most important step in the identification of the beneficial product categories is the assessment of the sales and profit figures that show the categories, which types of products bring the most significant amount of income and profit. Here's a structured approach to achieve this:Here's a structured approach to achieve this: 
 
 Process: 
 Data Collection: 
 
 Load Data: Read your data into your program with Pandas and show it in a DataFrame format. Make sure that it has columns for product categories, sales and profit. 
 Example: df = pd. import_csv(‘sales_data. csv’. 
 Group and Aggregate Data: 
 
 Group Data: Time series can be grouped by product category as shown in the time series code below using df. groupby('Product_Category'). 
 Aggregate Metrics: To do this, use the aggregation functions to determine the total sale and total profit under each category. For instance: 
 Example Code: 
 category_summary = df. groupby('Product_Category'). agg({'Sales': 'sum', 'Profit': 'sum'}) 
 This will generate a new DataFrame that will give a summery of total sales and profit by each product category. 
 Sort and Rank: 
 
 Sort Data: The aggregated data is to be sorted by total sales & profit in the descending order to find out the most successful categories. For example: 
 Example Code: 
 top_categories = category_summary. sort_values(by=['Sales', 'Profit'], ascending=False) 
 This will help in listing categories that are most profitable in bearing the costs in listing as well as the cost of sales. 
 Visualize Results: 
 
 Create Visuals: Bar charts to be effectively used in presenting the data regarding the best performing categories. For example, use Matplotlib or Seaborn:For example, use Matplotlib or Seaborn: 
 Example Code: 
 import seaborn as sns 
 sns. barplot(x=top_categories. index, y='Sales', data=top_categories) 
 This makes it easier to identify the leading categories on the basis of the visual representation given above. 
 Analysis and Insights: 
 
 Evaluate: This will help in identifying the specific reasons as to why the given categories have been performing well. Some of these include the price strategies, product positioning and the customer’s preferences. 
 Following these steps you can define and analyze the product categories, which impact on the sales and/or profit.

=Question:Explain how you would analyze seasonal sales trends using historical sales data
Answer:
Historical sales analysis for seasonal sales include looking at patterns and trends in sales that are common with given period of the year. Here’s a detailed approach to perform this analysis:Here’s a detailed approach to perform this analysis: 
 
 Process: 
 Data Preparation: 
 
 Load and Clean Data: Now, let’s start with importing the historical sales dataset into an pandas dateframe. Make sure that the date column is at the right format of datetime using the method pd. to_datetime(). 
 Example: target_h[‘Date’] = pd. to_datetime(target_h[‘Date’]). 
 Aggregate Sales Data: 
 
 Group Data: This is to enable trend analysis through grouping and summing of the sales data by the right time intervals like the month or quarter. For instance, to aggregate monthly sales:For instance, to aggregate monthly sales: 
 Example Code: 
 monthly_sales = df. groupby(df['Date']. dt. to_period('M')). agg({'Sales': 'sum'}) 
 
 It is useful in preventing every day high and low abnormal movements from skewing the results while focusing on mid-term trends. 
 Decompose Time Series: 
 
 Decomposition: Time series decomposition has to be done to be able to split the data in the time series into trend, seasonal, and residuals. This can be done using libraries like statsmodels:This can be done using libraries like statsmodels: 
 Example Code: 
 from statsmodels. tsa. seasonal import seasonal_decompose 
 decomposition = seasonal_decompose(monthly_sales['Sales'], model='additive') 
 This decomposition helps to Pull out features such as trend and seasonality hidden in the system. 
 Plot and Visualize: 
 
 Create Visuals: It is recommended to plot the sales functions on lines to focus on the relationships with the time series components. For example: 
 Example Code: 
 
 plt. figure(figsize=(10, 6)) 
 
 plt. ax. plot(moment. monthly_sales. index. to_timestamp(), monthly_sales. Sales, label= ‘Monthly Sales’) 
 
 plt. title('Monthly Sales Trends') 
 
 plt. xlabel('Date') 
 
 plt. ylabel('Sales') 
 
 plt. legend() 
 
 plt. show() 
 
 This plays a big role in finding the highest and the lowest sale period, average sale period or even a general trend of the business. 
 Analyze and Adjust Strategy: 
 
 Evaluate Patterns: (It will involve identifying trends that are cyclical, for instance, sales tend to be high during specific period such as holidays or periods when companies offer certain promotions). 
 Strategy Adjustment: Apply these findings for the purpose of sales prediction as well as for fine-tuning the marketing, stocking and selling activities. 
 Following such a process, you will be in a position to analyze seasonal fluctuations meaning you will be able to make good decisions on sales history.

Grouped Statistics:

=Question:Why is it important to calculate grouped statistics for key variables? Provide an example using regional sales data.
Answer:

Understanding Segmented Performance: Preliminary aggregate statistics enable the analyst to focus in on various segments or categories of performance. For example, calculating sales and profit statistic by region assists in determining the contribution of each region on the overall business performance. Cohesive this partitions designate where strategy is effective and which may require a strategic. 
 
 Informed Decision-Making: Thus, the studying of grouped statistics helps in making a decision in businesses. For instance, if some areas produce higher sales and profit margins, then few of the resources which include the marketing budgets or inventories can be re-instituted in the said areas in order to increase optimal utilization. On the other hand, it allows low-performance areas to be explored in terms of possible problems that may exist like overcrowding of the market or some issues with distribution. 
 
 Targeted Strategy Development: Statistics that are grouped help in the formulation of appropriate strategies. It also reveals the degree of sales and profitability by a region, which helps the companies to base their strategy on region-by-region analysis. These might like targeting clients in a particular region through the appropriate marketing communication or changing offer to match the needs of a certain area. 
 
 Resource Optimization: Grouping of values in a tabular form assists in proper allocation of resources based on a set of statistical measures. For instance, it possible for one region to be performing better than others, and hence it could be wise to invest more in that area so that to leverage on the performance. This helps in making appropriate investments on whatever is most useful in delivery of the services. 
 
 Example Using Regional Sales Data:Example Using Regional Sales Data: 
 
 Let us recall an example of a retail company that has to assess the results of its sales activity in different regions. To identify the top-performing regions, follow these steps:To identify the top-performing regions, follow these steps: 
 
 Data Preparation: Load and preprocess the data, which contain variables; Region, Sales, and Profit. 
 
 Group Data: Calculate aggregate data of Sales and Profit by regions using function of Pandas: 
 
 Example Code: 
 regional_summary = df. groupby('Region'). agg({'Sales': 'sum', 'Profit': 'sum'}) 
 
 Analyze Metrics: In this type of report comparison of total sales and profits of each region is made for analyzing the regions performance. For example: 
 
 Example Code: 
 regional_summary['Average_Sales_Per_Store'] = df. groupby('Region')['Sales']. mean() 
 
 Sort and Interpret: Rank the results obtained in order to ascertain the most productive regions. 
 
 Example Code: 
 top_regions = regional_summary. sort_values(by='Sales', ascending=False) 
 
 Visualize: 2 charts showing the sale and profit by the region. For instance: 
 
 Example Code: 
 import matplotlib. pyplot as plt 
 
 plt. figure(figsize=(10, 6)) 
 
 plt. bar(top_regions. index, top_regions['Sales']) 
 
 plt. xlabel('Region') 
 
 plt. ylabel('Total Sales') 
 
 plt. title('Total Sales by Region') 
 
 plt. show() 
 














Question:-2
However, in the data analysis procedure, the phase of loading and inspecting the dataset and analyzing them creates a significant aspect in DA technique. The following is a breakdown of the code and what the code is for, and this is a step by step guide on how to explore a dataset using python.

Step 1: Required Libraries H2 and Hikari-cp are imported.
Code:
import pandas as pd

import numpy as np

import matplotlib. pyplot as plt

import seaborn as sns

%matplotlib inline

Explanation:
pandas: This library is mandatory for operations involving structured data, particularly in the form of tables: it helps to load, process and analyze datasets.
numpy: Combined with pandas, it performs other basic operations such as mathematical computations on the data.
matplotlib. pyplot: This is for the purposes of drawing figures such as charts and graphs which make it easier to understand the data patterns.
seaborn: A powerful tool, which is destined to become one of the most effective solutions in the creation of beautiful and useful plots.
%matplotlib inline: They make sure that all the created visualizations are displayed in the notebook space which is helpful while working in frameworks such as Jupyter.
Marks Allocation: 4/20 (Importing of libraries is very important in order to make the data analysis tools to run effectively).

Step 2: As for the pattern, the loading of the dataset demonstrates the complexities in creating models for machine learning.
Code:

df = pd. read_csv(‘ your_dataset.csv’)

Explanation:
pd. read_csv() takes data from a CSV file and loads the data into pandas data frame which is denote by ‘df’. The argument ‘your_dataset. csv’ should be replaced with the path or with the name of the file with the dataset.
This function just builds the datasets within the CSV data in the shape of records as rows and the features as column way.
Importance:
Charging the dataset correctly is the primary and a onerous step since it makes the data available for analysis.
So let’s use DataFrame for data manipulation because it is much easier to work with, organize, and clean it up.

Step 3: Selecting the Structure for the First Few Rows 
Code:

 print("First 5 rows of the dataset:This may be in the form of [‘the URL of the article itself,’ ‘<www. bufadora. com/ARTICLE-URL HERE>’]. 
 print(df. head()) 
 
 Explanation: 
 df. head() shows the first 5 rows of the dataset at once, although, one has an option of showing an n number of rows by inputting the number inside the head() bracket (e. g. df. head(10) to display first ten rows). 
 Importance: 
 Checking an overview of data allows you to get an idea of the organization of information on the selection of columns, the types of data, the identification of outliers. 
 You have a clear perceivable vision of how the dataset is arranged, which guide the next steps you want to take in the analysis. 
 
 Step 4: Summary Statistics 
 
 print("\nSummary Statistics:")
 
 print(df. describe()) 
 
 Explanation: 
 -df. The function describe() offers basic statistics summary of the numerical variables in the data frame. This includes: 
 
 -Count: Number of values in attribute that is not null. 
 
 -Mean: The mean of the data set: Arithmetical mean of the data points. 
 
 -Standard Deviation (std): Coalition of the data points. 
 
 -Min, Max: Range of data. 
 
 -Percentiles (25%, 50%, 75%): In addition, explain the nature of the data and the distribution of data. 
 
 Importance: 
 -Descriptive measurements provide a snapshot of the data and allows for the understanding of the distribution, the central tendency and variability of the data. 
 -These metrics allow to discover alerting anomalies, trends and other patterns in a data set at the very initial stage of analysis 


Step 5: Handling for missing Observations 
 print("\nMissing Values in the Dataset:This is why it is crucial to comprehend the text as institutionally, it is most apparent in fixating on its precise form and grammar, as <air filled>institutional reading||Here I agree with you, Read this [because]: prove its importance and usefulness or for some other reason as it is apparent, institutionally, mostly in paying attention to the text’s form and grammar, <air filled>institutional reading. 
 
 print(df. isnull(). sum()) 
 
 Explanation: 
 -df. isnull(). sum() also performs the detection of missing values by column and gives the count of null ‘NaN’ values in every column. 
 -These missing data can distort the analysis and so it is very important to address them right from the beginning. 
 
 Importance: 
 -Missing values detection is an initial important step before getting into further analysis or building any model. 
 -It allows you identify a way to proceed with the missing values for instance imputing, deleting or even ignoring depending on the situation.
