# pandas-challenge
Module 4

# Background
You are the new Chief Data Scientist for your city's school district. In this capacity, you'll be helping the school board and mayor make strategic decisions regarding future school budgets and priorities.

As a first task, you've been asked to analyze the district-wide standardized test results. You'll be given access to every student's math and reading scores, as well as various information on the schools they attend. Your task is to aggregate the data to showcase obvious trends in school performance.

# Before You Begin
1. Create a new repository for this project called pandas-challenge. Do not add this homework to an existing repository.
2. Clone the new repository to your computer.
3. Inside your local Git repository, create a folder for this homework assignment and name it PyCitySchools.
4. Add your Jupyter notebook to this folder. This will be the main script to run for analysis.
5. Push these changes to GitHub or GitLab.

# Instructions
Using Pandas and Jupyter Notebook, create a report that includes the following data. Your report must include a written description of at least two observable trends based on the data.

# District Summary
Perform the necessary calculations and then create a high-level snapshot of the district's key metrics in a DataFrame.
Include the following:
- Total number of unique schools
- Total students
- Total budget
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed math AND reading)

# School Summary
Perform the necessary calculations and then create a DataFrame that summarizes key metrics about each school.
Include the following:
- School name
- School type
- Total students
- Total school budget
- Per student budget
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed math AND reading)

# Highest-Performing Schools (by % Overall Passing)
Sort the schools by % Overall Passing in descending order and display the top 5 rows.
Save the results in a DataFrame called "top_schools".

# Lowest-Performing Schools (by % Overall Passing)
Sort the schools by % Overall Passing in ascending order and display the top 5 rows.
Save the results in a DataFrame called "bottom_schools".

# Math Scores by Grade
Perform the necessary calculations to create a DataFrame that lists the average math score for students of each grade level (9th, 10th, 11th, 12th) at each school.

# Reading Scores by Grade
Create a DataFrame that lists the average reading score for students of each grade level (9th, 10th, 11th, 12th) at each school.

# Scores by School Spending
Create a table that breaks down school performance based on average spending ranges (per student).
Use the code provided below to create four bins with reasonable cutoff values to group school spending.
<img width="611" alt="image" src="https://user-images.githubusercontent.com/127918227/234157914-59f80537-dc36-4461-83bc-2d4bb1cc8037.png">\n
Use pd.cut to categorize spending based on the bins.
Use the following code to then calculate mean scores per spending range.
<img width="677" alt="image" src="https://user-images.githubusercontent.com/127918227/234158048-24e3e913-cf86-467d-bb52-573a8d499dea.png">\n
Use the scores above to create a DataFrame called spending_summary.
Include the following metrics in the table:
- Average math score
- Average reading score
- % passing math (the percentage of students who passed math)
- % passing reading (the percentage of students who passed reading)
- % overall passing (the percentage of students who passed math AND reading)

# Scores by School Size
Use the following code to bin the per_school_summary.
<img width="676" alt="image" src="https://user-images.githubusercontent.com/127918227/234158771-9d89833a-8a85-4bd7-ae22-f224718e2c4c.png">\n
Use pd.cut on the "Total Students" column of the per_school_summary DataFrame.
Create a DataFrame called size_summary that breaks down school performance based on school size (small, medium, or large).

# Scores by School Type
Use the per_school_summary DataFrame from the previous step to create a new DataFrame called type_summary.
This new DataFrame should show school performance based on the "School Type".
