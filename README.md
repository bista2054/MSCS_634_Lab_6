# MSCS_634_Lab_6
Association Rule Mining with Apriori and FP-Growth

## Purpose
The purpose of this lab is to explore association rule mining techniques using the Apriori and FP-Growth algorithms on transactional data. The goal is to identify frequent itemsets, generate meaningful association rules, and visualize the results to uncover hidden patterns in the dataset. The lab also compares the efficiency and output of the two algorithms to understand their practical applications in real-world scenarios.

## Key Insights

### Data Preparation
- The dataset used is the Online Retail dataset from the UCI Machine Learning Repository, containing transactional data.
- Data cleaning steps included removing missing values, converting CustomerID to integers, and filtering out negative quantities.
- The cleaned dataset consists of more than 300K  transactions, around 4k unique customers, and 3k unique products.

### Frequent Itemset Mining
- **Apriori Algorithm:** Identified frequent itemsets with a specified support threshold. The top frequent itemsets were visualized using Seaborn's barplot.
- **FP-Growth Algorithm:** Applied the same support threshold as Apriori and compared the efficiency. FP-Growth was found to be faster for larger datasets due to its optimized approach.

### Association Rules
- Generated association rules using confidence and lift metrics.
- High-confidence rules indicated strong relationships between frequently co-occurring items.
- Visualizations (e.g., scatter plots) highlighted rules with high confidence and lift, providing actionable insights for business strategies like product recommendations.

### Comparative Analysis
- FP-Growth was more efficient than Apriori for this dataset, especially with lower support thresholds.
- Both algorithms yielded similar frequent itemsets, but FP-Growth scaled better with larger transaction volumes.

## Challenges and Decisions

### Data Set Selection
Finding an appropriate dataset took longer than expected. I tried downloading and using different versions, but ultimately, using a direct URL to access the dataset helped smooth things out and made the process easier.

### Important Module
Working with some key modules was a bit tedious at times because they seemed to cause issues on my machine. I had to restart my system a few times and try again to get everything running smoothly.

### Visualization
Coming from a Java background, visualization wasn’t as straightforward for me as it is with Python or JavaScript. I had to rely on online resources and examples to get the visualization code working properly in the Python notebook.
