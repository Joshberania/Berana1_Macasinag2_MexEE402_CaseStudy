# MexEE 402: Data Preprocessing Case Study

MexEE Elective 2: Data Science and Machine Learning
Batangas State University, Alangilan Campus
1st Semester, AY 2026-2027

## Members

| Name | Student Number | Section |
|---|---|---|
| Beraña, Steven Josh | 23-07634 | MEXE-4101 |
| Macasinag, Criz Glenn | 23-05117 | MEXE-4101 |

## Notebook links

| Chapter | Member 1 |
|---|---|
| Ch1_2_3 | [Ch123_Beraña1_Macasinag2](https://colab.research.google.com/drive/1ZWOe3By0EzK4fIKFydX928dIxllaUnd4) | 
| Ch4 | [Ch4_Beraña1_Macasinag2](https://colab.research.google.com/drive/1X3GiSw0jUyUAyAQi-d8-Ht1i9ZtO37Vi?usp=sharing) |
| Ch5 | [Ch5_Beraña1_Macasinag2](https://colab.research.google.com/drive/1tfqVGZ3L-yWI-vSmy-df330puJ14Plze) |
| Ch6 | [Ch6_Beraña1_Macasinag2](https://colab.research.google.com/drive/1EMIP1ZZeRbOJarXuNgfZwZzGIFRlvH1K?usp=sharing) | 
| Ch7 | [Ch7_Beraña1_Macasinag2](https://colab.research.google.com/drive/1xyjBISRdZVOgmuzdvVLYhZIHOTsbHM5y?usp=sharing) | 
| Ch8 | [Ch8_Beraña1_Macasinag2](https://colab.research.google.com/drive/1evGI-SsRzWw7pIdAMUoGTc-zAZWOQ4XI?usp=sharing) | 
| Ch9 | [Ch9_Beraña1_Macasinag2](https://colab.research.google.com/drive/1e12_CJ8VMdyE6Gxn75ngjVrb6ef7HniK?usp=sharing) |

## What we learned

One short paragraph per chapter, Ch1_2_3 to Ch9. Say what the chapter taught
you and what surprised you. Not what the library does, but what you understood.

| Chapter | Learnings |
|---|---|
| Ch1_2_3 | <p align="justify"> In these three chapters, we learned a lot beyond programming, especially about what we need to know first before proceeding to the next steps. As for Chapter 1, we were immediately introduced to the idea that not all raw data is ready for analysis. We cannot simply create a program and run it right away. Each dataset needs to go through preprocessing first, where the data is prepared before proceeding to machine learning. We were not surprised but rather expected that missing or inconsistent values could possibly cause messy results later on, which we have already experienced before in subjects where we dealt with programming. In Chapter 2, we realized that each data type in every column is important, which is interconnected with the previous chapter because this is where we started to encounter data processing and how the data is handled. We were surprised that we needed to distinguish between `object`, `int64`, and `float64` to determine what operation should be applied first before proceeding to the next step. Lastly, in Chapter 3, we learned that simply deleting missing values is not always the automatic solution when encountering them. We only learned now that there are different approaches to handling missing values, such as imputation, deletion, and prediction. This also helped us become more careful about looking closely at the program before making a risky solution, since we could either spend a long time troubleshooting to find the problem again or even have to repeat everything from the beginning. Overall, the questions helped us understand each process better, rather than simply copying the program, because they helped us connect the dots that seemed overwhelming at first. As time goes by, we become more engaged in programming without even noticing how many steps actually need to be followed. </p> |
| Ch4 | <p align="justify"> We felt that the process was becoming more understandable compared to the previous chapters because we were starting to see how the data is being prepared step by step before it can actually be used. Compared to Chapters 1 to 3, it seems that we're more focused on understanding the raw data, its different types, and how to handle missing values. However, in this chapter, we learned that converting categorical data into numerical values is not as simple as just assigning numbers to each category. In addition, we learned that the type of category matters because it determines what kind of encoding should be applied. At first, we thought that assigning numbers would already be enough, but we realized that doing so could create an unnecessary ranking between categories that do not actually have one. For example, Little, Medium, and Lots can be assigned numerical values because they have a natural order, while Sunny, Cloudy, and Rainy need a different approach because none of them is necessarily higher or lower than the others. This made us realize that even a simple step like converting data into numbers still requires us to understand the meaning and relationship of the categories first. Overall, this chapter helped us become more careful in handling categorical data because the way we encode it can affect how the machine learning model understands the information. </p> |
| Ch5 | <p align="justify"> In this chapter, we learned that preparing data does not stop after cleaning missing values and identifying the types of data. Compared to the previous chapters, the process in this chapter was shorter and more straightforward because we mainly focused on scaling the values of the features. We learned that the range of values matters because a variable with much larger numbers may have more influence on a machine learning model. At first, we thought that it would not matter as long as the data was correct, but we realized why scaling is used to put different features on a more comparable scale. We also learned that StandardScaler and MinMaxScaler work differently, but both can help make the features easier to compare. Overall, this chapter helped us understand that even a simple step like scaling can affect how a machine learning model handles different features. </p> |
| Ch6 | <p align="justify"> We learned that outlier has a value of its own and far from the rest just like the 100 among the numbers between 10 to 22, where it can mess up the results and give a wrong picture of the data. We also learned that Z-score and IQR are two ways to find outliers, and finding one is not the end of the process. We also learned what to do with an outlier depending on the situation, if it is a mistake we can just remove it, but if it is a real value that is just very high then it is better to just limit or shrink it so we do not lose information. </p>|
| Ch7 | <p align="justify"> For this chapter, it tought us that the feature selection is about deciding which information actually helps a model to predict. In this chapter we identify the three methods for feature selection which is the filter, wrapper, and embedded methods where in each of them chose a different set of features from the same data, and with that,  only study hours and class participation were chosen by all three. We also learned that in this chapter, the extracuriculllar activities will be dropped by the filter because of its low correlation with final grade but still will be kept by Lasso. </p>|
| Ch8 | <p align="justify"> This chapter tought us that preprocessing is not just for fixing but it is also a process that works best when the steps are chained together in a pipeline just like in the example prvided and used which is related to the conveyor belt concept so that the exact same steps will run smoothly at the same order every time. What surprised us but not actually surprised us is the ColumnTransfer, because it quietly drops every column we don't name, so the final result will be only AGE and FARE instead of the whole dataset. We also realized that the order of the steps matter like filling the blanks must happen before scaling or else the scaler will not work since it has an uncomplete data. </p>|
| Ch9 | <p align="justify"> As for the chapter 9, it correlates with the all the chapter since we again learned all of it but this time we applied them from one messy datasets into a much cleaner one. Missing values were filled in, numbers were scaled, categories is converted into numbers with one-hot encoding, Age was grouped into life stages, and all of it was chained into a pipeline with a ColumnTransformer. We also used correlation to see how the columns relate to each other. What we learned is that these techniques are not just separate lessons since in reality they are used together as a one workflow, and the order of the steps matters. </p> |


## Errors we found

List any mistake you found in the original notebooks, and the correct version.
There are real ones in there. Finding them earns points.

| Chapter | Errors |
|---|---|
| Ch1_2_3 | <p align="justify"> So far, none of the programs crashed during the programming activities, but a warning appeared in Step 3, specifically during imputation. It indicated that using inplace=True on the Year and Publisher columns may no longer be valid in future versions of pandas. We corrected it by assigning the result of fillna() directly back to each column. Therefore, the corrected version is df['Year'] = df['Year'].fillna(df['Year'].mean()) and df['Publisher'] = df['Publisher'].fillna(df['Publisher'].mode()[0]). Moreover, we also noticed another issue, although it was not a major one, which was the confusion between the Chapter Questions and what was presented in Chapter 3 of the notebook. Only two methods were implemented in the code, which were imputation and deletion, while prediction was only discussed and not implemented. This was not a programming error, but rather an inconsistency in the instruction or question that might lead to confusion. Lastly, we encountered an issue where the vgsales.csv file was no longer available when we continued working on the notebook. To prevent the file from being lost again, we decided to mount our Google Drive and access the CSV file from there instead of relying on the temporary notebook storage. This helped us keep the dataset available even when the notebook session was restarted. </p> |
| Ch4 | <p align="justify"> In this chapter, we only encountered a small error while Mr. Beraña was manually typing the provided code instead of copying and pasting it directly into our Google Colab. He accidentally missed typing the colon (:) after the Lemonade Sold variable, which caused a syntax error when we tried to run the program. We were able to identify the problem by checking the code and comparing it with the provided version, then corrected it by adding the missing colon. Overall, this human error reminded us to be more careful, especially when inputting code, and to run the program from time to time so we can immediately identify and correct any errors. </p> |
| Ch5 | <p align="justify"> In this chapter, we did not encounter any major programming errors or warnings while running the code. The programs for StandardScaler and MinMaxScaler ran successfully and produced the expected results. We only had to make sure that we understood what happened to the values after scaling, since the numbers changed but their purpose was to put the features on a comparable scale. Overall, there were no significant errors that needed to be corrected in this chapter. </p> |
| Ch6 | <p align="justify"> We noticed from this chapter is that the z-score of 100 is about 2.6 which is lower than the cutoff which is 3, so the code that we needed to do is instead of >3 we changed it into >2. </p>|
| Ch7 | <p align="justify"> For this chapter we only encountered one error but not exactly an error since the program still runs but shows some flow which while using cv >= 4 on the 7-row dataset, some test folds contain only one row, so R² cannot be computed and scikit-learn repeatedly raises an UndefinedMetricWarning. The code still runs, but the cross-validated scores are invalid, and the selection changed from all four features (cv=2) to only assignments completed. </p>|
| Ch8 | <p align="justify"> On this chapter, we dont encounter error or warnings since all cells ran successfully from uploading and loading the datasets, to splitting it into features such as X and Y, to building the pipeline and applying it. </p>|
| Ch9 | As for this chapter, we did not actually encounter a visible error from the program but the “before discretization” histogram actually displayed the binned Age values which is the Adult, Elderly, and Child. And the “after discretization” histogram plotted titanic_preprocessed[:, 2], which is the Embarked_C column, not Age. </p>|

## Note on AI tools

Say whether you used an AI tool, and what for. This is not a penalty.
Hiding it is.

| Chapter | Justification on AI Tool Usage |
|---|---|
| Ch1_2_3 | <p align="justify"> Throughout these chapters, we admit that we used AI, but we mainly used it as a guide instead of relying too much on it. Our use of AI was similar to what we discussed in Chapter 1, where our initial answers were like raw data. They could contain mistakes, inconsistencies, or other things that we might have missed. That is why, whenever we finished answering a question, we used AI to verify and validate whether our answers were correct, if something was missing, and to fix any grammar errors. When we encountered steps that we could not immediately understand, we also asked AI to explain them clearly, which helped us understand the purpose and function of the steps better. Lastly, AI was also helpful in finding errors. For example, we noticed the inconsistency in the Chapter Questions ourselves, while AI helped us identify the programming warning and provided a corrected version of the code, which we also used in our program. </p> |
| Ch4 | <p align="justify"> We did not heavily use AI in this chapter. Instead, we mainly used it to validate our answers and check if there were any mistakes, inconsistencies, or missing information in our work. We used AI as an additional way to spot possible errors and make sure that our answers were reasonable before finalizing them. </p> |
| Ch5 | <p align="justify"> No AI tool was used in this chapter. We answered the questions and completed the activity based on our own understanding of the notebook and instructions provided. </p> |
| Ch6 | <p align="justify"> We also used AI on this chapter especially when we identify the value should be >2. Also we used it to further understand the meaning behind the code. </p>|
| Ch7 | <p align="justify"> We did use AI for identifying the error for this chapter. Even though the all of the program runs but to identify the remaining and obvious error is we used AI to resolve it and came up with cv=2. </p>|
| Ch8 | <p align="justify"> As for this chapter, even though the program proceed smoothly without an error, we used AI to understand fully the concepts behind those programs. </p>|
| Ch9 | <p align="justify"> For chapter 9, uppon discussing it with AI to further understand it there we identify that the final output for visualization of before and after discretization. </p>| 

## References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.
