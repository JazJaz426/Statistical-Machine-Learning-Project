# Statistical-Machine-Learning-Project

This is an inter-discipline project (statistics and nutrition), which aimed to investigate the complex relationship between micronutrients and dietary fat intake with obesity and lipid metabolism. 

As one of the statistics students, a series of scientific and feasible questions were formulated through the discussion with nutrition students. The questions were later reformulated as statistical questions by statistics students and a series of models were developed and assessed based on the given Australian health data.

## 1.Statistical Questions

Given the dataset, the statistical questions and hypothese were formulated after dicussion with nutrition kids.

<img width="811" alt="Screen Shot 2020-01-23 at 7 49 33 pm" src="https://user-images.githubusercontent.com/46860162/72969417-897d0d80-3e19-11ea-9e2f-d988b1c50b7b.png">

## 2. Data
Our data was Australian Health Data and proper data cleaning was performed, which includes correction for measurement error, excluding unrelevant variables, missing value handling, creating relevant variables through self-made formulas, etc. Also, colinearity and confounding effects were investigated as well.

### Correlation Plots
<img width="685" alt="correlation plot 1" src="https://user-images.githubusercontent.com/46860162/72969141-08be1180-3e19-11ea-8954-a2d35fa53d99.png">

<img width="690" alt="correlation plot 2" src="https://user-images.githubusercontent.com/46860162/72969148-0a87d500-3e19-11ea-865b-2bcafa698e1a.png">

## 3. Models
Here we applied multiple different models. This includes logistic regression models with different penalizations, classfication tree model, Gaussian graphical model, Log-linear model, PCA, LDA and QDA. For each model, model assumptions were properly considered and limitations were carefully discussed. For all the models, we applied 10-fold cross validation.

### 3.1 Logistic Regression Models with Penalizations

Here I selected the Logistic Regression Model with Lasso Penalization as the example.

<img width="788" alt="logistic" src="https://user-images.githubusercontent.com/46860162/72969220-25f2e000-3e19-11ea-88d1-cabde3a7a412.png">

### 3.2 Classification Tree Model

<img width="710" alt="tree" src="https://user-images.githubusercontent.com/46860162/72969224-29866700-3e19-11ea-83a3-4f54ed8fad09.png">

### 3.3 Gaussian Graphical Model

<img width="634" alt="gaussian graphical" src="https://user-images.githubusercontent.com/46860162/72969249-33a86580-3e19-11ea-8a87-fe6c0f16b28e.png">

### 3.4 Log-Linear Model

<img width="561" alt="log-linear" src="https://user-images.githubusercontent.com/46860162/72969188-1a071e00-3e19-11ea-9e55-fa52e172fc58.png">

## 4. Model Result and Limitations


<img width="698" alt="accuracy" src="https://user-images.githubusercontent.com/46860162/72969180-16739700-3e19-11ea-983c-ff83ab5623c0.png">

Similarly to the other classifiers, a 20 repetitions of 10-fold cross validation was performed. For the LDA which separates the classes of BMI, there was an accuracy of 87.84%. The prediction accuracy for separating the classes of FATPER was 95.82%. The QDA which separates by FATPER yields a prediction accuracy of 79.26%. Therefore LDA would be a good classifier to make predictions on the relationship between the lipid and micronutrients variables on BMI and with FATPER. The accuracies of all classifiers is shown below in Fig 5.7.

Both assume the independent variables come from a normal distribution, i.e. multivariate normality. When considering the homoscedasticity assumption, the homogeneity of the variances of the predictors should be equal across levels of predictors for LDA. However QDA may be used when covariances are not equal. Both LDA and QDA require the number of independent variables to be less than the sample size. However it has been suggested that discriminant analysis is relatively robust to slight violations of these assumptions.

### 5. Findings and Discussion

See attached HTML file for more details.

### 6. Presentation

<img width="1016" alt="Screen Shot 2020-01-23 at 8 06 55 pm" src="https://user-images.githubusercontent.com/46860162/72970568-0c9f6300-3e1c-11ea-90a2-4e18d356e5db.png">

<img width="1024" alt="Screen Shot 2020-01-23 at 8 07 40 pm" src="https://user-images.githubusercontent.com/46860162/72970564-0b6e3600-3e1c-11ea-9a9e-a1e1c1b25e71.png">

### Team members: Anne Hu, Jiaming Lin, Pravin Radhakrishnan, Jayden Abdallah, Laura Baker, Shujie Chen, Rui Han. Probably the best team members ever!
