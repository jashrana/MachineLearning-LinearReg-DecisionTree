# MachineLearning LinearReg/DecisionTree
 Machine Learning Techniques on an Iris Dataset with 2 classes using Linear Regression and Decision Tree Learning with Scikit Learn. <br> <br>
 Code files included:
 1. Working Sheet - Decision Tree Learning.ipynb
 2. Working Sheet - Logistic Regression.ipynb

## Aim
To understand:
- The basics of understanding the dataset and using respective machine learning categories,
- Using a machine learning package for a given task
- Prepare a short report demonstrating how you have applied it.


## 1. Logistic Regression: 
Logistic Regression is a classification & predictive analysis algorithm which stems from Linear Regression. It’s confusing because the name contains the term ‘Regression’, but it’s a proper classification algorithm used:
a. Categorizing labels using the dataset.
b. Converting Linear Regression problem to Logistic Regression (making classes using grouping)
In logistic regression, a logit transformation is applied to the odds—that is, the probability of success divided by the probability of failure. This is also commonly known as the log odds or the natural logarithm of odds, and this logistic function is represented by the following formulas:

$$ y = \beta_0 + \beta_1 \times X_1 + .... + \beta_n \times X_n$$

Where:
1. $X_1 ... X_n$ is the attributes/features of the data.
2. $\beta_0$ is the intercept (slope of the line).
3. $\beta_1 ... \beta_n$ are the weights associated with each attribute/feature X.


# 2. Decision Tree Learning: 
Decision Tree Learning is a Supervised Learning technique that can be used for both classification & regression but is mainly preferred for classification solutions. It is based on a tree structure, where we have a root node and there are some decisions to be made from that node to reach another node. The internal nodes represent the feature of a dataset, the branches represent the decision rules, and the leaf nodes represent the outcome.
The structure is divided into decision nodes, leaf nodes, and root node. The root node is the first node of the classifier and is also a part of the decision nodes. Decision nodes are the nodes where the decision-making process takes place while the leaf nodes provide the value or the solution of the decisions that take place. Splitting is a process where one divides the tree into sub-trees based on some given conditions. Pruning is a process of removing unwanted branches from the trees so that the tree doesn’t become complex, but not every time you can do pruning or cut down on many branches. Below is a representation of the decision trees:

There are 2 attribute selection measures associated with decision trees:
- InformationGain: It is a measurement of changes in entropy after the segmentation of a dataset based on an attribute. It calculates how much information a feature provides us about the class. Using that value, we split the nodes and build a decision tree. We formulate the information gained as:
$$Information Gain = Entropy(S) -  [Weighted Avg \times Entropy(each feature)]$$ 
Where:
   1. Entropy is $Entropy(s) = -P(yes)log2 P(yes)- P(no) log2 P(no)$.
   2. $S$ = Total number of samples
   3. $P(yes)$ = probability of yes
   4. $P(no)$ = probability of no

- <Link>Gini Impurity: Gini Impurity is the measure of purity or impurity used when creating a decision tree algorithm. An attribute with a low Gini index should be preferred compared to a high Gini index. It can only create binary splits, and so it's usually preferred with Classification and Regression Tree (CART) algorithm. The formula is as follows:
$$GiniIndex = 1 - \sum_{i=0}^{k} p_i^2$$
Where:
   1. $p$ is the probability of the given number.
   2. $k$ is the number of classes present.

---
References:
1. S. Yegulalp, “14 open source tools to make the most of machine learning,” Info World, 23 September 2020. [Online]. Available: https://www.infoworld.com/article/3575420/14-open-source-tools-to-make-the-most-of-machine-learning.html.
2. “What is Logistic Regression?,” IBM, [Online]. Available: https://www.ibm.com/topics/logistic-regression.
3. G. Choueiry, “Interpret Logistic Regression Coefficients [For Beginners],” Quantifying Health, [Online]. Available: https://quantifyinghealth.com/interpret-logistic-regression-coefficients/.
4. “Decision Tree Classification Algorithm,” Java T Point, [Online]. Available: https://www.javatpoint.com/machine-learning-decision-tree-classification-algorithm.
5. "Information Gain and Mutual Information for Machine Learning," MachineLearningMastery.com, [Online], Available: https://machinelearningmastery.com/information-gain-and-mutual-information/#:~:text=Information%20gain%20is%20the%20reduction,before%20and%20after%20a%20transformation.
6. "Gini Impurity", Learn Data Science - Tutorials, Books, Courses, and More, [Online], Available: https://www.learndatasci.com/glossary/gini-impurity/
