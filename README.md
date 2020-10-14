# SalaryPrediction
### Salary Prediction Project (Python)
The goal of the project is to examine a dataset of job postings and salaries, and conduct exploratory data anlysis on the features that are likely to predict salaries for a new set of job postings leveraging on the test dataset 
#### Problem Definition
The HR department of a company need real time solution that would foster effective employment offers to potential employees.
#### Tool
The codes were wittten using Python 3 and Jupyter Notebook IDE.

### Data 
train_features.csv: Each row includes metatdata for individual job posting. The JobID is the unique identifier for each posting. 
train_salaries.csv: Each row represents a JobID and corresponding salary
test_features.csv: Just like the train_features file, each row represents metadata for individual job posting.

#### Features in Dataset
- Job Type: CEO, CFO, Manager, Janitor etc.
- Industry: Finance, Oil, Health etc.
- Degree: High School, College, Masters, Doctorate
- Major: Business, Engineering, Math, Physics etc
- Years of Experience: Candidates Years of Experience
- Miles from Metropolis: Distance from Metropolis

### Data Exploration Steps
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
  
    
