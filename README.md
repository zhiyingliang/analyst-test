#Clinical Research Unit Analyst, Test Data Worksheet.

A data file is available for your download at http://thin.med.ucalgary.ca/data/analyst-data.csv

-This file contains 300K records
-Each record has 6 variables (id, time, cats, v1, v2, v3)

Although this assessment involves the calculation of a few statistics, priorities in assessing the responses of each candidate are as follows:

-Clear, complete, repeatable, well-commented code
-Demonstration of proficiency in data summary and manipulation
-Numbers that are sensible and comparable with staff completions of the same assignment

This is contrived and randomly generated data.  We are aware that different statistical packages, approaches and personal preferences will introduce small amounts of variance in results.  This will not be held against you.  

Feel free to use different tools for each question, or take different approaches to the same question to demonstrate your diverse experiences.  Three separate reviewers will assess submissions. Scores out of 10 for each question will be summed and averaged.  The top three (of 7) candidates will be invited for a second interview to be scheduled on the afternoon of the 5th or morning of the 6th of February 2015. 

Submissions received prior to the 4th of February at noon will be considered.  All candidates will be contacted by the 5th of February with results of this assessment.

##Question 1.  

Choose your favorite scripting/programming language (there are no points for one language over another but something with statistical functionality would be advised).  Use this scripting language to download the data file and produce some descriptive statistics about the data set.

Provide summary statistics, your brief description and your script file.  You should provide everything needed to re-run your analysis with little effort.  

##Question 2.  

The variables in this file have less than informative names. Rename variables 4, 5 and 6 to normal, poisson and gauss respectively.

Provide your script file.

##Question 3.

Variable 4 (v1/normal) is comprised of samples drawn from three different normal distributions.  Stratifying by the variable named time, calculate the mean and standard deviation of each of the three distributions.

Provide summary statistics, your brief description and your script file.  You should provide everything so that we can re-run your analysis with little effort. 

##Question 4.

Variable 5 (v2/poisson) is comprised of samples drawn from a single poisson distribution, Produce a histogram of this data with lines at the X = median and X = mean.

Provide your script file and a pdf file containing your histogram.

##Question 5. 

Variable 6 (v3/gauss) is comprised of samples drawn from three normal distributions.  Using a mixed model with id (random) and cats (categorical) determine if there are significant category (cats) effects.  

Provide model summary statistics your brief assessment and your script file.


##Question 6. 

The incremental category differences calculated in question 5 should have been very close to equal.  This is because in the script that was used to generate the data, a uniform means adjustment was applied to the gauss variable based on the category value of each record.

Generate a new variable in the data set called `cru` with the following properties.  

It should be sampled from a normal distribution with an overall mean of 24 and a standard deviation of 10.

Ensure that there is a significant linear regression coefficient for the variable `time` with a value of 3 when `id` is treated as a random effect.

Submit your code, your model summary statistics and your brief interpretation.  
Take steps in your code to ensure that if I generate the same variable using your code that I get exactly the same model statistics.


