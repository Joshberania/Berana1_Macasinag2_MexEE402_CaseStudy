# MexEE 402: Data Preprocessing Case Study

MexEE Elective 2: Data Science and Machine Learning
Batangas State University, Alangilan Campus
1st Semester, AY 2026-2027

## Members

| Name | Student Number | Section |
|---|---|---|
| Beraña, Steven Josh | 23-07634 | MEXE-4101 |
| Macasinag, Criz Glenn | | MEXE-4101 |

## Notebook links

| Chapter | Member 1 | Member 2 |
|---|---|---|
| Ch1_2_3 | [link]() | [link]() |
| Ch4 | [link]() | [link]() |
| Ch5 | [link]() | [link]() |
| Ch6 | [link]() | [link]() |
| Ch7 | [link]() | [link]() |
| Ch8 | [link]() | [link]() |
| Ch9 | [link]() | [link]() |

## What we learned

One short paragraph per chapter, Ch1_2_3 to Ch9. Say what the chapter taught
you and what surprised you. Not what the library does, but what you understood.

| Chapter | Learnings |
|---|---|
| Ch1_2_3 | <p align="justify"> In these three chapters, we learned a lot beyond programming, especially about what we need to know first before proceeding to the next steps. As for Chapter 1, we were immediately introduced to the idea that not all raw data is ready for analysis. We cannot simply create a program and run it right away. Each dataset needs to go through preprocessing first, where the data is prepared before proceeding to machine learning. We were not surprised but rather expected that missing or inconsistent values could possibly cause messy results later on, which we have already experienced before in subjects where we dealt with programming. In Chapter 2, we realized that each data type in every column is important, which is interconnected with the previous chapter because this is where we started to encounter data processing and how the data is handled. We were surprised that we needed to distinguish between `object`, `int64`, and `float64` to determine what operation should be applied first before proceeding to the next step. Lastly, in Chapter 3, we learned that simply deleting missing values is not always the automatic solution when encountering them. We only learned now that there are different approaches to handling missing values, such as imputation, deletion, and prediction. This also helped us become more careful about looking closely at the program before making a risky solution, since we could either spend a long time troubleshooting to find the problem again or even have to repeat everything from the beginning. Overall, the questions helped us understand each process better, rather than simply copying the program, because they helped us connect the dots that seemed overwhelming at first. As time goes by, we become more engaged in programming without even noticing how many steps actually need to be followed. </p> |
| Ch4 | |
| Ch5 | |
| Ch6 | |
| Ch7 | |
| Ch8 | |
| Ch9 | |


## Errors we found

List any mistake you found in the original notebooks, and the correct version.
There are real ones in there. Finding them earns points.

| Chapter | Errors |
|---|---|
| Ch1_2_3 | <p align="justify"> So far, none of the programs crashed during the programming activities, but a warning appeared in Step 3, specifically during imputation. It indicated that using inplace=True on the Year and Publisher columns may no longer be valid in future versions of pandas. We corrected it by assigning the result of fillna() directly back to each column. Therefore, the corrected version is df['Year'] = df['Year'].fillna(df['Year'].mean()) and df['Publisher'] = df['Publisher'].fillna(df['Publisher'].mode()[0]). Moreover, we also noticed another issue, although it was not a major one, which was the confusion between the Chapter Questions and what was presented in Chapter 3 of the notebook. Only two methods were implemented in the code, which were imputation and deletion, while prediction was only discussed and not implemented. This was not a programming error, but rather an inconsistency in the instruction or question that might lead to confusion. </p> |
| Ch4 | |
| Ch5 | |
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
| Ch4 | |
| Ch5 | |
| Ch6 | |
| Ch7 | |
| Ch8 | |
| Ch9 | |

## References

McKinney, W. (2021). Python for Data Analysis, 3rd ed. O'Reilly.
VanderPlas, J. Python Data Science Handbook.
Any other page or article you used.
