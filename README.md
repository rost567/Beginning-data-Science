We will use data published by the World Bank about population in countries.  

The process is:  
**PART 1**  
- Changing column headers, because those are values, not variable names.
- Using data about the average height in countries around the world. It comes from Kaggle.
- Manipulating the dataframe "height" to be tidy. Currently, multiple variables are stored in one column.
- Working with data about billboards in the 2000s.
- Manipulating the dataframe "billboard" into two dataframes that each store one observational unit.
- About average heights. What's the country with the tallest men? Defining two variables "country_tallest_men" as a string and "height_tallest_men".
- In which country is the difference of average heights between men and women largest?
- The Pearson's correlation value of average male and average female height.

**PART 2**  
Main topics: 
> - Matplotlib
> - Introduction to more advanced visualization tools

Now exploring data on college majors sourced from the American Community Survey 2010–2012 Public Use Microdata Sample. This dataset can be found at this [URL](https://raw.githubusercontent.com/fivethirtyeight/data/master/college-majors/recent-grads.csv)

- Plotting the basic information to get a sense of the dataset. "Rank" is the major’s rank by median earnings.
- Does the unemployment rate look proportional to the rank of the major? To see this, we will display the unemployment rate against the rank of the major.
- Does the salary look proportional to the rank of the major? For this we will display the median salary, the 25th and 75th percentiles against the rank of the major. We will plot three lines in the same plot.
- Displaying the number of low wage jobs against the rank of the Major.
- To see the relation between low wage jobs and the rank of the Major we will display the percentage of low wage jobs against the rank of the major, using Matplotlib to get a more precise plot. Extracting the rank, number of low wage jobs, and the number of employed from the data and putting each of them into their own series.
- Displaying the percentage of low wage jobs against the rank of the major.
- Now to get some information about the distribution of the data. Displaying the histogram for the median of the salary.
- Displaying the histogram for the ratio of employed with low wage with the variables 'df_wage', 'df_employed', previously extracted.
- Using subplot to display two figures.
> - The first figure is the histogram for the ratio of employed with low wage, like the previous one.
> - The second figure is the same histogram but with 30 equal-width bins.
- Making the previous plot pretty. Adding one title by subfigure. Using two different colors for each histogram. Adding x and y labels. Displaying a vertical grid in the first sub-figure, and a horizontal grid on the second one. Removing the edges around the plot.
- To see some isolated extreme values. In this part, we will try to identify and understand these outliers. Extracting a dataframe containing the rows with the 10 highest median salaries.
- From the Major with top 10 median salary, displaying the median, the 25th and 75th percentiles on a bar plot. Using the the attribute 'kind' in the pandas plot function.
- Also plotting the histogram for a specific category. Displaying the histogram of the median salary for the Major with category "Engineering"
- Let's see if we can infer the correlation between two factors using scatter plots. Displaying the median salary against the unemployment rate on a scatter plot.Using the the attribute 'kind' from the pandas plot function.
- Now analyzing and visualizing the categorical data. We want to count how many students there are per category. Extracting the different categories (column "Major_category") and displaying them on an horizontal bar plot. Summing up the number of students in each category (column "Total").
- we have to merge the smaller categories into a single group.  
> - First, separating the data in two groups, depending on the number of occurence. 
> - The small group should contain all major category that have less than 200,000 individual.
> - Making sure that the variable containing all the small groups is named something like "small_....".

