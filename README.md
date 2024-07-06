# Introduction
I am Ayush Raj, currently pursuing a B.Tech at IIT Patna. I have a strong foundation in machine learning, deep learning, and data structures and algorithms (DSA). My passion for competitive programming has driven me to solve over 1500 problems on platforms such as [Codeforces](https://codeforces.com/profile/ayush_raj14), [CodeChef](https://www.codechef.com/users/ayush_raj14), and [LeetCode](https://leetcode.com/u/ayush_raj_14/).

## AspireNex Machine Learining Internship

#### TASK 1 - CREDIT CARD FRAUD DETECTION

#### About data

*   Data contains 284807 rows and 31 columns.
*   Data does not have any null values.
*   Data['Class'] value counts is very unbalanced.
    *   99.8% value is 0 and 0.2% value is 1.

I trained LogisticRegression model on given data which given an accuracy of 0.9991398, This is case of overfitting which is obviously expected due to data imbalance.

<span style="color:green">

### Imbalance dataset
</span>

To deal with this problem, we have to modify the data.
*   UnderSampling the oversampled data.
*   OverSampling the undersampled data.

I have undersampled the 0's data such that overfitting can be reduced.

Now, again i trained my LogisticRegression model with newly created data then i achived accuracy of 98%.



#### TASK 3 - CUSTOMER CHURN PREDICTION

##### About Data

*   Data have 7000+ rows and 21 columns
*   Data does not contains any null values
*   Data need manipultaion, many columns dtype is objects.

#### Cleaning and converting data
*   There is some space as a value in `TotalCharges` columns which i have removed.
*   Replced `Yes` with 1 and `No` with 0 every where.
*  `pd.get_dummies`  on few columns like `PaymentMethod` , `Contract` , `InternetService`.

StandardScaler to scale our data.

### Training

*   Trained this data to three different model `RandomForestClassifier` , `LogisticRegression` and `GradientBoost`.
*   Best performing model was LogisticRegression with accuracy of 80.74%
*   plotted bar chart of accuracy of all models, Confusion matrix and Classification report.