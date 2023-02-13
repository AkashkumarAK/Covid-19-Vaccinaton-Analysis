# Covid-19-Vaccinaton-Analysis
# ![image](https://user-images.githubusercontent.com/83581531/218499483-0f55f1c1-8c98-4ef2-854e-b9f1568ed2fb.png)

## Problem Statement
### Covid 19 pandemic has changed our lifestyle completely. It has caused unprecedented devastation worldwide. Moreover, 4.5 million people have died since the beginning of the pandemic, and the only acceptable way out of the disaster is to vaccinate all parts of society as early as possible. Vaccination has been shown to contribute reducing the number of cases and severe illnesses from COVID-19, But with the increase in the percentage of vaccinated population, are the number of deaths getting reduced? or can we predict with further vaccination what will be the number of deaths in the country?






## DATASET SOURCE
### https://www.kaggle.com
### https://covid19.who.int

## Data Preprocessing
### * Checking countries which are present in dataset covid but not in  dataset population. 
### * Renaming them if they are present with other name and applying the same to vaccine source dataset 
### * Data reduction(attribute subset selection)

## Final Dataset
### ![image](https://user-images.githubusercontent.com/83581531/218497469-9d5b0468-e857-476c-b924-2b6f224aeac6.png)

## Problem Analysis
### 1. WHAT WERE THE STATS OF NUMBER OF DEATHS BEFORE AND AFTER VACCINATION ?
### ![image](https://user-images.githubusercontent.com/83581531/218500179-94844cb9-c9f2-420d-a83d-2b2117976762.png)
#### * We can see from the graph the deaths were exponentially high when vaccines were not properly developed but as soon as the first vaccination dose was given, a fall in the no of deaths was observed.
#### * Also, some countries did not get early  vaccination approvals leading to an increase in the number of deaths. This also resulted in deaths from non-covid diseases like heart-attack, Alzheimer increased during surges. 
#### * Several other factors like Vaccination rates and total vaccinations in a particular country  also affect no of deaths.


### 2. ANALYSIS OF PROGRESS OF VACCINATION RATES IN DIFFERENT COUNTRIES
### ![image](https://user-images.githubusercontent.com/83581531/218500767-58c1cc85-05ff-4a67-a215-4b604fc75b4c.png)
#### *  Unlike any other country US started their vaccination process  much earlier ,but still has most no of deaths due to covid.
#### *  We observe that Italy has the maximum vaccination peak showing that the people are more responsive  towards getting their shots which in turn will reduce the no of deaths due to covid.


### 3.Q. WHAT ARE THE TRENDS OF TOTAL VACCINATIONS IN DIFFERENT COUNTRIES ?
### ![image](https://user-images.githubusercontent.com/83581531/218501509-9bbbf2b8-ef92-403b-96fe-758a8c1c4505.png)
#### * As China has high GDP so it can manufacture the required number of vaccines and followed by India which has 1.87 billion total vaccinations. 
#### * Here we also see the US though having the highest GDP still ranks 3rd in the graph which is mainly due to vaccination hesitancy of people. 
#### * In this, the total vaccination of Italy is not mentioned though having the highest vaccination peak as it has less population  having fewer total vaccinations compared to highly populated countries like the US,CHINA.


## Model Building
### ![image](https://user-images.githubusercontent.com/83581531/218502293-7b177332-492a-43ce-a984-fda91cf7de2f.png)

#### * According to our problem statement we have to predict the number of deaths based on vaccination rates of a country.

#### * To solve this problem we will use linear regression model.

#### * DEPENDENT VARIABLE :-     NEW DEATHS 	

#### * INDEPENDENT VARIABLE :-  VACCINATED POPULATION         					       PERCENTAGE 

#### * EQUATION :- 
                                    Y = M X + C
        IN OUR CASE :-  Y = NEW DEATHS 
                                  X = VACCINATED POPULATION RATIO
#### * EQUATION :-
                               NEW DEATHS=M*(RATIO) + C 
                               
                               
                               
### INFERENCES FROM MODEL:
#### * The line in red represents the regression line and the points in blue are the orignal datapoints.
 
#### * We observe a negative slope of the regression line for italy.

#### * From slope it can be said that the number of negativedeaths are decreasing with vacciantion.

#### * Intercept :- 401.44

#### * Slope :- -4.89

#### * Equation : -             
                   new deaths =(-4.89)*(ratio)+ 401.44



## Model evaluation
#### * TO MEASURE THE ACCURACY OF THE REGRESSION MODEL WE ARE USING R-squared METHOD

#### * R-SQUARED VALUE- 0.49

#### * The R-squared value of our model is 0.49. This statement means that our model explains 49% of the variance of the data corresponding to the number of articles. It is close to 1 so we can say this is not a good model.

## Conclusion
#### * From our analysis it is strongly evident that factors such as number of vaccinations and vaccination  rates affect the number of deaths.

#### * The slope of regression line is negative ,we can infer that the number of deaths are decreasing with increase in vaccination rates showing good efficiency  of vaccine .

#### * R-squared value is 0.74 which is close to 1 shows that it is a good model.  This model can be used to predict future deaths based on current vaccination rates.
#### * But the 2nd model shows R-squared value of 0.49 which shows only 49% of the variance of the data corresponding to the train data .Since it is not close to 1 so it is not a good model in this case  of the country.









                               




 









