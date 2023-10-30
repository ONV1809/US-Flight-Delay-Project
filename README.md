# US-Flight-Delay-Project
---
Project on US domestic flights in the year 2006. Notebooks contain Exploratory data analysis and workflows for creating models for predicting the extent of a given flight's arrival delay.
The main data source used in this project can be found at: https://www.kaggle.com/datasets/bulter22/airline-data
- The file is approximately 5GB, so may take a while to download.

## OVERVIEW + STRUCTURE
---
This project is made up of 3 main Jupyter Notebooks titled:
- Delay Prediction1 - EDA.ipynb
- Delay Prediction2 (without DEPDELAY)- ML.ipynb
- Delay Prediction3 (with DEPDELAY) - ML.ipynb

The focus of Delay Prediction1 was to understand the dataset (US Domestic Flights - 2006) that we were working with through exploratory data analysis. We wanted to understand the various factors that affected flight delays, whilst also collecting data from external sources so that we could attempt to explain more of the variance and aid our models in future notebooks. This notebook also contained visualizations and statistics that help provide an insight into the relationship between variables, and thus, the nature of the problem.

The main focus of this project was to predict the arrival delay of domestic flights in the US in the year 2006. 2 prediction models were created. One with "Departure Delay" as a feature and one without. The 2nd Jupyter Notebook contains the model that did not include the feature which held 'future information', in this case, 'DepDelay'(Departure Delay (mins)). This model would be useful to consumers/businesses who would like to be able to predict delays weeks, months, or even years in advance.

The final Jupyter Notebook shows the workflow for developing a model that included this 'future information'.Departure Delay was referred to as future information as it is impossible to know how much a plane's departure has been delayed until it has actually taken off from the airport runway. This model would be of use to passengers/families of passengers/businesses who are waiting for a delayed flight and would like to more accurately predict the landing time, so that adjustments to travel, collection time or itineraries could be made.

## Skills Demonstrated in each Jupyter Notebook
---

## EDA Notebook
- Creating and uploading data to a SQLite Database.
- Querying a SQLite Database.
- Pandas DataFrame Manipulation (Feature Engineering, .apply/map function).
- Merging data from external data sources (inner joins).
- Working with datetime data types.
- Defining custom functions.
- Dealing with missing values.
- Machine Learning Pre-Processing
- Data visualisations for insights.
- Using visualisations to derive Machine Learning insights.
- Conducting Exploratory Data Analysis.
  
## Machine Learning Notebooks 
- Further Feature Engineering.
- Feature Selection for modeling.
- Splitting Data into train and test splits.
- Dealing with skewed variables.
- Dealing with uneven scales within variables.
- Creating Dummy variables for categorical variables.
- Training Classification models.
- Testing  variety of models on test data.
- Assessing models with Accuracy, Precision, Recall, and F1-Score.
- Tuning model via hyper-parameter tuning in GridSearchCV.
- Conducting Feature importance with Random Forests.


## Other files in the repo
---
- Within the repo, you can find files such as "100000flights", which is a subset of 100000 flights if you would like to work with a subset of data.
- In my project, I worked only with flights that were not diverted or cancelled. The diverted_cancelled.csv allows others to take on a complete project based around whether a flight was diverted or canceled.
- airports, runways, and carriers are data sources that I merged to the original data source in order to extract new insights
- pre-processed flight delay data x5000.csv is a file with data (5000 entries) pre-processed, in case you cannot train models on your machine, for whatever reason.
- Pickled Files containing the various models I developed can be found in the 'Models' folder.

## DEPENDENCIES
---
This Project was written in Python (VS Code using Jupyter Notebooks). A range of libraries were used throughout the development of this project. These included:
-Numpy
-Pandas
-Matplotlib
-Seaborn
-Scikit-learn

Please refer to the "requirements-flight.txt" file for a full list of all libraries used throughout this project.

## USAGE
---
If you would like to run this project yourself, please do the following:
- Clone this repository
- Make sure you have all the correct packages + their versions installed. This can be done by running 'pip install -r requirements.txt' in your command line.
- Now you can open each of the Jupyter Notebooks and run the cells in order.

## FUTURE WORK
---
There are multiple areas in which this project could be expanded upon. This includes but is not limited to:
- Finding and adding new data sources to improve the accuracy of the models. For example, the weather conditions at each airport at time of takeoff/landing.
- Using more advanced machine learning, models/ensemble methods to improve prediction accuracy.
- In the Jupyter Notebooks above, models were only trained on small subsets of the 7,000,000 flights that occurred in 2006. If someone has access to larger amounts of computational power, model accuracy could be improved by using larger subsets of the dataset.
- Random Forest Feature importance was used in this project. More advanced feature importance methods could be used to help aid airlines/airports determine their weak/strong points.
- Due to the high dimensionality of the data, Principal Component Analysis could potentially improve the accuracy of our models.

## CONCLUSION
---
This project is a deep dive into predicting flight delays for US domestic flights in 2006. It contains a complete data analysis workflow, starting with EDA, moving to model creation, evaluation and comparison.

## CONTACT DETAILS
---
If you have any questions or suggestions, feel free to reach out. Contributions to this project are welcomed.


