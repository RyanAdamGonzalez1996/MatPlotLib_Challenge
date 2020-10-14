# MatPlotLib_Challenge

Read in data from two csv files and manipulate and format the data onto multiple graphs to properly convey and report the data. After words, write a report on three observations

OBSERVATIONS ##################################################

1. Propriva having the lowest amount of datapoints shows that the success rate for this drug is low, as the mice are not living long enough to get the full amount of datapoints. Likewise, Capomulin seems to have the highest success rate as it is the drug regimen with the highest amount of datapoints, indicating that the mice on that regimen are living longer.

2. For the Capomulin regimen, it shows a correlation between the size of the average tumor with the heavier mice. This can show that the dosage is not as potent for the bigger mice and/or the tumor growth seems to be correlated with a mouse's size.

3. Based off of the box and whisker plot, Ceftamin has the least consistency of all of the four tested regimens. This data shows that the the drug seems to only work for specific mice, possibly due to their genetics, and despite it working well for select mice, the drugs overall ability to reduce tumor size, is definitely one of the least effective regimens.

###############################################################

## Instructions

Your tasks are to do the following:

* Before beginning the analysis, check the data for any mouse ID with duplicate time points and remove any data associated with that mouse ID.

* Use the cleaned data for the remaining steps.

* Generate a summary statistics table consisting of the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen.

  **Hint**: You can calculate each statistic on a single line using .agg. Use this [Group and Aggregate by One or More Columns in Pandas](https://jamesrledoux.com/code/group-by-aggregate-pandas) for reference.

* Generate a bar plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows  the number of total mice for each treatment regimen throughout the course of the study.

  * **NOTE:** These plots should look identical.

* Generate a pie plot using both Pandas's `DataFrame.plot()` and Matplotlib's `pyplot` that shows the distribution of female or male mice in the study.

  * **NOTE:** These plots should look identical.

* Calculate the final tumor volume of each mouse across four regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Calculate the quartiles and IQR and quantitatively determine if there are any potential outliers across all four treatment regimens.

* Using Matplotlib, generate a box and whisker plot of the final tumor volume for all four treatment regimens and highlight any potential outliers in the plot by changing their color and style.

  **Hint**: All four box plots should be within the same figure. Use this [Matplotlib documentation page](https://matplotlib.org/gallery/pyplots/boxplot_demo_pyplot.html#sphx-glr-gallery-pyplots-boxplot-demo-pyplot-py) for help with changing the style of the outliers.

* Select a mouse that was treated with Capomulin and generate a line plot of tumor volume vs. time point for that mouse.

* Generate a scatter plot of mouse weight versus average tumor volume for the Capomulin treatment regimen.

* Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment. Plot the linear regression model on top of the previous scatter plot.

* Look across all previously generated figures and tables and write at least three observations or inferences that can be made from the data. Include these observations at the top of notebook.

Here are some final considerations:

* You must use proper labeling of your plots, to include properties such as: plot titles, axis labels, legend labels, _x_-axis and _y_-axis limits, etc.

* See the [starter workbook](Pymaceuticals/pymaceuticals_starter.ipynb) for help on what modules to import and expected format of the notebook.
