
                    **Lab 1: Data Visualization, Data Preprocessing, and Statistical Analysis Using Python**
By: Murali Krishna Vattikunta
Dataset: Superstore Sales (via Kaggle)
Introduction:
The main goal of this lab was to get comfortable digging into a dataset using Python. Working with the Superstore Sales data, I focused on cleaning it up, handling formatting issues, running some basic stats, and building visualizations. The aim was to take raw data and turn it into something readable and insightful using Python’s core data science stack: Pandas, NumPy, Matplotlib, and Seaborn.

My Key Takeaways & Findings
1. Visualizing the Data
Sales Trends: Looking at the data, order sizes fluctuate wildly. Line plots showed a lot of spikes and dips, pointing toward seasonal demand or unpredictable buying habits.
Category Breakdown: Bar charts made it easy to see which product categories and sub-categories are pulling in the most revenue versus those falling short.
Distribution: Histograms revealed that most sales are relatively low-dollar amounts, with just a few massive orders creating a long tail.
2. The Statistical Breakdown
Skewed Numbers: The standard deviation for sales outpaced the mean, proving that the data is heavily skewed by a few major transactions.
Scaling & Normalization: Applying Min-Max scaling squished the sales numbers neatly between 0 and 1, which makes comparisons much easier.
Spotting Outliers: Using Z-scores and correlation analysis, I was able to mathematically prove just how far out those extreme sales values were from the average and see how different numerical variables moved together.
Challenges Faced & Decisions Made
Dealing with Missing Data: I couldn't just use a one-size-fits-all approach for missing values. I had to mix it up using forward fills, backward fills, and mean imputation depending on what made sense for each specific column.

Data Type Cleanup: The Postal Code column was originally loading as a float (with decimals), which looked messy. Once the missing values were handled, I converted it over to a clean integer format.
Environment Headaches: One of the most frustrating roadblocks wasn't the data itself, but version compatibility issues between NumPy, Pandas, and SciPy. I had to spend some time adjusting my environment packages to get everything running smoothly.
Handling Outliers: The IQR (Interquartile Range) method flagged some massive outliers in the Sales column. I ended up filtering these out to prevent them from skewing the overall analysis, which gave me a much cleaner baseline to work with.
Tech Stack Used
Python
Pandas
NumPy
Matplotlib
Seaborn
