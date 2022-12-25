# Telecorm Churn Analysis

## Problem Statement

Telecom industry is growing rapidly with expanding internet,and electricity acess to more part of human population it also create opportunities to earn huge benefit for corporations to earn huge benefit but at the same time it create a stiff competition in between business firms in form of big marketing advertisement budget, low price and dynamic offers, way to provide better customer services and customer churn rate become matice to indicate firms position .
Recently, the companies are facing major challenge with customer churn, as customers switch to alternate provider due to various reasons like lower cost, multi service offerings, marketing promotions by competitors, etc.
So, The main aim of this project is to investigating the main reasons for customer churn in telecommunication sector and find a way to reduce it.

## Data Description 

- Total number of rows in data : 3333
- Total number of columns : 20(19 independent and 1 dependent colunn)
- Our dataset has 8 columns with float d-type, 8 columns with int d-type ,and 4 columns with object d-type.
● Churn: A binary identifier whether the customer has churned or not. -
● State: State in which the customer lives in.
● Account length: it is the no of days the account has been active.
● Area code: An identifier to the area the customer lives in.
● International plan: A binary identifier to whether the customer has opted for an international plan.
● Voice mail plan: A binary identifier to whether the customer has opted for a voicemail plan.
● Number Vmail messages: Number of voicemail messages sent or received.
● Total day minutes: How much the customer has talked over phone in the daytime.
● Total day calls: How many calls the customer has made over phone in the daytime.
● Total day charge: How much money was charged to the customer in the daytime.
● Total eve minutes: How much the customer has talked over phone in the evening.
● Total eve calls: How many calls the customer has made over phone in the evening.
● Total eve charge: How much money was charged to the customer in the evening.
● Total night minutes: How much the customer has talked over phone in the night.
● Total night calls: How many calls the customer has made over phone in the night
● Total night charge: How much money was charged to the customer in the night.
● Total intl minutes: How much the customer has talked over phone internationally.
● Total intl calls: How many calls the customer has made over phone internationally.
● Total intl charge: How much money was charged to the customer for international calls.
● Customer service calls: How many service calls were made to the customer.

## Data Preprocessing

- There are no null values, and if in any case we found that there was any null values.we can drop particular column if it is not relevant to database or we could use dropna() or fillna() function accordingly
- Trying to do appropriate outlier treatment in our dataset.
- Handling incoorect format of our feature columns. 
- There exists a perfect linear relationship between Minutes and its corresponding Charge which is true for all the features like international minutes and charges, night minutes and night charges,etc.

# EDA tools 

1. Bar Graph
Bar Graphs are the pictorial representation of data, in the form of vertical or horizontal rectangular bars, where the length of bars is
proportional to the measure of data. They are generally used to visualize categorical data. I have also used the grouped bar graphs or clustered bar graphs. 
It is used to represent values for more than one object that shares the same category

2. Histogram and Distribution Plots
A histogram is a bar plot where the axis representing the data variable is divided into a set of discrete bins and the count of observations
falling within each bin is shown using the height of the corresponding bar. Histograms aim to approximate the underlying probability density
function that generated the data by binning and counting observations. Kernel density estimation is used to approximately show the probability
density curve of the variable.

3. Box Plot:
A box and whisker plot—also called a box plot—displays the five-number summary of a set of data. The five-number summary is
the minimum, first quartile, median, third quartile, and maximum. It shows data spread, data distribution, 
central value of our variable with the help of median, and help us in outlier detection. The values our of upper and lower bound
whiskers can be treated as outliers here.

4. Pie Chart:
A Pie chart is a type of graph that displays data in a circular graph. The pieces of the graph are proportional to 
the fraction of the whole in each category. In other words, each slice of the pie is relative to the size of that category in the
group as a whole. Pie charts are often used to represent sample data—with data points belonging
to a combination of different categories .

5. Correlation Heatmap:
A correlation heatmap is a type of visualisation tool that shows a 2D correlation matrix between two discrete dimensions,
using coloured cells to represent data from usually a monochromatic scale. The colour of the cell is proportional to the
correlation between the variables that cross through row and column at that cell. It is assisted by a colour bar making data easily
readable and comprehensible.

6. Violin Plot
Violin Plot is a method to visualize the distribution of numerical data of different variables. It is similar to Box Plot but with
a rotated plot on each side, giving more information about the density estimate on the y-axis. 
The advantage of a violin plot is that it can show nuances in the distribution that aren’t perceptible in a boxplot. On the other
hand, the boxplot more clearly shows the outliers in the data.
Violin Plots hold more information than the box plots, they are less popular. Because of their unpopularity, their
meaning can be harder to grasp for many readers not familiar with the violin plotrepresentation. 

## Extrapolatory Data Analysis Observation

1 – Our churn rate was very high (around 14.5%) and we need to do something to
decrease the value of churn rate.
2- some states like New Jersey, California, Texas was showing high value of churn
rate , so we need focus on operation inside this states .
3 - Most customers who have international plan are churned. It could be because many of the
plan might have been taken by tourists who churned once their tour is over.
4 - Customer who didn’t have voice plan, they churned more
5- Higher the number of minutes, higher are the chances of customer churning as 
high minutes used may be indicating towards high pay to bill.
6- International minutes use was more in churned population than staying population.
7 – Higher the number of customer call user has to make, then the more likely they
are going to leave due to bad services.

## Conclusion

1 - Company should introduce plan with proportionally reduce charges as amount oF usage increase.
It could be like be like combo offer where many services are available in combinationat 
less price than each of them individually.
2 - Company should also focus on their quality of services as users start to churn
with a greater number of customers service class. 
3- Some states where churn is high like New Jersey, California, Texas, South
Carolina should receive company focus more and company should implement new
strategy here which was successful instates where churn is quite low.
4 - Company should try offer attractive voice plan offer to gain new users and
retain them
5- Company should offer better benefits with international plans to retain those
users.

