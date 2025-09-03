# UC BERKELEY - CAPSTONE PROJECT IN MACHINE LEARNING & AI

<a href="https://github.com/kfmatovic716/HEALTH-INSURANCE-COST-ML.git"><h2 align="center">HEALTH INSURANCE COST PREDICTION & RISK ANALYSIS USING MACHINE LEARNING TECHNIQUES</h2></a>

![Logo](images/healthinsurance.jpeg)


## INTRODUCTION
The growing emphasis of health equity has recently become a major priority in the United States and it has contributed to the rising healthcare costs. Leveraging health insurance data to predict future claims costs and identifying key factors that drive these  escalating costs can provide actionable insights to improve decision-making and expense management of health insurance providers.

## PROBLEM STATEMENTS 
<ul>
    <li>Based on an individual’s demographic and lifestyle, can we predict the individual’s health insurance charges accurately?</li>
    <li>Can we classify who would likely incur <strong>high</strong> versus <strong>low</strong> health insurance costs?</li>
    <li>What factors strongly influence health insurance costs? </li>
</ul>

## GOALS 
<ul>
    <li><strong>Cost Prediction</strong> - Build a baseline predictive model using <strong>Linear Regression</strong>, then enhance performance using <strong>Ridge and Lasso Regression</strong>. Evaluate models using <strong>R-squared, Mean Absolute Error (MAE), and Mean Squared Error (MSE)</strong> metrics.</li>
    <li><strong>Risk Classification</strong> - Classify individuals into <strong>high-cost or low-cost</strong> categories using Logistic Regression, based on lifestyle features and/or predicted charges.
</li>
    <li><strong>Feature Importance</strong> - Determine the most influential feature that affects health insurance cost using <strong>GridSearchCV</strong></li>
</ul>


## DATA ACQUISITION
<ul>
    <li><strong>SOURCE: </strong> Kaggle ➡️ <a href="https://www.kaggle.com/datasets/harishkumardatalab/medical-insurance-price-prediction"><strong style="font-size: 16px;">Health Insurance Cost Data</strong></a></li>
    <li><strong>DATA SIZE: </strong>The raw data has 7 features and 2,772 records in total</li>
</ul>

## DATA DESCRIPTIONS
<p>The dataset contains the following features, along with their data types and corresponding descriptions: </p>
<ul>
    <li>age - person’s age</li>
    <li>sex - person’s gender</li>
    <li>bmi -  body mass index</li>
    <li>children - number of children</li>
    <li>smoker - indicates if person is smoker (“yes”) or non-smoker (“no”)</li>
    <li>region -  US region where person resides</li>
    <li>charges (target variable) - insurance premium price<</li>
</ul>
        
## EXPLORATORY DATA ANALYSIS (EDA)
<ul>
    <li><strong>Missing Values and Duplicate Records</strong></li>
    <ul>
        <li>There were no missing values in the column features</li>
        <li>There were 1,435 duplicate rows that were deleted from the rawdata; Some of the records didnt just have one duplicate but 3 duplicates!</li>
        <li>There were <strong>total of 1,337 records in the new dataset</strong> after deleting duplicates</li>
    </ul>
    <br>
    <li><strong>Univariate Analysis and Outlier Detection</strong></li>
    <ul>
        <img src="/images/age.png"/>
        <li>The age distribution is skewed to the right, which means that the majority of individuals fall within the younger age range (18–20). The curve then stretches gradually toward older ages, extending up to age 63. The smallest representation is seen at ages 64–65, which aligns with expectations in the context of insurance: individuals over 65 are typically considered higher risk, making them less desirable participants for many insurance plans. </li>
        <li>Age appears to have a consistent distribution and no present outliers in the feature</li>
        <img src="/images/bmi.png"/>
        <li>Body Mass Index categories are as follows: underweight are <18.5, healthy weight: 18.5 to less than 25, overweight: 25.0 to less than 30.0 and obesity: >=30.0 </li>
        <li>The BMI illustrates an approximately normal distribution, with the highest concentration of values between 25 and 35 which corresponds to the overweight and obese categories. The tail-end distributions represent individuals in the healthy weight range on the lower end and the severely obese group on the upper end. </li>
        <li>This distribution reflects prevailing health and lifestyle patterns in the US. A significant proportion of the population is overweight, largely attributed to poor nutrition, high stress levels, and sedentary lifestyles.</li>
        <li>There were a few outliers (approximately 7) with BMI over 47 that are severely obese </li>
        <img src="/images/children.png"/>
        <li>The 'number of children’ feature shows a right-skewed distribution. The majority of participants (approximately 575) reported having no children, followed by 324 participants with one child. The frequency declines progressively as the number of children increases, forming a long tail toward higher values. </li>
        <li>There were no outliers to be observed in this feature</li>
        <img src="/images/charges.png"/>
        <li>The health insurance cost, which serves as the target variable, is right-skewed, indicating that the majority of the population pays less than $14K. However, there is a notable presence of outliers, with some individuals incurring costs exceeding $34K.</li>
        <img src="/images/gender.png"/>
        <li>Population in gender feature is evenly distributed, approximately 50% are  males and 50% female participants</li>
        <img src="/images/smoker.png"/>
        <li>There is approximately 80% non-smoker population in this dataset, indicating class imbalance. </li>
        <li>The model might achieve high accuracy by mostly predicting “non-smoker,” but it would perform poorly in detecting smokers without adjustment</li>
        <img src="/images/region.png"/>
        <li>The regions of origin are evenly distributed among participants in this dataset, with the exception of the Southeast, which has a slightly higher representation</li>
    </ul>
    <br>
    <li><strong>Bivariate Analysis</strong></li>
        <ul>
            <li></li>
            <li></li> 
        </ul>
    <br>
    <li><strong>Multivariate Analysis</strong></li>
        <ul>
            <li></li>
            <li></li> 
        </ul>
</ul>
            
## DATA TRANSFORMATIONS
            
## MODELLING USING MACHINE LEARNING ALGORITHMS

## EVALUATION

## RECOMMENDATIONS TO CLIENT

## FUTURE RECOMMENDATIONS - IMPROVEMENTS ON DATA QUALITY AND PERFORMANCE OF THE MODELS

