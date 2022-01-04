# KaggleSurvey-Income-Education
**Objective:**
- Analyze based on survey dataset from 2020 “Kaggle ML & DS Survey Challenge.”
- Understand nature of women’s representation in Data Science and Machine Learning.
- Examine the effects of education on income level.

**Attachments:**
- **clean_kaggle_data.csv:** Input dataset based on the survey in **kaggle_survey_2020_answer_choices.pdf**
- **kagglesurvey_income_education.ipynb:** IPython Notebook detailing the analysis performed

**Process:**
- Exploratory data analysis to summarize characteristics
- Descriptive statistics
- Two-sample t-test
- Bootstrap data for comparing the mean
- ANOVA test to compare the means of salary for three groups

**Findings:**
- (Gender related) Male participants of the survey has more considerable income. If mainly compare the salary levels of man and woman, the median salary of man is evidently higher than the median salary of woman. Also, the upper whisker of man’s salary has wider range and higher salary than the one of woman’s.
![alt text](https://github.com/elenayinyin/KaggleSurvey-Income-Education/blob/main/Compensation_between_Man_Woman.png)

- (Education related) Explore the relation between amount of money spent on machine learning and/or cloud computing services (Q25) and different education levels. The master’s degree turns out highly willing to spend any money on computing services, even more likely to pay than doctoral degree.

- (Gender related) After bootstrapping 1000 replications of data for each gender, take the two-sample t-test for woman’s and man’s salary. The p-value indicates that mean salary of man is different from mean salary of woman.

- (Education related) After bootstrapping 1000 replications of data for each of Bachelor's, Master's, and Doctoral degree, take one-way ANOVA to compare variances between 3 populations’ mean salary. We concluded that at least one pair of salary means is different from each other.
