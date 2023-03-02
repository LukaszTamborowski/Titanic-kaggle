# Titanic Kaggle

This repositorie presents my submission in kaggle [Titanic - Machine Learning from Disaster](https://www.kaggle.com/competitions/titanic). <br>

In this competition, the <b>goal</b> is to perform a 2-label <b>classification problem</b>: predict which <b>passengers survived</b> the tragedy. <be> This competition offers two datasets. One training, where the labels are known, and one testing where the labels are unknown. The goal is to submit a file with predictions, which say whether someone survived or not. <br> All of the data, pictures and score are set in my repository.

  Here's the sample of the dataset: <br>
  
 ![Titanic Kaggle](https://github.com/LukaszTamborowski/Titanic-kaggle/blob/main/data%20view.png?raw=true) <br>
  
Columns include: 
- Variable :	Definition	: Key
  
- survival	:  Survival	:  0 = No, 1 = Yes
- pclass	:  Ticket class	: 	1 = 1st, 2 = 2nd, 3 = 3rd
- sex	: Sex	
- Age	: 	Age in years	
- sibsp		: # of siblings / spouses aboard the Titanic	
- parch		: # of parents / children aboard the Titanic	
- ticket	: 	Ticket number	
- fare	: 	Passenger fare	
- cabin		: Cabin number	
- embarked		: Port of Embarkation	: 	C = Cherbourg, Q = Queenstown, S = Southampton

  

  
  ## Analysis
  First graph presents how many males and females are in the dataset<br>
  ![Titanic Kaggle](https://github.com/LukaszTamborowski/Titanic-kaggle/blob/main/photoos/male%20female%20dash.png?raw=true)<br>
Second graph shows how many people survived or died grouped by fare<br>
   ![Titanic Kaggle](https://github.com/LukaszTamborowski/Titanic-kaggle/blob/main/photoos/Passengers%20by%20fare.png?raw=true)<br>
  Third graph shows people that are sorted by class aboard<br>
  ![Titanic Kaggle](https://github.com/LukaszTamborowski/Titanic-kaggle/blob/main/photoos/passengers%20by%20class.png?raw=true)<br>
  
  ## Missing Data
 There was a problem with missing data in age so I decided to  fill missing gaps with median age by sex. <br>
``median_age_men_2 = df_2[df_2.Sex == 1]["Age"].median()`` <br>
  ``median_age_women_2 = df_2[df_2.Sex == 0]["Age"].median()``
 
   ## Modeling

The data was split by train test split function with proportion 80% train set 20% test set
The model used for this problem was logistic regression.
Accuracy score was 0.84 and other metrics I used was confusion matrix. <br>
  ![Titanic Kaggle](https://github.com/LukaszTamborowski/Titanic-kaggle/blob/main/photoos/correlation.png?raw=true)<br>

   ## Result by module
 Here are the results on test set: <br>   
 ![Titanic Kaggle](https://github.com/LukaszTamborowski/Titanic-kaggle/blob/main/photoos/survived%20by%20module.png?raw=true) <br>
  
 ## Submission

