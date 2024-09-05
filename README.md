# Wine_dataset_analysis

<h4>1. Dataset and Features:</h4>
   
The dataset consists of 178 instances, with 13 attributes related to the chemical properties of wines grown by three different cultivators in Italy.
Key attributes include:
<h5>Alcohol:</h5> Alcohol content varies between 11.0% to 14.8%, with a mean of 13.0%.
<h5>Malic Acid:</h5> Ranges from 0.74 to 5.80, with a mean of 2.34, indicating variability in acidity among the wines.
<h5>Proline:</h5> Has the highest variability, with values ranging from 278 to 1680, reflecting differences in the wines' phenolic compounds.

<h4>2. Descriptive Statistics:</h4>
   
<h5>Central Tendency and Dispersion:</h5>
The mean and median values for most attributes are quite close, indicating a fairly symmetric distribution for attributes like alcohol and magnesium.
Attributes like malic acid and color intensity have higher skewness, indicating asymmetry in their distributions.
Standard Deviation and Variance: The attribute proline exhibits the highest standard deviation (314.9), indicating it is highly dispersed around the mean.
<h5>Range and Variability:</h5>
Alcohol shows a narrow range (3.8), while attributes like color intensity and proline have much larger ranges, highlighting significant differences among the wines.
<h5>Skewness and Kurtosis:</h5>
Positive skewness in malic acid (1.04) and magnesium (1.09) suggests these distributions have longer right tails.
Kurtosis values close to zero for most attributes indicate that the distributions are near normal, with magnesium showing the highest kurtosis (2.1), suggesting a more peaked distribution.

<h4>3. Inferential Statistics:</h4>
   
<h5>One-Sample t-Test on Flavanoids:</h5>
The t-test on the flavanoids attribute reveals a highly significant difference from the population mean of 0.05 (t-statistic ≈ 26.44, p-value ≈ 2.31e-63). This suggests that flavanoids content in the wine is substantially higher than the hypothesized mean, reflecting the distinctive characteristics of the wines.
<h5>Confidence Intervals:</h5>
For flavanoids, the 95% confidence interval (1.88 to 2.18) and the 99% confidence interval (1.84 to 2.22) provide a precise range within which the true mean flavanoids content lies. The narrow intervals reflect high confidence in the estimate of the mean.

<h4>4. Regression Analysis:</h4>

   
<h5>Logistic Regression Model:</h5>
The dataset was split into training and testing sets, and the features were standardized to improve model performance.
Logistic regression was employed to predict the wine classes (class_0, class_1, class_2) based on their chemical properties.
The model achieved an accuracy of 94.44%, suggesting that the chemical properties are strong predictors of wine type.
<h5>Model Performance:</h5>
High accuracy indicates the logistic regression model effectively differentiates between the three wine classes.
This suggests that the features, especially those with significant variability like proline, flavanoids, and color intensity, are key differentiators among the classes.

<h4>5. Implications and Recommendations:</h4>
    
The analysis highlights distinct chemical profiles for each wine class, which could be leveraged for wine quality assessment and classification.
The significant variability in attributes like proline and flavanoids underscores the importance of these compounds in wine differentiation and potential influence on taste and quality.
The high classification accuracy of the logistic regression model indicates potential for developing automated systems for wine classification based on chemical properties, aiding wine producers and quality control processes.
The model achieved an accuracy of approximately 94.44%, indicating a strong predictive performance.
