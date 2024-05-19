> [!NOTE]
> If an error occurs with the opened Jupyter Notebook on GitHub, copy and paste the notebook into this instead: https://nbviewer.org/

# Basket Analysis
Market Basket Analysis is a data mining technique employed to discover relationships and patterns within large datasets, particularly in the context of market analysis. By identifying frequently co-occurring items in transactions, businesses can gain valuable insights into customer behavior, optimize product placement, and enhance overall marketing strategies.

## Data
This Online Retail II data set contains all the transactions occurring for a UK-based and registered, non-store online retail between 01/12/2009 and 09/12/2011.The company mainly sells unique all-occasion gift ware. Many customers of the company are wholesalers.

The dataset can be accessed at the following link:
https://www.kaggle.com/datasets/mashlyn/online-retail-ii-uci/

## Objectives
1. **Association Rule Discovery**: Identify associations and correlations among products or items in a dataset. Discover rules that indicate the likelihood of certain items being bought together.
2. **Cross-Selling Opportunities**: Uncover opportunities for cross-selling by understanding which products are frequently purchased together.
3. **Promotion Planning**: Optimize promotional campaigns by identifying items that are frequently bought together. Design effective promotions and discounts to incentivize the purchase of complementary products.
4. **Optimizing Product Layout**: Arrange products in-store or online in a way that encourages the purchase of related items, creating a more convenient and satisfying shopping experience.

## Method
<h3>Apriori algorithm</h3>

- We utilize the Apriori algorithm for conducting market basket analysis.
- This algorithm proves highly effective in discerning frequent itemsets and deriving association rules, relying on predefined metrics like support and confidence.
- To execute the Apriori algorithm, we utilize the mlxtend library, a reliable Python library for machine learning extensions.

**The following parameters are configured for the algorithm:**
- Maximum Combination Length
  - We set the maximum combination length to 2 items.
  - This choice is made to focus on pairs of items, allowing for a more targeted analysis of co-occurrences.
- Minimum Co-Occurrence Support Threshold
  - A minimum co-occurrence support threshold of 1% is established to filter out infrequent itemsets.
  - This ensures that only associations with a significant presence in the dataset are considered.

## Summary Reports
> [!NOTE]
> For a comprehensive and interactive view please visit the following link https://basket-analysis.streamlit.app/

<h2>Top 5 Products based on support</h2>
<div align=center>

  ![image](https://github.com/Agungvpzz/Basket-Analysis/assets/48642326/37062fde-5881-4424-af4f-304b9453e2e2)
</div>
  
<h2>Network Profile</h2>
<div align=center>
  
  ![image](https://github.com/Agungvpzz/Basket-Analysis/assets/48642326/ca25a6b2-51db-4fda-a3ed-dbba479f4c84)
</div>


<h2>Bundling Products with minimum confidence 50%</h2>
<div align=center>
  
  ![image](https://github.com/Agungvpzz/Basket-Analysis/assets/48642326/4bdb9878-5aa2-4cdd-a580-15bd66cb7911)
  ![image](https://github.com/Agungvpzz/Basket-Analysis/assets/48642326/b33d56e2-3e1b-4232-bfa9-23544b34d324)
</div>


<h2>Product Heatmap Layout</h2>
Selected category: "RED STRIPE CERAMIC DRAWER KNOB"
<div align=center>

  ![image](https://github.com/Agungvpzz/Basket-Analysis/assets/48642326/743f627d-c5a5-4264-9b0c-0ef510b708b5)  
</div>







