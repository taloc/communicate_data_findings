# Project: communicate_data_findings
Final project of Udacity's DAND about visualizations using python libraries
To view the explanatory presentation please download and open the file: slide_deck_template.slides.html


## NOTE: If you are a Udacity student doing the DAND, please do not plagiarize this project

The academic objective of this project is to demonstrate the skills of:
- Using python's visualizations libraries
- Importing a dataset and run exploratory and explanatory analysis, based on visualization techniques
- Identifying oddities, patterns, outliers and insights from the dataset
- Creating a presentation from Jupyter Notebooks using the built-in functions

## Datasource
The dataset is from a company called Prosper that contains loans information of 113936 rows and 81 columns.

### Dataset
Loan data from Prosper (can't include the csv due to github size limits):
https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv

Data dictionary: https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0

## Libraries used:
- pandas
- numpy
- matplotlib.pyplot
- seaborn

#### After that wrangling work these were some of the initial hypothesis that came to my mind:
- What are the popular reasons why people ask for loans (Listing Category)
- Do Prosper clients' have a good credit grading?
- Can we profile the type of most profitable client?
- And, can we profile the type of client that might default?
- How large are the amounts of loans? 
- Is there a correlation between certain variables?
- Is the location of a borrower a factor of whether or not they are good clients?


## Summary of Findings

A methodological exploration process was applied using various visualization techniques to plot univariate, bivariate and multivariate relations.

#### Interesting findigs:
- Majority of Prosper clients are in the highly populated States of the United States
- The top most common reason to request loans are for debt consolidation and usually their terms are for 36 months
- The credit grading of Prosper clients is balanced, meaning that they have a significant number of clients with gradings AA, A and B, while most of their clients are full-time and self-employed.
- Prosper's internal rating codes, can demonstrate how better rating reduces the chance of having unprofitable clients (negative estimated returns).


## Key Insights for Presentation

Please open the file slide_deck_template.slides.html to view the presentation in a web browser. The presentation is focused in the understanding of the Prosper client's profile. We can assume that this information can be used for marketing and sales purposes to better target a clientele that is both credit worthy and profitable for the company.

I used a series of bar charts to analyze single categorical variables such as: credit grading, listing category, status of the loan and the borrower's State. This gave me a first insight on the profile of the clients and loans.

Then I added a new dimensions to be able to plot both bivariate and multivariate visualizations, for this I had to use a color coding to visualize a different level of insight. In these visualizations I studies the credit rating and the employment status, credit rating and the listing category and finally the listing category with the term of the loan. This analysis provided a new level of insight on what the clients are using their loans, for how long and what is the credit rating of those loans.

Finally, the most important insight for me was to focus on the profitability of Prosper from the perspective of the borrower's rate and estimated returns. Prosper has 7 different internal ratings from 1 to 7 (seven being the best rating). It was quite revealing to corroborate that the lowest Prosper rating (1) tends to produce the lowest estimated returns (negative estimated retuns) which are unprofitable. As the Prosper rating increases towards 7 we can observe how the estimated returns slightly move to the right on the X axis where the estimated return variable is plotted.


#### Disclaimer on limitations of the analysis:
The above analysis is limited to descriptive statistics from a limited set of data from the Prosper loan dataset. The results cannot be used to project future estimations as more information and different predictive statistics methods should be used to produce such numbers.


## External sources and references:
https://www.investopedia.com/terms/a/aaa.asp

https://en.wikipedia.org/wiki/Charge-off

https://seaborn.pydata.org/generated/seaborn.countplot.html
