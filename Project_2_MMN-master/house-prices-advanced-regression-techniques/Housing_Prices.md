## Project 2:  Housing Price
<b>Team numbers: 10 

Team members: Maha Aldosary - Noha Zamaan- Mariah Alshiekh(leader)</b>


***
### Overview:
This project is working to predict the price of houses depending on the features of each house. the data that deal with it is collected from Kaggle compittion websit which contains two datasets (train_data and test_data). 
***
### Methodology of Processing:
1-import all library that used .</b> 

2- Uploading the two dataset(train -test)data.</b>

3-Disply the data by using several functions such as '.head()',  '.info()' ,'.describe()'.</b>

4- Chick missing value via : </b>
- 'isnull()sum()' to count the missing value for each feature.
- using method to count the number of columns that have missing value.
- calculate the presentage of missing value fro each column.</b>
#### Remove noise from data:
we applied different strategy to removing null value:</b>

a- The columns that have just two missing value ,fill them via 'mode' approach becuase it contain small number, so no big deal to apply complex method.</b>

b- Some columns have missing value but in real no, 'nan' in these columns mean this feature not available in this house, so we fill them by replacing 'nan' to '0' in nemoric columns and 'no feature' in object columns.</b>
#### Dummy function :

we use '.get_dummies' to covert columns to [0,1] values beacuse in this project we will use regressor type for each model so, we need to prepare our feature to be ready.</b>
#### Correlation :
 Correlation funtion is used with 'heatmap.corr()' to see the realation betwwen target and features.Addtion, using heatmap to double check that both data do not contain missing value
#### Visulazition:
we applied different types of ploting such as ['Histogram','Boxplot','Lineplot','bar'] to easy understand the freatures.and their relation with target(Price_Sale) 
</b>
### Preparing for modeling:
- Caculate the baseline. 
- Assign X_train,y_train and X_test by 3 strategy:
   * <b>Frist strategy:</b> Using only the features that have nemorics value
   *<b>Second strategy:</b>  Using the features that have more or equal 0.6 correlation value with target.
   * <b>Third strategy:</b> Using all features
### Modeling:
We applied a veriety of strategies
- First Steratgy:using nemoric features we use 
['Linear_regression', 'Ridge_regressor', 'Lasso_regressor', 'Random_Forest', 'Extra_trees', 'Knn_regression', 'Decision_tree', 'Bagging_regressor'] models</b>
-Second Sttrategy: usinf=g features that have high correlation with target. We use  [Random_Forest, Extra_trees, Bagging_regressor]models
- Third strategy: using all features with  [Random_Forest, Extra_trees, Bagging_regressor] models

### Results:


The best result was in Random_Forest and the worth result was in Decision_tree.</b>

- Second Strategy: using high correlation features with target.</b>
the best score was in Extra_Tree model and the worth score was in Bagging model.
- Third Strategy: using all features.</b>
the best score was in Random_Forest model and the worth score was in Bagging model.
#### Finally
The best score we got in using the nemoric features strategy without scale and Grid_search in <b>Random_forest model</b>.






