# SalaryPrediction
### Salary Prediction Project (Python)
The goal of the project is to examine a dataset of job postings and salaries, and conduct exploratory data anlysis on the features that are likely to predict salaries for a new set of job postings leveraging on the test dataset 
#### Problem Definition
The HR department of a company need real time solution that would foster effective employment offers to potential employees.
#### Tool
The codes were wittten using Python 3 and Jupyter Notebook IDE.

### Data 
- train_features.csv: Each row includes metatdata for individual job posting. The JobID is the unique identifier for each posting. 
- train_salaries.csv: Each row represents a JobID and corresponding salary
- test_features.csv: Just like the train_features file, each row represents metadata for individual job posting.

#### Features in Dataset
- Job Type: CEO, CFO, Manager, Janitor etc.
- Industry: Finance, Oil, Health etc.
- Degree: High School, College, Masters, Doctorate
- Major: Business, Engineering, Math, Physics etc
- Years of Experience: Candidates Years of Experience
- Miles from Metropolis: Distance from Metropolis

### Data Discovery Steps
- Import Data Libraries and set up directory
- Load Data
- Merge train_features and train_salaries dataset as one that includes:
    -  1 million rows and 9 features
    - Both categorical and numeric features
- Clean Data
    - Rename Columns
    - No duplicates and null values in dataset
    - Dropped 5 rows where Salary is less than or equal to 0
 - Explore Features using Data Visualization
    - Use IQR to detect/confirm outliers
 - Utilize Correlation Matrix to examine relationships between variables
 - Use label encoding to identify correlation between all features 
  
  ## Data Exploration
  
  ### Univariate Plots
  - Job Type
  
  ![JobType](https://user-images.githubusercontent.com/66134645/95991525-de731080-0dfa-11eb-9970-4d8ccda2c1e1.png)

- Industry 

![Industry](https://user-images.githubusercontent.com/66134645/95992054-84267f80-0dfb-11eb-84b1-7b8f42a99006.png)

- Degree

![Degree](https://user-images.githubusercontent.com/66134645/95992071-8d175100-0dfb-11eb-9b27-506b8c6dc85e.png)

- Major

![Major](https://user-images.githubusercontent.com/66134645/95992124-999ba980-0dfb-11eb-81f2-d3e588a12ac1.png)

### Insights
- Job Type: All job types roughly have a similar count
- Industry: All industries roughly have a similar count
- Degree: Employees with High school and 'None' degrees have the highest count when compared to    other groups. The count of employees with Bachelors, Masters and Doctoral degree are roughly similar.
- Major : Employees with no major are the most popular when compared with other employees. The counts of other majors are roughly the similar



#### Salary (Target Feature)


![Boxplot](https://user-images.githubusercontent.com/66134645/95992198-b0da9700-0dfb-11eb-88f8-de28d08f2e47.png)

![Hist](https://user-images.githubusercontent.com/66134645/95992207-b46e1e00-0dfb-11eb-8311-af58dd58c396.png)

### Insights:

- The boxplot indicates the median salary is about 120k and about 75% of employees earn about 85k and more.
- The histogram shows the highest salary point is at about 130k. The histogram is almost a normal distribution except it is slightly right skewed.
- Both plots indicate some outliers which could potentially be salaries of the top management such as the CEOs.



### Bivariate Plots

![jobtype boxplot](https://user-images.githubusercontent.com/66134645/95995522-92769a80-0dff-11eb-9258-0062b32bb0dd.png)

![insdutry-boxplot](https://user-images.githubusercontent.com/66134645/95995541-9b676c00-0dff-11eb-8c4e-424c92365241.png)

![Boxplot Degree](https://user-images.githubusercontent.com/66134645/95995636-c2be3900-0dff-11eb-8251-08470ed5d26f.png)

![boxplot major](https://user-images.githubusercontent.com/66134645/95995569-a4583d80-0dff-11eb-8917-30dcceb80aa8.png)

![years of experience](https://user-images.githubusercontent.com/66134645/95995672-d073be80-0dff-11eb-8fb9-d0057e826a1f.png)

![miles from metro](https://user-images.githubusercontent.com/66134645/95995658-ca7ddd80-0dff-11eb-8671-dd92fb94cc7e.png)

### Insights 

- Job Type: The box plot shows the CEO's has the highest salary followed colsely by the salaries of the CFO's, and  CTO's. The Janitor earns the least salary when compared to other employees.
- Industry: The highest earning industries as displayed by the box plot are the Finance and Oil industries while the least two earning industries are the Education and Service sectors. 
- Degree: Employees with high school or no degrees tend to earn lower salaries when compared to other degrees
- Major: The employees who majored in Engineering and Business earn slightly higher than other majors in exception of those with 'none' major. Employees with no major earn the least salaries.
- Years of Experience: The plot shows that as employees years of experience increase, their salaries increases as well and vice-versa.
- Miles from Metropolis: The plot shows thatas  employees miles from metropolis increases, their salaries decreases and vice-versa.  



### Correlation Matrix

![correlation matrix](https://user-images.githubusercontent.com/66134645/95995689-d49fdc00-0dff-11eb-90e8-3340a68e8cce.png)

### Insights
- There is a positive relationship between Salary and Years of Experience.
- There is a negative relationship between Salary and theses features :Miles from Metropolis, Major and Degree
- Also, there is positive correlation between Major and Degree

### Conclusion
Based on the output of the correlation, there is indication that when years of experience increases, salaries of employees seems to increase, that is employees with longer years of work experience are more likely to earn high salaries

Also, there is an indication that when salary increases, miles from metropolis decreases.This could be that employees who earn high income are more likely to afford homes and other expenses of living in or close to the Metropolis.




