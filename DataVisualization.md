1. Data visualization :-
	1. Data visualization is a technique in Data Science which is used to analyze and visualize the data graphically
	2. It uses charts, boxplots, histograms, bar graphs etc
	3. It consists multiple libraries like: Matplotlib, Seaborn, Plotly, Cufflinks etc
	4. It can be used with code: Matplotlib, Seaborn etc. And with tools: Power BI, tableau, Google Data Studio
	5. The whitespace in which the plots are made is called a Canvas

2. Matplotlib :-
	1. plt.plot(x, y) : plots a line graph with x-axis and y-axis
	2. plt.xlabel('x_name') : plots the labels for x-axis
	3. plt.ylabel('y_name') : plots the labels for y-axis
	4. plt.title('title_name') : plots the title of the plot
	5. plt.subplot(row, column, select) : plots multiple plots at the same time. Note: for subplot() you have to plot() only below the selected part of the canvas
	6. fig = plt.figure() : used to initialise the figure function
	7. axis = plt.add_axes([slide_left, slide_bottom, width, height]): used to add the width and height of the canvas
	8. axis.plot(x, y) : plot the figure with the axes

3. Types of plots in Matplotlib :-
	1. plt.scatter(x, y) : plots a scatter plot
	2. plt.hist(x) : plots a histogram
	3. plt.boxplot(x) : plots a boxplot
	4. plt.save('filename.png') : saves the plot. Note: extension may vary

4. Distribution and Categorical plots :-
	1. Quantitative vs Qualitative variables
		1. Quantitative : continous values(Distribution plots)
		2. Qualitative : categorical values(Categorical plots)
	
	2. Distribution plots :
		1. distplot/histplot = used for basic data distribution
		2. jointplot = used for comparing two plots
		3. pairplot = used for comparison of numeric values
		4. rugplot = used for basic points distribution
	
	3. Categorical plots : 
		1. boxplot = used with 5 number summary. Note: X-axis should be quanti and y-axis should be qualy. Also, some circles are called Outliers
		2. violinplot = similar to boxplots
		3. stripplot = used with scatter plots where one variable is categorical
		4. swarmplot = similar to stripplot 
		5. barplot = used for plotting both quantitative(y-axis) and qualitative(x-axis). Note: barplot() works with estimators(by-default it uses mean())
		6. countplot = used for count of columns or features
	
4. Seaborn :-
	1. sns.load_dataset() : loads some toy dataset from seaborn itself
	2. sns.distplot(columnName, kde = True) : plots a distplot
	3. sns.jointplot(x, y, df, kind) : plots a jointplot
	4. sns.pairplot(df, hue) : plots a pairplot
	5. sns.rugplot(df) : plots a rugplot
	6. sns.countplot(x, hue, estimator) : plots a countplot
	7. sns.boxplot(x, y) : plots a boxplot
	8. sns.barplot(x, y) : plots a barplot
	9. sns.violinplot(x, y) : plots a violinplot
	10. sns.stripplot(x, y) : plots a stripplot
	11. sns.swarmplot(x, y) : plots a swarmplot

5. Matrix plot in seaborn :-
	1. Heatmap = used to plot correlation between the columns. Note: for using heatmap you have to find out the correlation by data.corr()
		~ sns.heatmap(data.corr(), annot = True)