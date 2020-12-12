## Classification_Wine_Quality
Flask application to allow vinter's to predict wine quality classification.
## Project Description:

The premise of this project is to apply data science principles to shorten the barrel to bottle cycle time for niche vintners.  Using commonly tracked wine attributes to predict if a wine will be classified as prime or subprime. Early quality classification could enable advanced S&OP, budget forecasting, avoid costly last-minute marketing changes.

**Objective:**
The objective of this project is to provide niche wine vintners with a tool to predict wine quality that is tailored to their own threshold for precision and accuracy all based on commonly tracked wine attributes.

**Methodology:**
The data was a combination of two from Kaggle. One for red and one for white wines:

- [red wine kaggle dataset](https://www.kaggle.com/sgus1318/winedata)
- [white wine kaggle dataset](https://www.kaggle.com/sgus1318/winedata?select=winequality_white.csv)

The commonly tracked wine features are: 
• Alcohol
• Sulphates
• pH
• Density
• Total Sulphur Dioxide • Free Sulphur Dioxide • Chlorides
• Residual Sugar
• Volatile Acidity
• Fixed Acidity 

I used classification to design a learning model based on precision metric. In this case, using precision metric is based on the assumption that purchase of materials is based on forecast. 
Logistic Regression, K-Nearest Neighbors, and Random Forest models were trained and compared on the Receiver Operating Characteristic curve. Random Forest scored the highest at 0.86 True Positive rate and is the recommended model for this application.  I took the analysis a step further to principle component analysis discovering, perhaps not surprisingly, alcohol is the most important feature. 
Finally, I tied the analysis into a Flask application.

**Results:**

The user can customize inputs of their wine attributes into the Flask application and get a prediction as to wine quality.  The application is based on Random Forest as the classifier precision as the metric.
