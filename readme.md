# Market Basket Analysis with Power BI and Apriori

This project demonstrates how **association rule mining** can be integrated into **Power BI** using **Python** to analyse transactional data and discover product associations.

The solution is implemented directly inside a Power BI report by running a Python script in **Power Query**, applying the **Apriori algorithm** to generate association rules from the BreadBasket dataset.

## Files

- `Market_Basket_Analysis_Dashboard.pbix`  
  Power BI report containing the complete market basket analysis workflow, including data preparation, rule generation, and interactive visualisations.

- `Market_Basket_Analysis_Notebook.ipynb`  
  Jupyter Notebook used to develop and validate the Apriori-based analysis outside Power BI.

- `breadbasket.csv`  
  Transactional dataset containing purchase records used for the analysis.

## Association Rule Mining Approach

The analysis follows these main steps:

1. Load and validate transactional data
2. Clean and standardise product names
3. Transform transactions into a basket matrix
4. Apply one-hot encoding
5. Generate frequent itemsets using Apriori
6. Derive and rank association rules using confidence and lift

The resulting rules are loaded back into Power BI as a structured table.

## Python Libraries

The Python script used in Power BI relies on the following libraries:

- `pandas`
- `mlxtend`

## Output

The dataset produced by the Python script includes:

- Antecedents
- Consequents
- Support
- Confidence
- Lift
- Leverage
- Conviction

These metrics allow users to explore and filter association rules interactively within Power BI.

## Notes

- Machine learning processing is executed during data refresh in Power Query.
- Support and lift thresholds can be adjusted in the Python script.
- Results may vary depending on parameter configuration.

## License

This project is provided for educational and demonstration purposes.
