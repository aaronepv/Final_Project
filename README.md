<img src="https://bit.ly/2VnXWr2" alt="Ironhack Logo" width="100" align="right"/>


#   Project - How difficult would be to be able to predict a winner(Blue or Red) for betting purposes?

Aaron Elias Pérez

*Data Part Time Barcelona Jun 2020*


## Content
- [Project Description](#project)
- [Dataset](#dataset)
- [Workflow](#workflow)
- [Results](#results)

<a name="project"></a>

## Project Description

The goal of this project is to find a prediction of a fight if Red or Blue fighter will win.
This is a data set of  UFC fight in the history of the organization. Every row contains information about both fighters, fight details and the winner.


<a name="dataset"></a>

## Datasets

Datasets:
- [Compiled UFC fight, fighter stats and information]/(https://www.kaggle.com/rajeevw/ufcdata).

<a name="workflow"></a>

## Workflow

- **Exploratory Data Analysis (EDA):**
  - Data Collection
  - Understanding the Dataset
  - Understanding Variables
  - Data Cleaning
  - Data Transformation
  - Data Visualization

 
 
 **Libraries Used:**

 - Scipy
 - NumPy
 - Pandas
 - Seaborn
 - Matplotlib
 - sklearn
 - xgboost (our best model for this project)

 
<a name="results"></a>

## Results

**Results from the Exploratory Data Analysis:**
 - 145 columns and 5144 rows
 - Red fighters have won more fights and titles than blue
 - The age of the fighters is concentrated between 25 and 30 years old (Men Fighters)
 - Most of the winners are between 28 and 30 years old (Men Fighters)
 - The main location for the fight even are in USA
 - The most common class weight is Lightweight and Welterweight (Men Fighters)
 - Tthe heavyweight category are lots of variety in weight and height
 - The female weight division is more controlled than the male's weight division.
 - The most common class weight is Strawweight and Bantamweight (Women Fighters)
 - The age of the fighters is concentrated between 26 and 32 years old (Women Fighters)
 - Most of the winners are between 28 and 30 years old (Women Fighters)
 

**Results from the Correlation analysis:**
 - The correlation between all the variables is minima and the varianza is very low.


**Results from the Ramdon Forest model:**
 - The accuracy is 0.64 of a fight prediction, but this model gives more importance to red than to blue.

**Results from the K-Nearest Neighbor (KNN) model:**
 - The accuracy is 0.61 of a fight prediction, this model does not work properly.
 
 **Results from the PCA model:**
- The accuracy is 0.62 of a fight prediction, this model works well although the accuracy is too low.

**Results from the XGB Classifier:**
This is the best model for the project because mainly allows us to get an ensemble model with a lower bias than its components: that is why weak learners with low variance but
high bias is well adapted for boosting.

Note:
Bias is the difference between the average prediction of our model and the correct value which we are trying to predict.

- The accuracy is 0.67 of a fight prediction, this model works properly because gives the same importance to red and blue.


<br><br>
 
 ## Next Steps
 
 - Collect more data about every single fighter and their hours of train before the combat.
 - Get some medical data about the fighter to study how many injuries the fighter comes to the fight.
 - Use all this information to compare a future fight between them and get and individual prediction.

