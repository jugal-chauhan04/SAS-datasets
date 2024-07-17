# SAS-datasets
Creating SAS datasets by combining, cleaning, and validating raw datasets.  

The objective of this project is to create a dataset in SAS using multiple raw data files in different formats. Focus is on applying data cleaning and validation procedures in SAS. 

### 1. Reading RAW data into SAS.  

Let's read a small sample (shown below) of raw data into SAS.  

<img width="351" alt="2024-07-17 (2)" src="https://github.com/user-attachments/assets/d8ace4a1-7ca1-4410-9727-881d8eb6ab57">


We will read this data file into SAS using following command.  
```SAS
DATA sleep;
    INFILE '/home/u63931916/sasuser.v94/data1.dat' dlm='09'x;
    INPUT Age 
          Gender $
          Duration 
          Efficiency;
RUN;

PROC print DATA=sleep;
RUN;
```
Which will generate the following output as SAS dataset  

<img width="629" alt="2024-07-17 (1)" src="https://github.com/user-attachments/assets/97001dbd-6108-470f-a878-86ad8c533702">  




