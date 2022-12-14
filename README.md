# Data Analysis with Python Projects

Data Analysis has been around for a long time. But up until a few years ago, developers practiced it using expensive, closed-source tools like Tableau. But recently, Python, SQL, and other open libraries have changed Data Analysis forever.

In the Data Analysis with Python Certification, you'll learn the fundamentals of data analysis with Python. By the end of this certification, you'll know how to read data from sources like CSVs and SQL, and how to use libraries like Numpy, Pandas, Matplotlib, and Seaborn to process and visualize data.

https://www.freecodecamp.org/learn/data-analysis-with-python/

There are many ways to analyze data with Python. By completing these projects, you will demonstrate that you have a good foundational knowledge of data analysis with Python.

Finish them all to claim your Data Analysis with Python certification.

## Mean-Variance-Standard Deviation Calculator

Create a function named calculate() in mean_var_std.py that uses Numpy to output the mean, variance, standard deviation, max, min, and sum of the rows, columns, and elements in a 3 x 3 matrix.

The input of the function should be a list containing 9 digits. The function should convert the list into a 3 x 3 Numpy array, and then return a dictionary containing the mean, variance, standard deviation, max, min, and sum along both axes and for the flattened matrix.

The returned dictionary should follow this format:

~~~
{
  'mean': [axis1, axis2, flattened],
  'variance': [axis1, axis2, flattened],
  'standard deviation': [axis1, axis2, flattened],
  'max': [axis1, axis2, flattened],
  'min': [axis1, axis2, flattened],
  'sum': [axis1, axis2, flattened]
}
~~~

If a list containing less than 9 elements is passed into the function, it should raise a ValueError exception with the message: "List must contain nine numbers." The values in the returned dictionary should be lists and not Numpy arrays.

For example, calculate([0,1,2,3,4,5,6,7,8]) should return:

~~~
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.6666666666666666, 0.6666666666666666, 0.6666666666666666], 6.666666666666667],
  'standard deviation': [[2.449489742783178, 2.449489742783178, 2.449489742783178], [0.816496580927726, 0.816496580927726, 0.816496580927726], 2.581988897471611],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
~~~
The unit tests for this project are in ```test_module.py```.

### Development
For development, you can use main.py to test your ``calculate()`` function. Click the "run" button and ```main.py``` will run.

### Testing
We imported the tests from ``test_module.py`` to ``main.py`` for your convenience. The tests will run automatically whenever you hit the "run" button.

### Submitting
Copy your project's URL and submit it to freeCodeCamp.

## Demographic Data Analyzer
In this challenge you must analyze demographic data using Pandas. You are given a dataset of demographic data that was extracted from the 1994 Census database. Here is a sample of what the data looks like:

```
|    |   age | workclass        |   fnlwgt | education   |   education-num | marital-status     | occupation        | relationship   | race   | sex    |   capital-gain |   capital-loss |   hours-per-week | native-country   | salary   |
|---:|------:|:-----------------|---------:|:------------|----------------:|:-------------------|:------------------|:---------------|:-------|:-------|---------------:|---------------:|-----------------:|:-----------------|:---------|
|  0 |    39 | State-gov        |    77516 | Bachelors   |              13 | Never-married      | Adm-clerical      | Not-in-family  | White  | Male   |           2174 |              0 |               40 | United-States    | <=50K    |
|  1 |    50 | Self-emp-not-inc |    83311 | Bachelors   |              13 | Married-civ-spouse | Exec-managerial   | Husband        | White  | Male   |              0 |              0 |               13 | United-States    | <=50K    |
|  2 |    38 | Private          |   215646 | HS-grad     |               9 | Divorced           | Handlers-cleaners | Not-in-family  | White  | Male   |              0 |              0 |               40 | United-States    | <=50K    |
|  3 |    53 | Private          |   234721 | 11th        |               7 | Married-civ-spouse | Handlers-cleaners | Husband        | Black  | Male   |              0 |              0 |               40 | United-States    | <=50K    |
|  4 |    28 | Private          |   338409 | Bachelors   |              13 | Married-civ-spouse | Prof-specialty    | Wife           | Black  | Female |              0 |              0 |               40 | Cuba             | <=50K    |
```
You must use Pandas to answer the following questions:

