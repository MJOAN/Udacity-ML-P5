# Udacity-ML-P5

## Project: Identify Customer Segments
Our final Udacity project will dive into unsupervised learning to "identify segments of the population that form the core customer base for a mail-order sales company in Germany. These segments can then be used to direct marketing campaigns towards audiences that will have the highest expected rate of returns. The data that you will use has been provided by our partners at Bertelsmann Arvato Analytics, and represents a real-life data science task." and files included are not apart of this repo due to size but, described below.

There are four files associated with this project (not including this one):
- `Udacity_AZDIAS_Subset.csv`: Demographics data for the general population of Germany; 891211 persons (rows) x 85 features (columns).
- `Udacity_CUSTOMERS_Subset.csv`: Demographics data for customers of a mail-order company; 191652 persons (rows) x 85 features (columns).
- `Data_Dictionary.md`: Detailed information file about the features in the provided datasets.
- `AZDIAS_Feature_Summary.csv`: Summary of feature attributes for demographics data; 85 features (rows) x 4 columns


#### More information to follow (_working on filling out completed README.md_)
##### running set of steps completed: 
      1. assess missing/nulls from azdias
      2. plotted that data for visual
      3. used function to replace "missing_unknown" values (used Udacity mentor function)
      4. replaced X, XX values as well
      5. dropped large null column 'KK_KUNDENTYP'
      6. create threshold for nulls which I thought best to be 13% 
      7. plot two groups 
      8. drop multi level or bi-level (except person) from azdias
      9. re-encode with simple map() on 'OST_WEST_KZ'
      10. create mixed categorical features from two column data 'PRAEGENDE_JUGENDJAHRE' and 'CAMEO_INTL_2015'
      11. create clean data function
      12. impute and scale azdias
      13. perform PCA on all components on azdias
      14. conclude 25 PCA's equate to about 90% variance 
      15. not sure if I correctly removed these OR if they remained in the variable
      16. plot pca using Udacity instructor plot helper functions
      17. re-apply PCA just on 25 components
      18. run scree plot using Udacity instructor plot helper functions
      19. iterate over PCA components looking at top and bottom features 
      20. assess categories of these PCA components using Data Dictionary
      21. apply KMeans on azdias using 10 clusters kept it simple to start 
      22. saved model as azdias model
      23.  investigate cluster distances with centers and scores using Udacity Instructor plot helper functions
      24. Plot centers, scores, for "elbow" plot
      25. re-fit KMeans using 8 clusters get new model
      26. with new model get azdias labels/preds
      27. run clean data function on customers data for pre-processing
      28. need to have same # of columns to compare azdias and customers
      29. used pandas difference, and intersection to get same columns shape
      30. run impute, scale on customers  using fit_transform()
      31. run PCA with 25 components on customers using PCA function 
      32. run predict on azdias model using customers pca data
      33. get customers labels/preds 
      34. compare proportion of data in each cluster for both datasets
      35. get azdias preds, and customers preds, and compare.
