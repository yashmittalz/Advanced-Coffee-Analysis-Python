# Part 2: Video Script (5-7 Minutes)

**Notes for recording:**
- Have your Jupyter Notebook open.
- Run the cells before you record so the graphs are visible.
- Highlight the "Upgraded" sections (CAGR and Forecasting) as these are specific requirements for Project 2.

## [0:00 - 1:00] Introduction
"Hello, this is [Your Name] presenting Project 2 for DAT 301.
For this project, I transitioned my analysis from R to Python. I am analyzing the Coffee_domestic_consumption dataset.
My goal was to replicate previous findings regarding global trends but also to upgrade the analysis by adding Growth Rate calculations and a Machine Learning Forecast for future years."

## [1:00 - 2:30] Data Wrangling with Pandas
*(Scroll to Cell 4)*
"I used the Pandas library for data manipulation. The biggest challenge, similar to Project 1, was the shape of the data. It came in a wide format.
I used the Pandas melt function—which is the Python equivalent of pivot_longer—to transform the years into rows.
I also used a lambda function to clean up the 'Year' column, converting strings like '1990/91' into integers. This prepared the data for our modeling later."

## [2:30 - 3:30] Basic EDA
*(Scroll to Cell 6 & 8)*
"Using Seaborn for visualization, we can see the Global Trend here. It is a steady, linear increase.
In the 2019 analysis, Brazil is the clear leader in volume, followed by Indonesia. But volume isn't everything..."

## [3:30 - 5:00] The Upgrade: CAGR & ML
*(Scroll to Cell 10 - CAGR)*
"This is where I expanded the project. I wanted to know who is growing the fastest, not just who is the biggest.
I calculated the Compound Annual Growth Rate (CAGR) for the top 5 countries.
*(Point to the Green Bar Chart)*
Interestingly, while Brazil is the biggest consumer, Vietnam (the second bar here) has the highest growth rate over the last 30 years, growing at nearly 10% annually. This suggests Vietnam is a crucial emerging market."

*(Scroll to Cell 12 - Forecast)*
"Finally, I used the Scikit-Learn library to perform a Linear Regression.
I trained the model on data from 1990 to 2019 and asked it to predict the future (2020 to 2025).
*(Point to the Scatter Plot)*
The orange dots represent our machine learning predictions. The model has a very high R-Squared score, and it predicts that global consumption will continue to rise, crossing roughly 55 million bags by 2025."

## [5:00 - End] Conclusion
"In conclusion, moving this project to Python allowed me to leverage Scikit-Learn for predictive modeling. We found that while Brazil leads in volume, Vietnam leads in growth speed, and the overall global market shows no signs of slowing down. Thank you."
