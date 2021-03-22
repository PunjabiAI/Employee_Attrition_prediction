# Employee-Attrition-Prediction
In this repo, I’ll introduce you to a machine learning project on employee attrition prediction with Python programming language. Employees are considered the backbone of an organization. The success or failure of the organization depends on the employees who work for an organization. Organizations must deal with the problems when trained, skilled and experienced employees leave the organization for better opportunities.
# What is Employee Attrition Prediction?
Employee attrition is downsizing in any organization where employees resign. Employees are valuable assets of any organization. It is necessary to know whether the employees are dissatisfied or whether there are other reasons for leaving their respective jobs.
Nowadays, for better opportunities, employees are eager to move from one organization to another. But if they quit their jobs unexpectedly, it can result in a huge loss for the organization. A new hire will consume money and time, and newly hired employees will also take time to make the respective organization profitable.
Retaining skilled and hardworking employees is one of the most critical challenges many organizations face. Therefore, by improving employee satisfaction and providing a desirable working environment, we can certainly reduce this problem significantly.
# Employee Attrition Prediction with Python
In this section, I will take you through a Machine Learning project on predicting Employee Attrition prediction with Python programming language.

Download the dataset from here : [HR-Employee-Attrition.csv](https://www.kaggle.com/pavansubhasht/ibm-hr-analytics-attrition-dataset/download)

let’s read the data and do some exploratory data analysis to understand this dataset properly:
# attrition = pd.read_csv('HR-Employee-Attrition.csv')

First steps in data exploration is getting a rough idea of how the features are distributed among them. To do this, I’ll use the kdeplot function in the seaborn library in Python:


![github large](https://github.com/PunjabiAI/Employee_Attrition_prediction/blob/main/Images/features_distribution.png)

The next step in a data exploration is to find the correlation matrix. By plotting a correlation matrix, we get a really good look at how the features relate to each other.


![github large](https://github.com/PunjabiAI/Employee_Attrition_prediction/blob/main/Images/correlation_plot.png)

# Observations From Above Plot:
From the correlation plot, we can see that a lot of our columns appear to be poorly correlated to each other. Generally, when building a predictive model, it would be better to train a model with features that are not too correlated with each other so that we don’t need to deal with redundant features. 

After exploring our dataset, let’s now move on to the task o feature engineering and numerically encoding the categorical values in our dataset. Feature engineering involves creating new features and relationships from the current features that we have.

# Machine Learning for Employee Attrition Prediction with Python
we need to train a Machine Learning model for predicting Employee Attrition prediction with Python. For this task, I will use the Random Forest Classification model provided by Scikit-learn.


![github large](https://github.com/PunjabiAI/Employee_Attrition_prediction/blob/main/Images/Accuracy.png)

As observed, our Random Forest returns around 88% accuracy for its predictions and at first glance, this may seem like a fairly good model.

Sklearn’s Random Forest classifier also contains a very handy attribute for analyzing feature importance which tells us which features in our dataset have received the most importance by the Random Forest algorithm. Let’s visualize the features taken into account by our machine learning model for employee attrition:


![github large](https://github.com/PunjabiAI/Employee_Attrition_prediction/blob/main/Images/feature_importance.png)

I hope you liked this article on Machine Learning project on Employee Attrition Prediction with Python programming language. Feel free to ask your valuable questions in the comments section below.
