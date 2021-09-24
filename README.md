# Embr. test data
An organization has collected data from individuals seeking their services related to mental health support. The data is in xlxs format with 2 sheets (check file preview and description in the repository). This project will consist of conducting a light EDA (i.e. Exploratory Analysis), and joining data from sheets as necessary to answer raised questions. 

## Questions 

#### Question 1
what percentages of "seen" (i.e. completed) appointments were in March for minors seen by psychatrists?
Answer: An approximate 3% of the total sample (patients who attended) represents minors (i.e. The legislative texts in Lebanon are in conformity with the stipulation of article 1 of the Convention on the Rights of the Child, in which a child is defined as every human being below the age of 18) - more details in Questions_Answers.ipynb notebook in the repository.

___

#### Question 2
For patients who attended more than 1 session, what was the average percentage change in phq9 scores? is there a difference in percentages variation between patients who saw 1 type of practitioner and those who did not?

Answer: The average percentage change for the sample (patients who attented more than once) is with a 95% confidence at a 47% average between 47.34 and 47.73 - more details in Questions_Answers.ipynb notebook in the repository.

The sampling distribution of the samples' (resampled) mean is visualized below in the image.

![Percentage change sampling distribution](Visualization/sampling_all.png)


Is there a difference between percentage change average of patient who saw same type of practitioner and those who did not?

The sample as a whole is below 30 entries, it is not recommended to run parameteric statistical tests when various assumptions related to those satistical tests are violated (we could have simply performed on the 2 samples a t-test for difference in means; However sample size is crippling and Heteroscedacity adding to that violation of distribution normality). Nevertheless, the conditions are best suited to perform a Bootstrapping on both sample and produce a sampling distribution.

The sampling distribution of the samples' -of patients who saw same type of practitioner- mean is visualized below in the image.

![Percentage change sampling distribution for the sample of patient who saw same practitioners](Visualization/sampling_same.png)


The sampling distribution of the samples' -of patients who saw different type of practitioner- mean is visualized below in the image.

![Percentage change sampling distribution for the sample of patient who saw different practitioners](Visualization/sampling_different.png)


As obvious the 2 sampling distribution's mean C.I does not overlap which is a clear indication that the 2 sample means are in deed diffirent and not just due to randomness in the data. In other words people 







