# Overview of the school district analysis 


For some scholar districts, It is necessary to assist their school boards and their superintendent in making decisions regarding school budgets and priorities associated. 

The purpose of this project is to generate insights into how some NaN values in some rows can affect an important part of the analysis of school budgets and priorities. 

## Data provided for the analysis

School data with the next columns are given (School ID, school_name, type, size, budget)
Student data with the next columns are given (Student ID, student_name, gender, school_name, reading_score, math_score)

## Some Metrics developed and recreated 

The district summary
The school summary
The top 5 and bottom 5 performing schools, based on the overall passing rate
The average math score for each grade level from each school
The average reading score for each grade level from each school
The scores by school spending per student, by school size, and by school type,

The recreation consists in assigning NaN to the scores of Math and Reading of the students of "Thomas High School", particularly in the ninth grade. After doing this modification we got some conclusions in every Metric. 

## Results


### How is the district summary affected?

The number of students in the district is 39,170 and the number of students with a NaN score was only 461. The students with a NaN score only represented 1.18% of the total students of the district. For that reason, some metrics of the district summary became slightly affected and some became not visibly affected. The district summary was slightly affected in the columns of Percentages Passing Reading Math and Overall.

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)


### How is the school summary affected?

The students with NaN scores represent 28.2% 
Only the school "Thomas High School" has some metrics affected:
- The Averages of Reading and Math didn't reflect a high difference because the mean was applied to over 1174 students, the students with NaN were not included in the average calculation.
- The Passing Math, Reading, and Overall have a high difference because the calculation included the students with NaN representing every NaN as a 0 score. 
With the NaN added


![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)


### How does replace the ninth graders’ math and reading scores affect "Thomas High School" performance relative to the other schools?

The relative performance is not well organized because of the wrong data of "Thomas High School"


![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)


![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

### How does replacing the ninth-grade scores affect the following:
Math and reading scores by grade are presented with a "na" string value. 


![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)


#### Scores by school spending 

The Passing Math and Reading Scores for schools with the spending ranges of $630-644 are less than they should be. The NaNs make the Passing Math percentages decrease and affect the general spending ranges of schools of the district. 

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)



#### Scores by school size
Changed the Passing percentages of Medium schools. The medium schools have 5% less overall passing with the NaNs.


![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)

#### Scores by school type
The NaNs reduce the Passing percentages for schools of type Charter. 

![This is an image](https://myoctocat.com/assets/images/base-octocat.svg)


## Summary

The most significant affectations were: 
The top 5 and bottom 5 performing schools, based on the overall passing rate
The school summary 
The average math score for each grade level for "Thomas High School" is not reflected
The average reading score for each grade level for "Thomas High School" is not reflected
The scores by school spending per student, by school size, and by school type
The district summary
