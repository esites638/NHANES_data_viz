# NHANES_data_viz
Final project for CS10 - interactive data analysis tool using NHANES data. 

## Features: 

Feature 1: takes as input user's reported gender, age, and height, and outputs average weight for individuals of the same same gender and age, and height within .05 meters. Also produces boxplot that displays users weight against distribution of all body weights in the dataset. 

Feature 2: Visualizing how physical activity rates tend to change with age for people with similar characteristics as user. Takes as input user's reported gender, weight, and height, and returns 1 boxplot of total minutes of moderate to vigorous physical activity per day per age category for observations of same gender, weight within 6 kg and height within .05 meters as user. 

Feature 3: data analysis to explore the relationship between BMI and demographic characteristics. A visualization (box plots and regression plot) and quantification (through linear regression) of the effect of income (relative to the Federal Poverty Level) on body mass index. 

## Lists and local variables 
Lists - The three dataframes used in this project are all lists of equal-length lists. Further, we used a list() function to create a list of all variables in our merged dataset. See (‘#reading in datasets’ code section towards top of file). 

Script/local variables - all of the functions we defined (average_weight(), exercise_over_time(), exercise_income_level()) make use of script variables. In each function a new script variable is created which is set to a narrowed-down dataframe, consisting only of the observations with characteristics that match the user’s input. For example, with the inputs ‘female’, ‘26’, and ‘1.549’ , a script variable within average_weight() called “female” is set to a subset of the original dataframe in which all observations are female, 26, and +/- .05 meters of 1.549m. 

## Function Names, domains, ranges, and behaviors: 

average_weight()
Age: integer
Height: integer/float
Gender: string (either female or male)
integer/float
takes as input user's gender, age, and height, and reports average weight for individuals of the gender and age, and height within .05 meters


exercise_over_time()
Gender: string(either male or female)
Weight: int/float
Height: int/float
boxplot
returns 1 boxplot of total minutes exercise per age category for observations of same gender, weight within 6 kg and height within .05 meters as user


exercise_income_level()
Gender: string (either female or male)
Age: integer
boxplot
Returns 1 boxplot of total minutes exercise (MVPA) per category of income:poverty level ratio for observations of same gender and age as user

## Additional information

Written in Python 3.6.7

Python packages:
Numpy
Pandas
Matplotlib
Seaborn
Statsmodels

The project was made using google colab, and imports data from three different files. We have saved the google colab project as an ipython notebook and have included the 3 files the code needs to reference. Running this code elsewhere will require modifications to the data importing section. 





