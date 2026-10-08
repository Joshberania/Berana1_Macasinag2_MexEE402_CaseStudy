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
| Ch6 | [link]() | 
| Ch7 | [link]() | 
| Ch8 | [link]() | 
| Ch9 | [link]() |

## What we learned

One short paragraph per chapter, Ch1_2_3 to Ch9. Say what the chapter taught
you and what surprised you. Not what the library does, but what you understood.

| Chapter | Learnings |
|---|---|
| Ch1_2_3 | <p align="justify"> In these three chapters, we learned a lot beyond programming, especially about what we need to know first before proceeding to the next steps. As for Chapter 1, we were immediately introduced to the idea that not all raw data is ready for analysis. We cannot simply create a program and run it right away. Each dataset needs to go through preprocessing first, where the data is prepared before proceeding to machine learning. We were not surprised but rather expected that missing or inconsistent values could possibly cause messy results later on, which we have already experienced before in subjects where we dealt with programming. In Chapter 2, we realized that each data type in every column is important, which is interconnected with the previous chapter because this is where we started to encounter data processing and how the data is handled. We were surprised that we needed to distinguish between `object`, `int64`, and `float64` to determine what operation should be applied first before proceeding to the next step. Lastly, in Chapter 3, we learned that simply deleting missing values is not always the automatic solution when encountering them. We only learned now that there are different approaches to handling missing values, such as imputation, deletion, and prediction. This also helped us become more careful about looking closely at the program before making a risky solution, since we could either spend a long time troubleshooting to find the problem again or even have to repeat everything from the beginning. Overall, the questions helped us understand each process better, rather than simply copying the program, because they helped us connect the dots that seemed overwhelming at first. As time goes by, we become more engaged in programming without even noticing how many steps actually need to be followed. </p> |
| Ch4 | <p align="justify"> We felt that the process was becoming more understandable compared to the previous chapters because we were starting to see how the data is being prepared step by step before it can actually be used. Compared to Chapters 1 to 3, it seems that we're more focused on understanding the raw data, its different types, and how to handle missing values. However, in this chapter, we learned that converting categorical data into numerical values is not as simple as just assigning numbers to each category. In addition, we learned that the type of category matters because it determines what kind of encoding should be applied. At first, we thought that assigning numbers would already be enough, but we realized that doing so could create an unnecessary ranking between categories that do not actually have one. For example, Little, Medium, and Lots can be assigned numerical values because they have a natural order, while Sunny, Cloudy, and Rainy need a different approach because none of them is necessarily higher or lower than the others. This made us realize that even a simple step like converting data into numbers still requires us to understand the meaning and relationship of the categories first. Overall, this chapter helped us become more careful in handling categorical data because the way we encode it can affect how the machine learning model understands the information. </p> |
| Ch5 | <p align="justify"> In this chapter, we learned that preparing data does not stop after cleaning missing values and identifying the types of data. Compared to the previous chapters, the process in this chapter was shorter and more straightforward because we mainly focused on scaling the values of the features. We learned that the range of values matters because a variable with much larger numbers may have more influence on a machine learning model. At first, we thought that it would not matter as long as the data was correct, but we realized why scaling is used to put different features on a more comparable scale. We also learned that StandardScaler and MinMaxScaler work differently, but both can help make the features easier to compare. Overall, this chapter helped us understand that even a simple step like scaling can affect how a machine learning model handles different features. </p> |
| Ch6 | |
| Ch7 | |
| Ch8 | |
| Ch9 | |


## Errors we found

List any mistake you found in the original notebooks, and the correct version.
There are real ones in there. Finding them earns points.

| Chapter | Errors |
|---|---|
| Ch1_2_3 | <p align="justify"> So far, none of the programs crashed during the programming activities, but a warning appeared in Step 3, specifically during imputation. It indicated that using inplace=True on the Year and Publisher columns may no longer be valid in future versions of pandas. We corrected it by assigning the result of fillna() directly back to each column. Therefore, the corrected version is df['Year'] = df['Year'].fillna(df['Year'].mean()) and df['Publisher'] = df['Publisher'].fillna(df['Publisher'].mode()[0]). Moreover, we also noticed another issue, although it was not a major one, which was the confusion between the Chapter Questions and what was presented in Chapter 3 of the notebook. Only two methods were implemented in the code, which were imputation and deletion, while prediction was only discussed and not implemented. This was not a programming error, but rather an inconsistency in the instruction or question that might lead to confusion. Lastly, we encountered an issue where the vgsales.csv file was no longer available when we continued working on the notebook. To prevent the file from being lost again, we decided to mount our Google Drive and access the CSV file from there instead of relying on the temporary notebook storage. This helped us keep the dataset available even when the notebook session was restarted. </p> |
| Ch4 | <p align="justify"> In this chapter, we only encountered a small error while Mr. Beraña was manually typing the provided code instead of copying and pasting it directly into our Google Colab. He accidentally missed typing the colon (:) after the Lemonade Sold variable, which caused a syntax error when we tried to run the program. We were able to identify the problem by checking the code and comparing it with the provided version, then corrected it by adding the missing colon. Overall, this human error reminded us to be more careful, especially when inputting code, and to run the program from time to time so we can immediately identify and correct any errors. </p> |
| Ch5 | <p align="justify"> In this chapter, we did not encounter any major programming errors or warnings while running the code. The programs for StandardScaler and MinMaxScaler ran successfully and produced the expected results. We only had to make sure that we understood what happened to the values after scaling, since the numbers changed but their purpose was to put the features on a comparable scale. Overall, there were no significant errors that needed to be corrected in this chapter. </p> |
| Ch6 | |
| Ch7 | |
| Ch8 | |
| Ch9 | |

## Note on AI tools

Say whether you used an AI tool, and what for. This is not a penalty.
Hiding it is.

| Chapter | Justification on AI Tool Usage |
|---|---|
| Ch1_2_3 | <p align="justify"> Throughout these chapters, we admit that we used AI, but we mainly used it as a guide instead of relying too much on it. Our use of AI was similar to what we discussed in Chapter 1, where our initial answers were like raw data. They could contain mistakes, inconsistencies, or other things that we might have missed. That is why, whenever we finished answering a question, we used AI to verify and validate whether our answers were correct, if something was missing, and to fix any grammar errors. When we encountered steps that we could not immediately understand, we also asked AI to explain them clearly, which helped us understand the purpose and function of the steps better. Lastly, AI was also helpful in finding errors. For example, we noticed the inconsistency in the Chapter Questions ourselves, while AI helped us identify the programming warning and provided a corrected version of the code, which we also used in our program. </p> |
| Ch4 | <p align="justify"> We did not heavily use AI in this chapter. Instead, we mainly used it to validate our answers and check if there were any mistakes, inconsistencies, or missing information in our work. We used AI as an additional way to spot possible errors and make sure that our answers were reasonable before finalizing them. </p> |
| Ch5 | <p align="justify"> No AI tool was used in this chapter. We answered the questions and completed the activity based on our own understanding of the notebook and instructions provided. </p> |
| Ch6 | |
| Ch7 | |
| Ch8 | |
| Ch9 | |

## References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.