How many people of each race are represented in this dataset? This should be a Pandas series with race names as the index labels. (``race`` column)
* What is the average age of men?
* What is the percentage of people who have a Bachelor's degree?
* What percentage of people with advanced education (``Bachelors``, ``Masters``, or ``Doctorate``) make more than 50K?
* What percentage of people without advanced education make more than 50K?
* What is the minimum number of hours a person works per week?
* What percentage of the people who work the minimum number of hours per week have a salary of more than 50K?
* What country has the highest percentage of people that earn >50K and what is that percentage?
* Identify the most popular occupation for those who earn >50K in India.

Use the starter code in the file ``demographic_data_analyzer``. Update the code so all variables set to "None" are set to the appropriate calculation or code. Round all decimals to the nearest tenth.

Unit tests are written for you under ``test_module.py``.

### Development
For development, you can use ``main.py`` to test your functions. Click the "run" button and ``main.py`` will run.

### Testing
We imported the tests from ``test_module.py`` to ``main.py`` for your convenience. The tests will run automatically whenever you hit the "run" button.

### Submitting
Copy your project's URL and submit it to freeCodeCamp.

### Dataset Source
Dua, D. and Graff, C. (2019). [UCI Machine Learning Repository](http://archive.ics.uci.edu/ml). Irvine, CA: University of California, School of Information and Computer Science.

## Medical Data Visualizer
In this project, you will visualize and make calculations from medical examination data using matplotlib, seaborn, and pandas. The dataset values were collected during medical examinations.

### Data description
The rows in the dataset represent patients and the columns represent information like body measurements, results from various blood tests, and lifestyle choices. You will use the dataset to explore the relationship between cardiac disease, body measurements, blood markers, and lifestyle choices.

File name: medical_examination.csv

Feature | Variable Type | Variable | Value Type
------------- | ------------- | ------------- | -------------
Age | Objective Feature | ``age`` | int (days)
Height | Objective Feature | ``height`` | int (cm)
Weight | Objective Feature | ``weight`` | float (kg)
Gender | Objective Feature | ``gender`` | categorical code
Systolic blood pressure | Examination Feature | ``ap_hi`` | int
Diastolic blood pressure | Examination Feature | ``ap_lo`` | int
Cholesterol | Examination Feature | ``cholesterol`` | 1: normal, 2: above normal, 3: well above normal
Glucose | Examination Feature | ``gluc`` | 1: normal, 2: above normal, 3: well above normal
Smoking | Subjective Feature | ``smoke`` | binary
Alcohol intake | Subjective Feature | ``alco`` | binary
Physical activity | Subjective Feature | ``active`` | binary
Presence or absence of cardiovascular disease | Target Variable | ``cardio`` | binary

### Tasks
Create a chart similar to ``examples/Figure_1.png``, where we show the counts of good and bad outcomes for the ``cholesterol``, ``gluc``, ``alco``, ``active``, and ``smoke`` variables for patients with cardio=1 and cardio=0 in different panels.

Use the data to complete the following tasks in ``medical_data_visualizer.py``:

* Add an ``overweight`` column to the data. To determine if a person is overweight, first calculate their BMI by dividing their weight in kilograms by the square of their height in meters. If that value is > 25 then the person is overweight. Use the value 0 for NOT overweight and the value 1 for overweight.
* Normalize the data by making 0 always good and 1 always bad. If the value of ``cholesterol`` or ``gluc`` is 1, make the value 0. If the value is more than 1, make the value 1.
* Convert the data into long format and create a chart that shows the value counts of the categorical features using seaborn's ``catplot()``. The dataset should be split by 'Cardio' so there is one chart for each ``cardio`` value. The chart should look like ``examples/Figure_1.png``.
* Clean the data. Filter out the following patient segments that represent incorrect data:
  * diastolic pressure is higher than systolic (Keep the correct data with ``(df['ap_lo'] <= df['ap_hi'])``)
  * height is less than the 2.5th percentile (Keep the correct data with ``(df['height'] >= df['height'].quantile(0.025))``)
  * height is more than the 97.5th percentile
  * weight is less than the 2.5th percentile
  * weight is more than the 97.5th percentile
* Create a correlation matrix using the dataset. Plot the correlation matrix using seaborn's ``heatmap()``. Mask the upper triangle. The chart should look like ``examples/Figure_2.png``.
Any time a variable is set to ``None``, make sure to set it to the correct code.

Unit tests are written for you under ``test_module.py``.

### Development
For development, you can use ``main.py`` to test your functions. Click the "run" button and main.py will run.

### Testing
We imported the tests from ``test_module.py`` to ``main.py`` for your convenience. The tests will run automatically whenever you hit the "run" button.

### Submitting
Copy your project's URL and submit it to freeCodeCamp.

## Page View Time Series Visualizer
## Sea Level Predictor
