# Sticking Together: A Look Into Attrition
## Comparison Machine Learning Project

# Contributors
  •	Karoly Burgyan<br>
  •	Shayla Badeaux<br>
  •	Christian Cantu<br>

# Sources
1.	[Database Source](https://www.kaggle.com/datasets/anshika2301/hr-analytics-dataset?select=HR_Analytics.csv)
2.	[Chat GPT](https://chat.openai.com/)
3.	[Stack Overflow](https://stackoverflow.com/)
4.	[Scikit-Learn](https://scikit-learn.org/stable/)
5.	[Hyperband Tuner](https://keras.io/api/keras_tuner/tuners/hyperband/)
7.	[Cultermap](https://web.archive.org/web/20230913171706/https://www.cultureamp.com/blog/cost-of-employee-turnover)
8.	[Investopedia](https://www.investopedia.com/terms/a/attrition.asp)


# Overview
HR analytics, commonly known as people analytics, workforce analytics, or talent analytics, involves the aggregation, analysis, and presentation of HR data. It encompasses the collection and application of talent-related information to enhance key talent and business outcomes. This practice enables your organization to evaluate the impact of various HR metrics on overall business performance, fostering data-driven decision-making. Professionals in this field are primarily responsible for interpreting and analyzing extensive datasets.<br>
In parallel, utilizing a comparison of machine learning models, such as neural networks, random forests, support vectors, and logistical regression, is explored to accurately predict employee resignations(attrition) from their respective roles. This comparison aims to leverage advanced analytical tools for a more insightful understanding of workforce dynamics.<br>

## Questions
  1. What correlations suggest better retention?
  2. What prediction models can help increase the likelihood of retention?

## Slides
• [Tableau Workbook](https://public.tableau.com/app/profile/karoly.burgyan/viz/HRBook_17011060285450/AttritionAtAGlance) <br><br>
• [Presentation Slides](https://docs.google.com/presentation/d/12RUXDCDHZtxtUFoaoBHiP8SCMSqjNNB0ViUJQJipwIE/edit#slide=id.gd9c453428_0_16)

## Neural Network Model



## Random Forest Model
Random forests or random decision forests are constructed during the training phase in order to help classify the output. Random decision trees help in correcting the habit of overfitting with regular decision trees. Random forests are a way of averaging multiple deep decision trees, trained on different parts of the same training set, with the goal of reducing the variance. With n_estimators= 200 was used out of a database with 1480 records. If n_estimators is too high a number, then the model tends to become overfitted.<br>
Classification Report:<br>
<img width="500" alt="image" src="https://github.com/cburgyan/project4/assets/134640833/39fe9146-8810-4717-898b-44fd74a42837">

Confusion Matrix:<br>
 <img width="150" alt="image" src="https://github.com/cburgyan/project4/assets/134640833/2124f31b-dd7a-4bf9-aeba-a10f56a76f1e">

Feature Importances:<br>
<img width="700" alt="image" src="https://github.com/cburgyan/project4/assets/134640833/db8dbc73-0924-4100-9fb7-c6d7b897bfee">


## Support Vector Model
Support vector machines, also known as support vector networks, represent a robust form of predictive machine learning. SVM accomplishes this by mapping training data onto points in space to optimize the gap width between two categories. Subsequently, test or new data is plotted or predicted to belong to either of those two categories based on its position in relation to the gap.<br>
Classification Report:<br>
 <img width="500" alt="image" src="https://github.com/cburgyan/project4/assets/134640833/be099249-956a-48e1-8f7b-9accecf63f1c">


Confusion Matrix:<br>
 <img width="150" alt="image" src="https://github.com/cburgyan/project4/assets/134640833/9194be7b-24d2-4f43-9b9f-e11d7d4d5c51">


## Logistic Regression Model
Logistic regression assesses the likelihood of an event, such as job resignation, by considering a dataset with designated independent variables denoted as X. This technique is susceptible to overfitting, particularly in instances with a substantial number of predictor variables. To address this, a correlation table was generated to identify variables with elevated values compared to others in the dataset. This process offered insights into potential close associations with the predicted factor, attrition.<br>

Classification Report:<br>
<img width="500" alt="image" src="https://github.com/cburgyan/project4/assets/134640833/fd948fbb-3ee0-4999-8f58-2c6856e5c437">

Confusion Matrix:<br>
<img width="150" alt="image" src="https://github.com/cburgyan/project4/assets/134640833/cb699021-5ca6-4413-bdd5-842afaa55797">


# Conclusions
Both the Support Vector and Logistic Regression Models had an accuracy of 82%. The Random Forest Model had an accuracy of 83%



