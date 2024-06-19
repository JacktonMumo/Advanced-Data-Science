# Machine Learning
## association(Apriori Algorithm)
* association is a technique used on unlabeled data for discovering frequent items or itemsets and generate association rules
* Apriori is an unsupervised algorithm under association , that helps in creating association rules from a given dataset
* it is a common algorithm used for data mining. it's used to identify the most common/frequently occuring elements and meaningful associations in a dataset
* It utilizes 3 key metrics to identify interesting relationships within a dataset:
    1. Support - indicates how popular a particular item within a group of items in a dataset is. (frequency)
    2. Confidence - goes beyond just how often items appear together. it tells you the likelihood of finding item A in a transaction, given that item B is present.
    3. Lift - it goes a step further than confidence by considering the baseline likelihood of items appearing together by chance. It compares the confidence to the expected confidence if items were independent
* breakdown of the steps for Association Apriori analysis:
    1. import libraries (mlxtend,pandas,seaborn,matplotlib)
    2. load and explore our dataset
    3. Data Cleaning
    4. Data preprocessing(optional)
    5. Apply Apriori Algorithm
    6. set association rules
    7. analyze and visualize results(optional)

* types of encoding in Machine learning - encoding categorical(qualitative) variables is a vital step in preparing ML tasks. when dealing with categorical data, characterized by non-numeric values such as text, it becomes necessary to transform them into numerical representation for compatibility with the ML algorithm
    1. One-Hot Encoding - it creates a new binary column for each categorical column/row. eg 1 or 0
    2. Frequency Encoding - this assigns numerical value to each category based on its frequenvy in the dataset
    3. Target Encoding - this one is more advanced than frequency, it encodes category based on the average value of the target variable
* Antecedents - are items that are on the left-hand side of the implication arrow(->) in an association rule
* Consequent - are items that are on the right-hand side of the implication arror(->)
* Eg. Bread(Antecedents)->Milk(Consequents)
* By analyzing the rules, you can identify interesting relationships between items. We can look for rules with:
    1. High confidence
    2. lift greater than 3 (meaning the two items probably appaer more together)

## Cohort Analysis
* it focuses on understanding the behaviour of a user over time. It involves grouping users based on shared characterisics (eg sign up date) and also it will analyze their actions within the group. This helps to identify trends and patterns in user engagement, churn (user drop-off), purchase behaviour
* in essence, cohort analysis helps to understand how a user interacts with ones products or services, while recommender systems leverage the understanding of users data to personalize user experience
* it is an unsupervised ML, but can sometimes be combined with supervised ML
* from cohort analysis we can answer questions like:
    1. user behaviour(their retention rate, purchase frequency)
    2. identifying churn points( are specific moments in a users lifecycle where they are at a heightened risk of cancelling subscriptions, stopping using a product, or otherwise disengaging from a service)
    3. how can a company improve user engagement