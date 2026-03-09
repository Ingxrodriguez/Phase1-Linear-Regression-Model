#### Phase1-Linear-Regression-Model

## Predicting Fish Toxicity Using Linear Regression

The goal of this project is to build a linear regression model that predicts fish toxicity (LC50) using molecular descriptors from the QSAR Fish Toxicity dataset. The project follows a standard data science workflow that includes data exploration, data transformation, and model development.

## 1.Dataset

The dataset contains chemical descriptors that describe molecular structures and their relationship to fish toxicity levels. The target variable is LC50, which represents the concentration of a substance required to cause toxic effects in fish.
[https://archive.ics.uci.edu/dataset/504/qsar+fish+toxicity]

## 2. Data Exploration
In the exploratory analysis stage, the dataset was examined to understand the distribution of variables and relationships between features. Several visualizations were created, including histograms, box plots, and a correlation heatmap. This step helped identify potential categorical variables and understand how different descriptors relate to the target variable.

![Heatmap](../Docs/Heat_map_Exploration_phase.png)

![Boxplot](../Docs/Boxplot_Exploration_phase.png)

## 3.Data Transformation

During the transformation stage, the dataset was cleaned and prepared for modeling. Duplicate rows were removed and the dataset was checked for missing values. The variables NdsCH and NdssC were identified as categorical variables and were converted into numerical format using one-hot encoding. The cleaned dataset was then saved as a new file to ensure the original dataset remained unchanged.


## 4.Model Development

A linear regression model was trained to predict LC50 using the transformed dataset. The dataset was divided into training and testing sets to evaluate how well the model performs on unseen data.

Model performance was evaluated using:

R² score, which measures how much of the variability in LC50 is explained by the model.

Mean Squared Error (MSE), which measures the average squared difference between predicted and actual values.

The model achieved an R² score of approximately 0.54, meaning that about 54% of the variability in LC50 can be explained by the features in the dataset.

![Evaluate_Model](../Docs/Evaluate_Model.png)



## 5. Model Interpretation

Regression coefficients were analyzed to understand which molecular descriptors have the strongest influence on LC50 predictions. A coefficient plot was used to visualize the impact of each feature on the model. Residual analysis was also performed to evaluate prediction errors and ensure the model behaves reasonably.

![Visualize_Coefficients](../Docs/Visualize_Coefficients.png)

![Residual_plot](../Docs/Residual_Plot.png)

## Technologies Used

Python

Pandas

NumPy

Matplotlib

Seaborn

Scikit-learn

## References
 -Scikit-learn Documentation: [https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html]
- Pandas Documentation: [https://pandas.pydata.org/docs/]
- Seaborn Documentation: [https://seaborn.pydata.org/]
-Medium website:[https://medium.com/@ishikacasley764/train-test-split-explained-simply-for-ml-beginners-7d4d9ebb7659]
-Rob Mulla [https://www.youtube.com/watch?v=xi0vhXFPegw&t=10s]







