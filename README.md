# Online Retail: RFM Customer Segmentation for Marketing Strategy

Leveraging RFM analysis to segment a retail customer base and design targeted marketing campaigns for high-value cohorts.

---

### Objective
The goal of this project is to analyze a transnational retail dataset to identify key customer cohorts. By applying RFM (Recency, Frequency, Monetary) analysis, we can segment customers based on their purchasing behavior and design a data-driven marketing strategy to improve customer retention and profitability.

### Dataset
This analysis uses the "Online Retail" dataset from the UCI Machine Learning Repository. It contains transactional data for a UK-based online retail company from December 2010 to December 2011.

### Methodology

1.  **Data Cleaning & Preprocessing:**
    * Loaded the dataset of over 500K+ transactions.
    * Handled missing `CustomerID` values, which are essential for segmentation.
    * Removed returns (negative `Quantity`) and transactional outliers (e.g., extremely high quantities/prices) to create a clean, analysis-ready dataset.

2.  **Exploratory Data Analysis (EDA):**
    * Analyzed monthly trends in revenue, orders, and active customers to understand business seasonality and growth.
    * Identified top-performing products and customers to uncover key revenue drivers.

3.  **RFM Feature Engineering:**
    * Calculated **Recency**, **Frequency**, and **Monetary** values for each of the 4,300+ unique customers.

4.  **Quantile-Based Segmentation:**
    * Developed a scoring system (1-4) for each RFM metric based on quartiles.
    * Summed the scores to create a final `RFM_Score` for each customer.
    * Grouped customers into actionable segments: **Champions, Potentially Loyal, At Risk, Can't Lose, and Lost**.

5.  **Strategic Deep-Dive:**
    * Performed a detailed analysis of the most valuable segment, the 'Champions', to understand their specific product preferences.

### Key Findings & Insights

* **Strong Pareto Principle:** The analysis revealed that the top 0.25% of customers contribute a massive 17% of the total revenue, highlighting their critical importance.
* **Actionable Customer Segments:** The quantile-based RFM model successfully segmented the customer base, with 'Champions' making up 37% of all customers.
* **High-Value Product Affinity:** The 'Champions' cohort shows a distinct preference for specific products, providing a clear path for targeted marketing efforts.

### Final Outcome & Business Strategy

The project culminates in a **Campaign Blueprint** for the **'Champions'** segment. The strategy recommends:

1.  **Exclusive Access:** Offering early access to new products that align with their known preferences (e.g., home decor, party supplies).
2.  **Loyalty Program:** Creating a premium tier with special rewards to acknowledge their value and encourage continued purchasing.
3.  **Personalized Bundles:** Curating product bundles based on their purchasing history to increase average order value.

### Tools & Libraries

* **Python**
* **Pandas** for data manipulation and cleaning.
* **Matplotlib** & **Seaborn** for static visualizations.
* **Plotly** for interactive visualizations.
* **Scikit-learn** for K-Means clustering (used for initial exploration).
