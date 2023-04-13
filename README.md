# assignment-5: Step by step explaination of the code
Importing Libraries: The script starts by importing the necessary libraries including NumPy, SciPy, Pandas, Matplotlib, Seaborn, and warnings.

Suppressing Warnings: The warnings.filterwarnings(action="ignore") line of code is used to suppress warning messages that may be generated during the execution of the script.

Reading CSV File: The pd.read_csv("Salaries.csv") function reads the "Salaries.csv" file and stores it in a Pandas DataFrame called df.

Creating Histograms: The next few lines of code create histograms using Matplotlib and Seaborn. The plt.hist() function is used to create a histogram of the 'salary' column in the DataFrame with 10 bins and normalized density. The sns.distplot() function is used to create a histogram using Seaborn.

Creating Bar Plots: The code then creates bar plots using both Matplotlib and Seaborn. The df.groupby(['rank'])['salary'].count().plot(kind='bar') function is used to create a bar plot using Matplotlib, which groups the data by the 'rank' column and counts the occurrences of 'salary' for each group. The sns.barplot() function is used to create a bar plot using Seaborn, with 'rank' on the x-axis, 'salary' on the y-axis, and the 'len' estimator to count the occurrences of 'salary' for each 'rank' group.

Creating Scatter Plots: The sns.jointplot() function is used to create a scatter plot using Seaborn, with 'service' on the x-axis, 'salary' on the y-axis, and data from the DataFrame 'df'.

Creating Box Plots: The sns.boxplot() function is used to create a box plot using Seaborn, with 'rank' on the x-axis, 'salary' on the y-axis, and 'sex' as the hue to create side-by-side box plots for each combination of 'rank' and 'sex'.

Creating Pair Plots: The sns.pairplot() function is used to create a pair plot using Seaborn, which shows scatter plots for all possible pairs of numeric columns in the DataFrame 'df'.
