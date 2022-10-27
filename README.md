# Tanzania_water_wells_project

## BUSINESS UNDERSTANDING

### Overview:

We are working on a project to point the Tanzanian clean water problem. Recent data from the World Bank show that Tanzania has a population of about 60 million. According to Nsemwa (2022) many Tanzanians continue to struggle with insufficient or limited access to clean and safe water. Only 30.6% of Tanzanian households use recommended water treatment methods, and only 22.8% have adequate hand-washing facilities (Ministry of Health report, 2019). Poor sanitation is estimated to cause 432,000 diarrhea-related deaths per year and is a major contributor to several Neglected Tropical Diseases (NTDs) such as intestinal worms, schistosomiasis, and trachoma. Malnutrition is also made worse by poor sanitation (WHO, 2019).



### Problem:

Tanzania is the largest country of East-Africa with 59,353,795 population according to worldometers.info. 25 million of this population have lacks access to clean water, 40 million people also have a lack access to improved sanitation. Water is a basic need and for human beings. The Tanzanian Water Ministry aimed to solve this problem by improving clean water sources. There are many water wells already established, but some of them are non-functional or needs repair.

### Goal:

Our goal in this project is to build a model that predicts the functionality of water points. With this predictive model, authorities can understand which water points are functional, nonfunctional, and functional but it needs to repair. This model can help the Tanzanian government to find likely maintenance needy wells or give useful information for future wells. With this model, we can help the Tanzanian authorities how to use water sources in a productive way. It also helps the investment of the government on wells.


### Metric: 

The metric is an accuracy score of 70%

## DATA UNDERSTANDSING

### Data:

The original data was obtained from the DrivenData 'Pump it Up: Data Mining the Water Table' competition. Basically, there are 4 different data sets; submission format, training set, test set and train labels set which contains status of wells. With given training set and labels set, competitors are wanted to build predictive model and apply it to test set to determine status of the wells and submit.
In this project, we used train set and train label set which have 59400 water points data with 40 features.

### Plan:

Understanding Data

Cleaning and Exploring Data

Preparing Data to Modeling

Finding Binary Model & Baseline

Ternary Target Modeling

### Understanding Data: 

We realized two main challanges in this dataset. Firstly, columns in this data are mostly categorical columns with many unique values with is not understandable for machines. The first challange is to solve this problem. Second challenge is to handle with highly imbalanced multi-target problem. We understood these two challanges with the understanding of data.

### Cleaning and Exploring Data:

Mainly, null, zero and missing values changed to mean.

Preparing Data to Modeling: 

To prepare our data to machine learning, we did some feature engineering, encoding and scaling.

### Findings:

Authorties should check again the wells which they funded.

The most common extraction type is gravity but second is hand pumps. The quality of handpumps are less than comumunal pumps. It shows that authorities need to focus on pumping type. It is seen that, there are many non-functional water points which belongs to gravity which is natural force so no need to do anything expensive as extraction type.

New tecqniques must be found to feed dry wells and repair wells.

More detailed finding can be found in notebooks with explorations.

### Future Improvements:

Feature engineering on categorical columns will be good idea to handle first challange.

Imbalanced target problem will be solved in more effective way.

Parameter optimization will be improved for XGBoost Model to fix overfitting problem.

Wells can be monitored well and model can be improved according to more accurate and recent data.

Different regions have different factors like climate, rainfall season etc. So, from the main model, different models can be build for each region.
