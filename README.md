# diabetes_analysis

libraries:
- pandas
- numpy
- seaborn
- sklearn

# Cleaning data base:
- removing duplicated rows
- removing units in glicose
- removing rows if measurement of blood pressure, bmi etc. are equal to Nan (possible measurement error)

Before:

![download1](https://user-images.githubusercontent.com/62389300/214905425-f1674fc1-c877-450c-a0e0-8420c2edf8f0.png)


After:

![download2](https://user-images.githubusercontent.com/62389300/214905523-12a0d9a9-30ad-471f-a721-3e6efce54ae4.png)


![download3](https://user-images.githubusercontent.com/62389300/214905589-07d5cfff-109f-4122-adcd-2ec786880e90.png)

# Traning decision tree:
Repeting experiment 1000 times

![download4](https://user-images.githubusercontent.com/62389300/214907515-5fde728b-1157-461b-ae8a-deaf9ef1ce2b.png)


Decision Tree Classifier

![download6](https://user-images.githubusercontent.com/62389300/214908068-726342a8-07c2-4ca2-b08c-6450d9934c18.png)


Decision Tree Classifier with max depth = 1

![download7](https://user-images.githubusercontent.com/62389300/214908624-5d727cbf-a149-4d27-9c23-e198a784d285.png)


Best score and best parameters using cross validation

Best score: 0.7447368421052631
Best parameters: {'max_depth': 5, 'max_features': 3}

![download8](https://user-images.githubusercontent.com/62389300/214908907-701b780a-5436-4bf8-9798-7aebea0ec6c2.png)

![download9](https://user-images.githubusercontent.com/62389300/214909898-7e0ec6da-1c78-4810-9216-b6d8898676e7.png)


# Traning random forest:

Best score: 0.7760082023239919
Best parameters: {'criterion': 'entropy', 'max_features': 4, 'n_estimators': 50}
RandomForestClassifier(criterion='entropy', max_features=4, n_estimators=50)


# Traning dataset - Decision tree vs. random forest

![download10](https://user-images.githubusercontent.com/62389300/214909680-62613746-4298-4392-84ba-6beef7d92e3c.png)



